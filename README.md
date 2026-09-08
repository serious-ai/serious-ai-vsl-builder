# Serious AI VSL Builder

By [Serious AI](https://github.com/serious-ai). Plan and script a VSL (video sales letter) with Claude Code, by conversation, using a Hormozi-derived beat map and value-equation framework.

This skill owns the *narrative strategy* of a sales video: what to say, in what order, and why. It doesn't cut video. For the actual editing, it hands off to its companion skill, [serious-ai-video-edit](https://github.com/serious-ai/serious-ai-video-edit).

## What it does

- **Diagnoses your offer** against Hormozi's value equation (Dream Outcome × Perceived Likelihood ÷ Time Delay × Effort) to find which leg needs the most persuasive work
- **Adapts an eight-beat structure** (callout, problem, credibility, live proof, offer stack, price anchor, guarantee, scarcity/CTA) to your specific offer, not a rigid template
- **Writes a beat-map script**: prompter bullets for most beats, verbatim text for anything that's a commercial promise (guarantees, prices)
- **Produces a shot list**, what to record, in what order, camera vs. voiceover
- **Hands off to `serious-ai-video-edit`** for the actual cut once footage exists

## Setup prompt

Paste into Claude Code, Codex, Hermes, Openclaw, or any agent with shell access:

```text
Set up https://github.com/serious-ai/serious-ai-vsl-builder for me.

Read install.md first to install this repo and register the skill with whichever agent you're running under. It has no dependencies, no API key, nothing to configure, it's pure methodology. Check whether serious-ai-video-edit is also installed and tell me if it isn't, since I'll need it once footage is ready to cut.
```

Then in a session:

> help me script a VSL for [your product]

It'll ask about your offer, diagnose the value equation, adapt the beat structure, and produce a script and shot list before anything gets recorded or cut.

## Manual install

```bash
git clone https://github.com/serious-ai/serious-ai-vsl-builder ~/Developer/serious-ai-vsl-builder
ln -sfn ~/Developer/serious-ai-vsl-builder ~/.claude/skills/serious-ai-vsl-builder
```

No dependencies to install. If you also want the video editor: `https://github.com/serious-ai/serious-ai-video-edit`.

## Why two skills, not one

Scripting a VSL and cutting a video are different jobs. Plenty of people want the editor (`serious-ai-video-edit`) for any kind of video, talking heads, tutorials, travel, interviews, with no interest in a sales-letter structure. And plenty of people scripting a VSL already have an editor. Keeping them separate means each does one thing well, and either can be installed alone.

See [`SKILL.md`](./SKILL.md) for the full framework and process.

## Credits & license

Maintained by [Serious AI](https://github.com/serious-ai). The beat map, value-equation framework, and production rules here came out of building and iterating on a real VSL for an underwriting-software product, distilled into a reusable methodology. MIT licensed (see `LICENSE`).
