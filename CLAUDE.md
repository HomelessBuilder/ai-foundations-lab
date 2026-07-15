# AI Foundations Lab — Project Manager Context

## What This Project Is

A general AI literacy course for beginners with limited technical
background. Delivered as a hands-on lab sequence where students build
a real personal AI-assisted learning environment as they learn.

This is not a lecture course. Every lab produces a real artifact the
student keeps and uses going forward.

## Path Definition (Decided 2026-07-01)

This project is the **hybrid model** — the current and alpha release path.
A future in-browser platform is under separate development in
`~/ai-course-platform/`. This project feeds that platform; it is not
replaced by it.

## Delivery: Hybrid Web Application

The course is delivered through a browser-based web interface. Lab
content and live Sabia chat are in the browser. Building work is done
locally by the student using Claude Code or Claude Desktop.

**Supported local tools:**
- **Claude Code** (terminal-based) — full capability, requires terminal comfort
- **Claude Desktop** (GUI app, no terminal) — full Claude capability without
  a terminal; a meaningful option for students intimidated by the command line

The pre-lab setup module should present both options and let the student
choose. Lab content references both paths where they diverge.

Key implications for content development:
- Lab content is written to render in a browser, not as standalone files
- The lab manual is fluid — it evolves as the student builds, not a static PDF
- Module unlocking is built into the interface (see below)
- Sabia operates inside this environment as the embedded instructor

**Module unlock system:**
The course ships as a complete package. Unlock modes:
- Self-guided: all modules open at start
- Pay-as-you-go: modules unlock per payment (specific student use case)
- Sabia-gated: Sabia reviews student artifact before unlocking next module

**Startup module (Module 0):**
Before the seven core modules, a technical onboarding module walks the
student through Claude Code installation and orientation. This is the
first thing a student does. It affects the current outline — Module 1
("What Are We Actually Doing?") may need to shift or merge with setup.

The web interface is a separate development project from this content
folder. Sabia develops course content here; the interface is built
elsewhere when ready.

## About Diego

See `~/ABOUT-ME.md` for baseline identity/voice.

- This course is a near-term revenue priority and potential foundation for a broader training business
- Advise first, act second — surface options before building anything

Working notes for this project (design calls, scoping decisions) live in
`instructor/content-decisions.md` — that file is this project's lightweight
Notes equivalent; don't create a separate one.

## The Student

- New to AI tools — may never have used Claude Code or any developer tooling
- Limited technical background — not assumed to know git, terminals, or code
- Motivated but cautious — needs wins early, complexity introduced gradually
- Goal: leave with working infrastructure and the confidence to keep learning

## What the Student Builds

A simplified version of Diego's own recursive development ecosystem:
- A project folder with a CLAUDE.md giving AI context
- A personal learning journal (simplified claude-journal)
- Basic git tracking of their work
- Prompting habits and session documentation discipline

By the final lab they have something real — not just notes.

## Course Structure (Working Outline)

**Module 1 — Understanding AI Tools**
What Claude Code is, how it differs from ChatGPT, what "context" means,
why documentation matters. Conceptual groundwork before any tools.

**Module 2 — Your First Project Folder**
Set up Claude Code, create a project folder, write their first CLAUDE.md.
First experience of giving AI structured context.

**Module 3 — The Learning Journal**
Start a personal learning journal. Write their first entry. Understand
why re-entry context matters. First taste of recursive documentation.

**Module 4 — Building Something Small**
Pick a real micro-project and build it with AI assistance. Practice
iteration, course-correction, and asking better questions.

**Module 5 — Documenting and Handing Off**
Log the session. Experience picking up where they left off using their
own documentation. The recursive payoff becomes real here.

**Module 6 — Git as a Safety Net**
Basic git — init, add, commit. Not full git — just enough to feel safe
making changes. Framed as an undo button, not version control theory.

**Module 7 — What Comes Next**
Where to go from here. More advanced topics. How this foundation connects
to more powerful usage. Course close.

## Folder Structure

```
ai-foundations-lab/
├── CLAUDE.md              ← this file
├── VISION.md              ← founding scope and decisions
├── curriculum/
│   ├── outline.md         ← full course structure
│   └── labs/              ← one file per lab
├── templates/             ← starter files given to students
│   ├── CLAUDE.md          ← student's simplified context file
│   └── journal/           ← student's learning journal starter
├── instructor/            ← notes, pacing, facilitation guidance
└── adaptations/           ← themed versions (trading, healthcare, etc.)
```

## What Is NOT in This Course

- MySQL or any database
- Multiple GitHub accounts or SSH key management
- AWS or cloud infrastructure
- The overseer/monitor pattern
- Anything requiring terminal comfort beyond the basics introduced here

## Relationship to Diego's Ecosystem

This course is modeled on what Diego built with his own meta-system but
simplified for a non-technical audience. The templates in `/templates/`
are stripped-down versions of his actual working files. The DEVLOG
entries in claude-journal are source material for lesson content and
examples.

The `/adaptations/` folder is where themed versions live — a trading
version, a healthcare version, etc. — applied on top of this general
framework. Do not build adaptations until the general course is stable.

## Standing Rules

- No file deletions without explicit instruction from Diego
- No permanent changes (commits, pushes, installs) without confirmation
- Advise first — surface options before building
- When scope feels unclear, ask rather than assume
