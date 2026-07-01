# Content Decisions — Lab Content

*Internal notes for Diego and Sage. Not student-facing — do not surface
any of this in the lab files themselves.*

Design calls made during lab content development, plus scoping decisions
that intentionally leave something out. Kept here instead of inline in
the lab files so students never see author's-notes-style commentary.

---

## Lab 3 — No "prove it works" moment

Lab 3 (journal setup) deliberately does not include a close-and-reopen
or re-entry demonstration, unlike Lab 2's CLAUDE.md persistence test.
The re-entry payoff — proving the journal actually helps you pick a
project back up cold — is Module 5's entire purpose. Previewing it in
Lab 3 would blunt that landing. Conscious scoping call, not an
oversight.

## Lab 6 — No rollback/checkout taught

Lab 6 (git as a safety net) teaches `init`, `add`, `commit`, and viewing
history — but deliberately stops short of teaching an actual
rollback/checkout to an older snapshot. Reasoning: restoring an old
snapshot is real git territory, and a wrong move there can be genuinely
destructive for a beginner with no safety net of their own yet. This
matches the outline's "explicitly not full version control theory"
scope (`curriculum/outline.md`, Module 6). Conscious narrowing, not a
missed opportunity.

## Terminal navigation gap — resolved

Flagged during Lab 2 drafting: Labs 2, 3, 5, 6, and 7 all assume the
student can navigate a terminal into a specific folder (`cd`, or a
platform shortcut), but nothing taught this skill. Resolved by adding
Step 5 to Lab 0 ("One More Skill: Moving Around in the Terminal"),
teaching the drag-and-drop `cd` trick and the right-click "Open Terminal
Here" shortcut. All later labs that require re-navigation (Lab 2 Step 2,
Lab 5 Step 3) now reference back to that step instead of re-explaining
or silently assuming it. Single fix at the source, not patched
per-lab.

## Webpage as the canonical example

Labs 4 and 5 both used a personal webpage as the illustrative example,
even though the Lab 4 project menu offers four options (webpage, cheat
sheet, small game, to-do/FAQ document). Rather than patch each
occurrence individually, decided: webpage is the course's canonical
illustrative example, stated explicitly once in Lab 4 Step 1 ("One
heads-up..."), with a light one-line reminder retained in Lab 5 since
it's a separate lab file a student might return to after time away.
