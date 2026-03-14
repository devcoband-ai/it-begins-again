# David's Guide

Welcome to the workspace. Here's what you need to know.

## Where to Put Your Stuff

| What you have | Where it goes |
|---|---|
| Writing — stories, drafts, notes, book material, fragments | `content/writing/` |
| Art — scans, illustrations, photos, analog press work | `content/art/` |
| Music — recordings, lyrics, song notes | `content/music/` |
| Not sure yet | `content/ideas/` |

Don't worry about naming conventions or formatting. Drop it in, Jeff and Devco will sort it out.

## How to Get Files Here

For now, send everything to Jeff. He'll get it into the repo. Once you have a GitHub account and are added as a collaborator, you can upload directly:

1. Go to the folder (e.g. `content/art/`)
2. Click **Add file → Upload files**
3. Drag your files in
4. Click **Commit changes**

That's it. No command line. No special tools.

## File Tips

- **Images:** JPG or PNG. If you're scanning analog press work, scan at 300 DPI or higher — we can always compress, but we can't add detail back.
- **Writing:** Plain text, Word docs, or PDFs all work. If you write in Google Docs, you can share the link and we'll pull it in.
- **Music:** MP3, WAV, or even a voice memo from your phone. Rough is fine.
- **Naming:** Descriptive names help. `sandersville-barn-1994.jpg` beats `IMG_4032.jpg`. But don't stress about it — we can rename later.

## The Most Important Thing: GitHub

Before AI tools, before Claude, before anything else — learn GitHub. This is the foundation.

Here's why: once you start creating with AI, the volume of work gets big fast. Drafts, revisions, images, variations, experiments. Without source control, you'll end up with a folder full of `final_v2_REAL_final_march14.doc` and no idea which version is the right one or what changed between them.

GitHub solves that. Every change is tracked. Every version is saved. You can go back to any point in time and see exactly what something looked like. You can experiment without fear of losing what worked.

Think of it like this: your analog press work has editions. Each print run is a version. GitHub does the same thing for digital work — every save is an edition, and you never lose a previous one.

### Your First Workflow

This is the core loop. Once you can do this, you can do everything else.

**One-time setup** (you only do this once):

```bash
# Open Terminal on your Mac (it's in Applications → Utilities)

# Clone the repo — this downloads the entire project to your computer
git clone https://github.com/devcoband-ai/it-begins-again.git

# Move into the project folder
cd it-begins-again
```

Now you have the whole project on your machine.

**Every time you want to add something:**

```bash
# Step 1: Pull the latest changes (in case Jeff added something)
git pull

# Step 2: Add your files to the ideas folder
# Just drag your files into the content/ideas/ folder using Finder
# Or copy them from the command line:
cp ~/Desktop/my-sketch.jpg content/ideas/

# Step 3: Stage your changes (tell git what you're adding)
git add .

# Step 4: Commit with a message (describe what you added)
git commit -m "Added barn sketch from 1994 - David"

# Step 5: Push it up (sends your changes to GitHub)
git push
```

That's it. Five commands. Pull, add, stage, commit, push.

**Tag Jeff as a co-author** on any commit by adding this to the end of your commit message:

```bash
git commit -m "Added new poem draft - David

Co-authored-by: Jeff Highman <jhighman@gmail.com>"
```

The blank line before `Co-authored-by` matters — keep it there.

### What to Learn Next

Once you're comfortable with the basic loop:

1. **Commit messages** — think of these as edition notes. "First draft of barn poem" is better than "added stuff"
2. **Viewing history** — `git log` shows everything that's happened, who did it, when
3. **Branches** — working on something experimental without affecting the main version (this comes later)

Jeff will walk you through each step. No rush. But the pull-add-commit-push loop is the one thing to get comfortable with first.

### Why It Matters for Artists

You're going to produce a lot of work. AI accelerates creation — what used to take weeks can happen in a day. The artists who thrive with these tools aren't the ones who generate the most. They're the ones who can organize, curate, and find their own work six months later.

GitHub is how you stay in control of your own output.

---

## Claude — Your AI Collaborator

You already have a Claude subscription. Here's how to think about the two ways to use it:

**Claude Chat** (claude.ai) — the web interface you've been using. Good for conversations, brainstorming, asking questions. Think of it as talking to someone.

**Claude Code** (command line) — this is where it gets powerful. Claude at the command line can read and write files, organize your work, help you draft and revise, and interact directly with this repo. Think of it as working *with* someone — side by side, in your actual workspace.

The goal is to get you comfortable at the command line over time. Not all at once. Jeff will walk you through it as we go. The commands are simple — you're mostly just talking to Claude in a terminal instead of a browser.

### Getting Started with Claude Code

When you're ready (Jeff will help with setup):

1. Open Terminal on your Mac
2. Type `claude` and hit enter
3. You're in. Just talk to it. Ask it to read a file, write something, organize your folder, whatever you need.

That's it. No special syntax. No programming. Just a conversation — but one where Claude can actually touch your files.

### Why the Command Line Matters

The chat interface is a notepad. The command line is a workshop. When Claude can see your files, read your drafts, look at your art, and write directly into your project — the collaboration gets real. You describe what you want, Claude builds it, you refine it together.

This is how Jeff works with Devco every day. Same tools, same workflow. You'll get there.

## Other Tools You'll Meet

- **Suno** — AI music generation. Describe a mood, a genre, a feeling. It builds a track. Jeff has the pro account. [Hear samples](https://suno.com/playlist/0d8339cb-779b-437a-a6d3-d5602a47e77e)
- **Nano Banana** — AI image generation. Describe what you see in your head. It renders it. Iterate until it matches.

## What Happens to Your Work

1. You send it → it goes in the repo
2. We shape it together — find structure, connections, threads
3. When something's ready, it gets staged on the DevCo Platform (private engine, you don't need to touch it)
4. Finished work comes back to you — your content, your copyright, your call on where it goes

## The One Rule

Everything here belongs to you. Nothing gets published without your say-so.
