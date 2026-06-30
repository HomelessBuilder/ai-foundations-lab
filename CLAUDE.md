# AI Foundations Lab — Project Manager Context

## What This Project Is

A general AI literacy course for beginners with limited technical
background. Delivered as a hands-on lab sequence where students build
a real personal AI-assisted learning environment as they learn.

This is not a lecture course. Every lab produces a real artifact the
student keeps and uses going forward.

## About Diego

- Owner of San Diego AI HELP (sandiegoai.help) — AI consulting for San Diego small businesses
- Content brand: Homeless Builder — documents the journey of building with AI
- This course is a near-term revenue priority and potential foundation for a broader training business
- Advise first, act second — surface options before building anything

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
