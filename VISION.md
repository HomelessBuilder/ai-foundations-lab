# AI Foundations Lab — Vision and Founding Decisions

*Written by: Overseer instance (~/) in collaboration with Diego*
*Date: 2026-06-30*

---

## Why This Course Exists

Diego built a recursive, self-improving AI development ecosystem over the
course of several weeks — working with Claude Code to create tooling,
journals, documentation systems, and infrastructure that compound on
themselves. The process of building it was itself the education.

The insight: that process is teachable. Stripped of its complexity, the
core loop — give AI context, build something, document what happened,
pick up where you left off — is accessible to anyone. A non-technical
person who learns that loop walks away with real capability, not just
familiarity with a chatbot.

This course teaches that loop, hands-on, with a real artifact at the end.

---

## The Founding Decision: Build, Don't Watch

Most AI courses are observational. Students watch demos, read prompts,
copy examples. They leave knowing what AI can do but unsure how to apply
it to their own work.

This course is different: every module produces something the student
keeps. By module three they have a working journal. By module six they
have git-tracked infrastructure. The learning and the building are the
same activity.

This is the core design constraint. If a module doesn't produce a
lasting artifact, it needs to be redesigned or cut.

---

## The Model: Diego's Ecosystem, Simplified

Diego's full meta-system includes:
- Multiple Claude Code instances (overseer + project managers)
- A federated journal model with MySQL backend (devlog-engine)
- SSH key management for multiple GitHub accounts
- A passive monitor running hourly via cron
- AWS infrastructure for the live website

None of that belongs in a beginner course.

What does transfer:
- The CLAUDE.md pattern — giving AI structured context
- The learning journal — documenting sessions for re-entry
- The handoff format — communicating across sessions
- Basic git — tracking work as a safety net
- The recursive principle — documentation that helps you learn more

The student's output is a personal AI-assisted learning environment.
Simpler than Diego's, but built on the same principles.

---

## The Adaptation Model

The general course is the foundation. Themed versions (trading, healthcare,
real estate, etc.) are adaptations that:
- Use domain-specific examples in the labs
- Frame the micro-project around a domain problem
- Adjust language and context to the audience

Adaptations live in `/adaptations/` and are built only after the general
course is stable. The first adaptation will likely be the AI trading
version (for a specific prospective student).

---

## What Success Looks Like for the Student

At the end of the course, the student has:
- Claude Code installed and working
- A project folder with a CLAUDE.md they wrote themselves
- A learning journal with at least three entries
- At least one small project built with AI assistance
- A git-tracked record of everything they built
- Confidence to open a new session and pick up where they left off

They don't need to understand everything. They need to have done it.

---

## Open Questions

- Delivery format: self-paced written guide, video + written, live cohort?
- Pricing and platform: Teachable, Gumroad, direct sale, something else?
- Prerequisite tech: what's the minimum setup a student needs before Lab 1?
- Assessment: how does Diego know a student completed each lab?
- Certificate or credential: is there a completion artifact beyond the files they built?

These are not blocking course development — they're decided when Diego is
ready to sell, not when he's building content.
