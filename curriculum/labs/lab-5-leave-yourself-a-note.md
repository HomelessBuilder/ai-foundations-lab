# Module 5 — Documenting and Handing Off
## Lab 5: "Leave Yourself a Note"

*Status: Draft — for Diego's review.*

**What you'll walk away with:** A second journal entry, a handoff note,
and proof — real proof, not just an idea — that your own notes can bring
you back into a project cold.

**Time:** About 60 minutes. Slower is fine.

---

### Before We Start

Back in Lab 1, we talked about a loop: context, build, document,
re-enter. You've lived two-thirds of it already — you gave Claude Code
context in Lab 2, and you built something real in Lab 4. Today we close
the loop: we document what happened, and then we actually re-enter,
cold, using nothing but what we wrote down.

This is the lab where the whole point of this course stops being an
idea and becomes something you've done yourself.

---

### Step 1 — Log What You Built

Pull up the summary Claude Code gave you at the end of Lab 4. Ask it to
turn that into your next journal entry:

```
Can you save a journal entry for what we built in the last lab, as journal/entry-2.md?
```

If you don't have that summary handy, ask Claude Code: "Can you look at
my project folder and tell me what we built?" — it can reconstruct it
from the files.

This one's straightforward — same pattern as entry-1, just a new chapter
in the same paper trail.

---

### Step 2 — Write a Handoff Note

A journal entry tells a story: here's what happened, in order. A
**handoff note** does something different — it's a quick briefing for
whoever opens this project next, so they can get oriented in seconds
instead of digging back through history. Even though that "whoever" is
almost always going to be you.

A good handoff note answers three things:
1. What is this project?
2. What's been done so far?
3. What's the very next thing to do?

Ask Claude Code to draft one:

```
Can you write a handoff note for this project as journal/handoff.md, covering what this project is, what's been done, and what to do next?
```

Read it before you move on. If anything in it feels vague or generic —
like "made progress on the project" — push back and ask for something
more specific. That's not a small nitpick:

> **Worth knowing:** a handoff note is only as good as its specifics. "I
> worked on my project" tells future-you nothing. "Built a webpage with
> my name and interests, still need to add a photo" tells future-you
> exactly where to stand. Vague notes feel like documentation but
> function like nothing at all.

If you want a sense of what a solid one looks like:

```markdown
# Handoff Note

## What This Is
A personal webpage project — my name, a short bio, and a list
of my interests.

## What's Done
Built the first version with Claude Code's help. Has a title,
two sentences about me, and a short interests list.

## What's Next
Want to add a photo and maybe a favorite quote. Haven't started
on that yet.
```

Yours will reflect what you actually built — use the same three
sections, just swap in your own project details.

---

### Step 3 — The Real Test

This is the part that matters most, so don't skip it or rush it.

1. Close Claude Code completely. Close the terminal window too.
2. Step away. The longer you go, the more real the test — 15 to 20
   minutes is better than 5. Go make coffee, take a walk, do something
   else entirely. Come back when you've genuinely moved on, not just
   paused.
3. Come back, open a terminal in your project folder (the navigation
   trick from Lab 0's Step 5), and start Claude Code fresh.
4. Type only this — nothing more, don't re-explain anything yourself:

```
I'm picking this project back up — can you tell me where things stand?
```

Watch what happens. It should tell you, accurately, what this project
is, what's been built, and what's next — pulled entirely from your
CLAUDE.md and your handoff note. You didn't remind it of anything. It
didn't remember you. It just read what you left behind.

> **If it feels a little off or incomplete** — that's not a failure,
> that's useful information. It means your handoff note needs a bit more
> specific detail somewhere. Go back, add what was missing, and try the
> test again. This is exactly the kind of course-correction we practiced
> in Lab 4, just aimed at your notes instead of your project.

---

### Step 4 — Write Down What Just Happened

This moment is worth keeping, not just experiencing. Ask Claude Code:

```
Can you save one more entry, journal/entry-3.md, about what just happened — what the test felt like, whether the re-entry worked, and what surprised me?
```

That's your third journal entry, and it's a different kind than the
first two — this one's about the process itself, not just what you
built.

---

### Where We Land

Say that back to yourself for a second: you closed everything, walked
away, came back with a system that has no memory of you — and it still
knew exactly where you stood. Not because it remembered. Because you
wrote it down well enough that it didn't need to.

That's the whole loop, complete: context, build, document, re-enter.
You've now done every piece of it yourself, for real.

Next lab, we add one more layer of safety on top of everything you've
built — git, and the confidence to change things without fear of losing
them.
