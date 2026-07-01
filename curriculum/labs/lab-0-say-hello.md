# Module 0 — Getting Set Up
## Lab 0: "Say Hello"

*Status: Draft — for Diego's review.*

**What you'll walk away with:** Claude Code installed and running on your
own computer, and a saved copy of your very first real exchange with it —
proof, in your own words, that it works.

**Time:** About 60 minutes. There's no clock here — go slower if you need to.

---

### Before We Start

Hi — I'm Sage. I'm going to be with you through this whole course, and
this first lab is the easiest one you'll do: we're just getting the tool
installed and saying hello to it.

That's it. No theory, no jargon, nothing to memorize. But don't mistake
"simple" for "not real" — by the end of this lab, you will have a working
AI development tool running on your own machine, and you will have used
it. That's not nothing. Most people never get this far.

Let's go.

---

### Step 1 — Installing Claude Code

The download link for your operating system is on this page — click it
and follow the installer. Here's what's actually happening while you
wait for it to finish:

> **Worth knowing:** Claude Code isn't a website or an app you open in
> your browser like ChatGPT. It installs directly onto your computer,
> which means it can see your files and work with them directly —
> that's the whole reason it can *build* things with you instead of just
> talking about them. You're not installing "another chatbot." You're
> installing a tool that can act.

If the installer asks you questions you don't recognize, the defaults
are almost always fine. When in doubt, press enter and keep going.

---

### Step 2 — Opening It Up

Once it's installed, you'll open something called a **terminal** — a
plain, text-only window for typing instructions directly to your
computer. It looks old-fashioned. It is old-fashioned. It's also simpler
than it looks: you type a line, press enter, something happens.

Open your terminal and type:

```
claude
```

Press enter. If you see a prompt waiting for you to type something —
that worked. Claude Code is running.

> **This part trips people up, and that's normal.** If nothing happens,
> or you get an error, don't panic and don't blame yourself — installers
> misfire for all kinds of small reasons that have nothing to do with
> you doing something wrong. Close the terminal, open a fresh one, and
> try `claude` again. If it still won't run, that's a real thing to flag,
> not a sign you're behind.

---

### Step 3 — Say Hello

Now for the actual moment this lab is about. Type this, exactly as
written, and press enter:

```
Hi! Can you introduce yourself and tell me what just happened when you started up?
```

Read whatever it says back to you.

> **Worth knowing:** notice that it answered *you specifically*, in this
> moment, about *this* window, on *your* machine — not a generic canned
> reply. That's the difference between this and a chat website. A chat
> window is a conversation. What you just opened is closer to a
> collaborator sitting at your computer with you. We'll go a lot deeper
> on this in the next module — for now, just notice it.

If the response feels strange or too technical in places — that's fine.
You don't need to understand everything it says. You just did something
real: you had your first real exchange with the tool you're going to be
building with.

---

### Step 4 — Save What Just Happened

Before we close this out, let's keep proof this happened — and let's
have Claude Code do it, not us.

Type this and press enter:

```
Can you save a summary of what we just talked about to a file called hello.txt?
```

Watch what happens. Claude Code creates the file itself, right there on
your computer.

> **Worth knowing:** that's the same capability from Step 3, showing up
> again in a more visible way. A chat window can tell you *how* to save
> a file. What you just used actually reached out and created one — on
> your machine, for real. That's the difference we keep coming back to.

Don't worry about organizing this properly yet. In Lab 2 we'll build a
real project folder and this will find a proper home. For now, it just
needs to exist.

---

### Step 5 — One More Skill: Moving Around in the Terminal

One last thing before we close out, because you'll need it starting next
lab: the terminal is always "standing" inside some folder, and moving it
to a different folder is called **navigating**. Right now it's probably
sitting wherever it opened by default — not necessarily where your files
are.

The easiest way to move it: type `cd ` (with a space after it, nothing
else yet), then drag the folder you want from your file browser (Finder
on Mac, File Explorer on Windows, or your file manager on Linux)
directly into the terminal window. It will auto-fill the folder's
location for you. Press enter, and the terminal is now "standing" in
that folder.

Some systems make this even easier — right-click a folder and look for
an option like "Open Terminal Here" or "Open PowerShell window here." If
you see that, it does the same thing in one click.

Try it now: navigate into whatever folder you saved `hello.txt` in, and
confirm you're there by typing `claude` again — a fresh session should
still be able to find and read that file.

> **Worth knowing:** this feels fiddly the first couple of times and
> then becomes automatic. Every lab from here on starts with "open a
> terminal in your project folder" — that instruction means exactly
> this, every time.

---

### Where We Land

Take a second before you move on. A few minutes ago, you didn't have
this tool. Now it's installed, it's running, and you've had a real
conversation with it — one that you kept a copy of.

We've got this. Next up, in Module 1, we slow down and actually talk
about what this thing is and why it's different from what you've
probably used before. You'll have this session to point back to, because
now you've actually seen it.
