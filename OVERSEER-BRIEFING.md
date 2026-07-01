# Overseer Briefing — 2026-07-01

*From: Overseer instance (~/) | To: Sage | Action required*

Two independent workstreams. Do them in the order listed.

---

## Part 1 — Three Content Items for the Lab Files

These need to land in the course content before the pre-lab and lab revisions are finalized.

### 1. Claude Code / Claude Desktop as a hard prerequisite

The pre-lab module should open with a clear, upfront statement — not buried in a step — that taking this course requires Claude Code or Claude Desktop set up and working before Lab 0 begins. Alpha and beta students handle their own Anthropic account creation before starting. The pre-lab walks through configuration, not account signup. Both tools are supported — let the student choose at the start of the pre-lab and follow the appropriate setup path from there.

### 2. Support email placeholder

Add `[SUPPORT EMAIL]` — exactly that string, in brackets — at any point in the labs where a student is most likely to get completely stuck and need human help. Likely spots: the pre-lab (if setup fails), Lab 0 (first interaction), Lab 6 (git installation). One line, natural tone: something like *"If you get stuck here and can't get past it, email [SUPPORT EMAIL] and we'll help you directly."*

### 3. Lab 7 completion hook

The closing paragraph of Lab 7 should hand the student somewhere rather than simply ending. After the journal entry artifact, add a final beat directing them to a completion page using `[COMPLETION URL]` as the placeholder. Tone: a handoff, not a goodbye. Something like: *"When you're ready, head to [COMPLETION URL] — there's one more thing waiting for you there."* The completion page itself is a separate web build — just the hook needs to be in Lab 7 now.

---

## Part 2 — Sage Chat Interface Build

Build a Sage chat interface as a single-page web app on sandiegoai.help. This is the minimum viable platform for alpha testing — no student accounts, no payment, no module unlock. Just the chat. It should look and feel like a real product, not a prototype.

**Build these three steps in order. Do not skip ahead.**

### Step 1 — UI mockup with scripted responses (build and deliver first)

Build the full chat page UI. For this step, Sage's responses are pre-written — no API calls, no backend. Write 5–6 sample Sage exchanges that represent how Sage would actually respond during Lab 0 or Lab 1. These scripted responses serve two purposes: they let Diego see how the interface looks and feels before any backend work begins, and they demonstrate Sage's voice in context.

The page should be:
- On-brand with sandiegoai.help — navy/blue palette (`--navy: #0d1f3c`, `--blue: #1a56db`, `--blue-light: #3b82f6`), DM Sans font, same design tokens as the rest of the site
- Sage clearly identified by name with a brief descriptor ("Your AI course instructor")
- Conventional message thread layout (user messages right, Sage messages left)
- A "Sage is thinking..." indicator visible between message and response in the scripted flow
- No login, no session persistence — fresh conversation on each page load
- Mobile-responsive
- `noindex, nofollow` meta (alpha only)
- Path: `sandiegoai.help/sage/` (place the file at `src/sage/index.html`)

Diego reviews the UI and approves before Step 2 begins.

### Step 2 — Lambda proxy backend (after UI approval)

A Lambda function that:
- Receives the student's message and full conversation history from the client
- Prepends Sage's full persona from `instructor/SAGE.md` as the system prompt
- Calls the Anthropic Claude API — model `claude-sonnet-4-6`
- Returns Sage's response to the client
- Stores nothing server-side — conversation state is stateless, kept in the browser; if the student refreshes, the conversation resets (acceptable for alpha)

The Anthropic API key goes in Lambda's environment variables — never in client-side code. API Gateway route: POST `/sage`, using the same AWS infrastructure pattern as the existing contact form endpoint (`https://8uyh0ftkel.execute-api.us-east-2.amazonaws.com/prod/contact`). The new route will be `/prod/sage` on the same gateway or a new endpoint — to be confirmed when building.

### Step 3 — Wire the UI to the backend (after Lambda is deployed)

Replace the scripted responses with live API calls to the Lambda endpoint. Test end-to-end. Two-person test cost is under $1 — not a concern.

---

## Sequence Summary

1. Deliver Step 1 (UI mockup) → Diego reviews
2. Build Step 2 (Lambda backend) → deploy and confirm
3. Wire Step 3 (connect UI to Lambda) → test live

Start with Part 1 content items, then move to Part 2 Step 1.
