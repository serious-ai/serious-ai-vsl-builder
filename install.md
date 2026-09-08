---
name: serious-ai-vsl-builder-install
description: Install serious-ai-vsl-builder into the current agent (Claude Code, Codex, Hermes, Openclaw, etc.), and check whether its companion skill serious-ai-video-edit is present.
---

# serious-ai-vsl-builder install

Use this file only for first-time install or reconnect. For daily usage, read `SKILL.md`.

## What you're doing

This skill is pure methodology, no code, no dependencies. It helps a user plan and script a VSL (video sales letter), then hands off actual video cutting to a companion skill, `serious-ai-video-edit`. Installing this skill is just getting `SKILL.md` onto disk and registered; there's no `ffmpeg`, no Python, no API key, nothing to configure.

## Steps

### 1. Get the repo onto this machine

```bash
test -d ~/Developer/serious-ai-vsl-builder || git clone https://github.com/serious-ai/serious-ai-vsl-builder ~/Developer/serious-ai-vsl-builder
cd ~/Developer/serious-ai-vsl-builder
```

If it's already there, `git pull --ff-only` and continue. If you're already reading this file from inside a fully-populated copy (e.g. a `.skill` package the user dropped into their agent's skills folder directly), skip cloning entirely and treat that directory as the install location.

### 2. Register the skill with the current agent

```bash
mkdir -p ~/.claude/skills
ln -sfn ~/Developer/serious-ai-vsl-builder ~/.claude/skills/serious-ai-vsl-builder
```

Substitute the equivalent skills directory for Codex (`~/.codex/skills/`), Hermes, Openclaw, or whichever agent is running. If you can't tell which agent you're in, ask the user once.

### 3. Check for the companion skill, serious-ai-video-edit

This skill produces a beat-map script and shot list; it does not cut video. When the user is ready to actually edit footage, the agent needs `serious-ai-video-edit` installed too. Check now, but don't block this install on it:

```bash
test -d ~/.claude/skills/serious-ai-video-edit && echo "present" || echo "missing"
```

If missing, don't install it automatically, just note it in the hand-off message (step 4) so the user knows it'll be needed later and can say the word when they're ready. It has its own setup flow at `https://github.com/serious-ai/serious-ai-video-edit`.

### 4. Hand off

Tell the user, in one short message:

- The skill is installed and ready, no further setup needed.
- A good first message is something like *"help me script a VSL for [product]"* or *"I want to build a sales video for X."*
- If `serious-ai-video-edit` isn't installed yet, mention that it'll be needed once footage is ready to cut, and that you can set it up then (or now, if they'd rather do both at once).

## Keeping the skill current

`cd ~/Developer/serious-ai-vsl-builder && git pull --ff-only` pulls the latest version. The symlink picks it up automatically.
