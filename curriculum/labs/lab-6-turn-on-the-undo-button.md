# Module 6 — Git as a Safety Net
## Lab 6: "Turn On the Undo Button"

*Status: Draft — for Diego's review.*

**What you'll walk away with:** Your project folder tracked by git, with
a real commit history — starting from the micro-project you built in
Lab 4.

**Time:** About 60 minutes. Slower is fine.

---

### Before We Start

You've built something real and you've documented it well enough to
pick back up cold. Today we add one more layer: the confidence to change
things without being afraid of breaking them.

That's all git is, for our purposes today. Not version control theory,
not branches, not anything complicated — just a safety net. Think of it
like a save point in a game: you can keep playing, and if something ever
goes wrong, there's a point you can always get back to.

---

### Before Step 1 — Check You Have Git

Ask Claude Code: "Is git installed on this computer?" If it isn't, ask
it to walk you through installing it. This takes a few minutes and only
happens once — Mac computers usually have it already. Windows computers
usually need Git for Windows added. On Linux, it isn't always
pre-installed, but Claude Code can check and walk you through a one-line
install command for your system.

---

### Step 1 — Turn On Tracking

Ask Claude Code:

```
Can you turn on git tracking for this project folder?
```

Claude Code will run something called `git init`. Nothing about your
files changes — this just switches on the recording. From now on, git is
quietly watching this folder, ready to save snapshots whenever you ask
for one.

A hidden folder called `.git` will appear in your project — that's
git's own storage space. You never need to open or touch it directly.

> **Worth knowing:** `init` is short for "initialize" — just a fancy way
> of saying "start tracking here." You'll see this word again if you
> ever read about git elsewhere. Now you'll know what it means.

---

### Step 2 — Take Your First Snapshot

A snapshot in git happens in two small steps: telling it what to save,
and then actually saving it. Ask Claude Code:

```
Can you save a snapshot of my project as it is right now, with a message describing what's in it?
```

Behind the scenes, that's two commands: `git add`, which grabs
everything you want included, and `git commit`, which actually saves the
snapshot along with a short message about what it contains.

You'll see some text appear in the terminal after each command — that's
git confirming it worked. As long as there's no red error text, you're
good, even if the wording looks a little technical.

Your first snapshot captures everything in the folder — your CLAUDE.md,
your journal, your project files, all of it. That's exactly right: the
whole thing is worth keeping, not just the project you built in Lab 4.

> **Worth knowing:** a "commit" is just git's word for a saved snapshot.
> Every commit is a point you could always return to later. You just
> created your first one.
>
> Claude Code wrote today's snapshot message for you. That's fine for
> now — as you get more comfortable with git, describing your own
> snapshots in your own words is a habit worth building.

---

### Step 3 — Make a Change, Snapshot Again

Go back to your micro-project from Lab 4 and ask Claude Code for one
small tweak — anything. Then take another snapshot:

```
Can you save another snapshot with a message describing what changed?
```

Do this once more if you'd like. The habit is the whole point: build
something, snapshot it, change something, snapshot again.

> **This part trips people up sometimes** — it can feel like you're
> asking to "save" the same thing you already saved. You're not. Each
> snapshot is its own separate point in time, even if the file only
> changed a little. That's exactly what makes this a safety net: lots of
> small, cheap points to come back to, not one single fragile save.

---

### Step 4 — See Your Safety Net

Ask Claude Code:

```
Can you show me the history of snapshots I've made so far?
```

You should see each commit you made, in order, with the messages you
gave them. That list is your safety net, made visible. Every one of
those points still exists, exactly as it was.

> **Worth knowing:** we're not going to practice actually rolling back
> to an older snapshot today — that's a real thing you can do, but it's
> a bigger topic than this lab needs. For now, just know it's possible:
> if you were ever in real trouble, you could ask Claude Code to help
> you get back to any point on this list. That possibility existing is
> what "safety net" means.

---

### Where We Land

You didn't just learn what git is — you built a real habit: change
something, snapshot it. That habit is what turns "I'm afraid to touch
this in case I break it" into "I can try things, because I've got a way
back."

Next lab, we close things out — and look at where all of this goes from
here.
