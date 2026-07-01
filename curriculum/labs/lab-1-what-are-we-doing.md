# Module 1 — Understanding AI Tools
## Lab 1: "What Are We Actually Doing?"

*Status: Draft — for Diego's review.*

**What you'll walk away with:** A short written reflection —
"What I Want to Build" — saved as a real file. It's the seed of
something bigger: next lab, it becomes the first draft of your project's
CLAUDE.md.

**Time:** About 60 minutes. Slower is fine.

---

### Before We Start

Last time, we got Claude Code installed and said hello to it. If you
still have that `hello.txt` file sitting there — good. We're going to
point back at it a few times in this lab, because everything here is
easier to explain when you've already seen it happen once.

Today we're not building anything yet. We're slowing down to understand
what this tool actually is. That might feel like a step backward after
the momentum of Lab 0 — it isn't. You can't use a tool well if you don't
know what kind of tool it is, and by the end of this lab, you will.

---

### Chat vs. Agent

You've probably used a chat website before — ChatGPT, or something like
it. You type a message, it types one back. That's the whole interaction:
words in, words out.

Go back and look at what happened in Lab 0. When you typed `claude` and
said hello, Claude Code didn't just answer with words — in Step 4, it
reached into your actual computer and created a real file. A chat
website can't do that. It can only talk *about* doing something. What
you're using is different enough that it gets its own word: an **agent**.

> **In plain terms:** a chat tool talks. An agent acts. It can look at
> your files, create new ones, run things on your computer — with your
> permission, and only what you ask it to do. That's the entire reason
> this course is possible: you're not just going to talk about building
> something. You're going to actually build it, with something that can
> reach into the work alongside you.

---

### What "Context" Means

Here's a question: if you hired a freelancer tomorrow and wanted help
with a project, what would you have to explain to them before they could
do anything useful? Probably: what the project is, what you've already
tried, what you want, maybe some background on your situation. Every
time you brought in someone new, you'd have to explain all of it again —
unless you'd written it down somewhere they could read first.

That written-down version — what the situation is, what matters, what's
already been decided — is what we mean by **context**. It's not a
technical term hiding something complicated. It's just: the background
information that lets someone (or something) act with understanding
instead of guessing.

Right now, Claude Code knows almost nothing about you or what you're
trying to do. Every time you open it, it's meeting you fresh. That's not
a flaw — it's actually a design choice we're going to use to our
advantage. Giving it context on purpose, in writing, is exactly what the
rest of this course teaches you to do.

> **This part is a little abstract, and that's normal.** "Context" is
> one of those words that clicks once you've actually done it, not
> before. You don't need to fully grasp it right now — Lab 2 is where
> you build your first real piece of it. For today, just hold onto the
> idea: writing things down on purpose changes what this tool can do
> for you.

---

### Why Documentation Matters — and the Loop We're Building

Here's the shape of what this whole course is teaching you, in one
sentence: **give it context, build something, write down what happened,
come back and pick up where you left off.** That's the loop. Every
module from here on is one piece of it.

- **Context** — telling it what it needs to know (starting next lab)
- **Build** — actually making something with it (Module 4)
- **Document** — writing down what happened, so it isn't lost (Modules 3 and 5)
- **Re-enter** — coming back later and picking up cleanly, using your own notes (Module 5)

You don't need to memorize this. You're going to live it, one lab at a
time, and by Module 5 it'll feel obvious instead of abstract. Documenting
isn't extra homework bolted onto the real work — it's what makes the
next session possible without starting over. That's the whole reason
"context" matters in the first place.

---

### Your Turn: What I Want to Build

Open Claude Code. Have a real conversation with it — no script to
follow, just talk to it the way you'd talk to a person you just met who
asked what you're hoping to get out of this. Some things you might
mention:

- What made you want to learn this
- What you'd love to be able to build or automate
- What's felt out of reach for you before now

If you're staring at a blank cursor and not sure how to start, that's
completely normal — try opening with something like:

> "I'm just starting to learn AI tools — here's what I'm hoping to be
> able to do someday..."

Then just keep talking from there.

When you feel like you've said what you actually think, type this and
press enter:

```
Can you save a short summary of what I just told you to a file called what-i-want-to-build.txt?
```

That's your artifact for this lab. Not a polished mission statement —
just something true, in your own words, that exists as a real file now.

---

### Where We Land

You now know something most people who use AI tools casually never
bother to learn: the difference between talking *at* something and
building *with* it. That's not a small thing.

Next lab, we give Claude Code its first real, permanent piece of
context — a project folder with a CLAUDE.md, seeded straight from the
file you just created. We've got this. Let's keep going.
