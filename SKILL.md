---
name: serious-ai-vsl-builder
description: Plan, script, and structure a VSL (video sales letter) using a Hormozi-derived beat map and value-equation framework. Use when someone wants to plan, script, storyboard, or structure a sales/demo video, not just edit raw footage they already have. Produces a beat-map script and shot list, then hands off actual cutting to the serious-ai-video-edit skill.
---

# Serious AI VSL Builder

By [Serious AI](https://github.com/serious-ai). This skill owns the narrative strategy of a VSL, what to say, in what order, and why. It does not cut video. For the mechanical editing (transcription, cuts, grading, subtitles, overlays), it hands off to the [serious-ai-video-edit](https://github.com/serious-ai/serious-ai-video-edit) skill.

## Principle

1. **Structure is a starting point, not a template to fill in blindly.** The eight-beat map below is proven, but every offer is different. Ask what the offer actually is, then adapt the structure, don't force an offer into beats that don't fit it.
2. **Proof beats prove of the outcome, they don't claim it.** The strongest VSLs let the viewer watch something happen (a live demo, a real result, a before/after) rather than being told to trust a claim.
3. **The value equation is a diagnostic, not a checklist.** Use it to find which leg of Dream Outcome, Perceived Likelihood, Time Delay, and Effort & Sacrifice is weakest for this specific offer, then build the beat that fixes it. Don't mechanically tick all four every time.
4. **Ask → confirm → script → hand off → iterate.** Never start cutting footage until the beat-map script is confirmed. Never touch the edit itself, that's `serious-ai-video-edit`'s job.
5. **Honesty over polish.** Real, unrehearsed proof (including moments that don't flatter the product) is stronger footage than a clean, scripted win. Don't sand off an honest rough edge, script around it.

## The eight-beat structure (Hormozi-derived)

The underlying arc, adapted from Alex Hormozi's `$100M Offers`: **callout → problem (avoided loss, not a speed/convenience pitch) → credibility in seconds → live proof → offer stack via the value equation → price anchored to the loss it prevents → guarantee → honest scarcity → single CTA.** Objections get answered inline, right where they'd naturally come up, never bolted on as a separate FAQ section.

1. **COLD OPEN.** The callout and the credibility, together, fast. Open on the specific fear or loss your exact buyer already has, before any self-introduction ("the deal that hurts you is not the one you pass on, it's the one you talk yourself into"). Land credibility as numbers, not a bio, inside the first 30 seconds. Close by naming the demonstration to come, so the viewer knows what they're about to watch and why.
2. **THE PROBLEM.** Avoided-loss framing, not a speed or convenience pitch. Name concrete, specific failure modes your buyer will recognize instantly, not abstract pain points. Close by positioning your offer as the codification of hard-won lessons ("every mistake became a rule"), not a generic tool.
3. **WHY LISTEN TO ME.** One short beat, deliberately brief and still. Carries your core credibility claim, and doubles as a pre-emptive answer to the biggest objection you'll face later (skin in the game, track record, whatever makes you the right messenger).
4. **THE DEMO (live proof).** The spine of the video. This is where Perceived Likelihood gets built, not asserted. Show the outcome actually happening on real material, not a rehearsed walkthrough. Narrate a handful of live moments rather than continuously; let silence and screen content do some of the work. End in a **reveal**: state the result honestly, including anywhere it didn't go perfectly. An honest gap is stronger proof than a clean win, don't hide it.
5. **THE SIMPLE PART.** The dream-outcome beat. State the dream as the *absence* of work, not a bigger number: what does the buyer no longer have to do? This is where Effort & Sacrifice and Time Delay both get crushed, ideally in one breath, because the demo already proved competence and the beat's only job is to prove *ease*.
6. **THE OFFER.** A stacked offer, each deliverable named and priced individually rather than one bundled price drop (the standard grand-slam-offer stacking technique). Simple numbered list, no jargon register. If you have a structural differentiator competitors can't claim, name it here explicitly.
7. **PRICE ANCHOR + GUARANTEE.** The single most important delivery in the video, slow down here. Anchor price to the size of the loss it prevents, not to feature value or competitor pricing. State every guarantee verbatim and exactly, this is a commercial promise, not a place for fresh phrasing. Answer the "why would you sell me this" objection inline, right after the guarantee.
8. **SCARCITY + CTA.** Real scarcity tied to an actual capacity constraint (you personally do the onboarding, you only take N clients a month, whatever is genuinely true), never a manufactured countdown. One single call to action, nothing else competing for attention on screen.

Reorder, merge, or drop beats when the offer calls for it. A cheap, low-commitment offer might not need a separate guarantee beat; a technical audience might want the demo doubled in length and the simple-part beat cut short. Ask, don't assume.

## The value equation

Hormozi's formula: **Value = (Dream Outcome × Perceived Likelihood of Achievement) ÷ (Time Delay × Effort & Sacrifice).** Use it as a diagnostic during the strategy conversation, not a scoring rubric to run mechanically:

- **Dream Outcome.** What does the buyer actually want, stated as their outcome, not your feature? Weak dream-outcome framing shows up as a features list instead of a result.
- **Perceived Likelihood of Achievement.** Can the buyer believe this will work for *them*, specifically? This is usually the weakest leg for anything unproven or technical, which is exactly why THE DEMO exists: proof beats claims here every time.
- **Time Delay.** How long until the buyer sees the outcome? If your offer is slow, either shorten the beat that discusses it or reframe around the first visible win rather than the final outcome.
- **Effort & Sacrifice.** What does the buyer have to do or give up? THE SIMPLE PART beat exists specifically to compress this to near-zero in the viewer's mind.

Ask which leg is weakest for THIS offer before scripting. A well-known brand with an unproven-feeling product needs more Perceived Likelihood work (a longer, more convincing demo). A trusted-but-slow provider needs more Time Delay reframing. Don't spend equal beats on all four; spend the most on whichever is weakest.

## Proof and offer rules

- **Verbatim only where precision is a commercial promise.** Guarantees, prices, and anything the buyer could reasonably hold you to must be said exactly the same way every time, scripted or read verbatim. Everything else should be re-phrased fresh each take, prompter bullets, not prose (see Production template below), a memorized script sounds memorized.
- **Ranges over single point figures, when your business allows it.** A stated range reads as considered and honest; a single exact number invites nitpicking and sounds more like a rehearsed pitch.
- **Speed through low-value proof material, never cut it out.** If a section is genuinely rich (a report walkthrough, a comp set, supporting detail) but too slow at normal speed, ramp the speed up so the viewer still sees it scroll by, don't remove it. This is a `serious-ai-video-edit` Hard Rule now (dropping footage instead of speeding through it is an anti-pattern there) precisely because of what was learned building this skill's own worked example.
- **The punch-line beat gets zero manipulation.** Whichever moment is the single strongest proof point in the whole video (the reveal, the result, the "aha") should run at full continuous speed, no cuts, no ramps. Everything else can be trimmed or sped through; this beat cannot.
- **Never expose the proprietary mechanism behind your proof.** Show the input and the result. Don't screen-share your actual pricing logic, scoring internals, or methodology in a way a competitor could copy, only the observable inputs and outputs need to be on screen.
- **Verify every claimed "catch" or proof point against the actual underlying record before scripting it.** If the proof is "the demo caught something a human missed" (or vice versa), confirm it against the real artifact, not memory, before it goes in the script. Prefer proof points that are independently checkable (a public record, a timestamp, a deed) over restated claims.

## Production template

- **Prompter carries beats and bullets, not full prose**, except for the verbatim whitelist above (guarantees, prices, the closing line). Reading full prose sounds read; working from bullets sounds spoken.
- **Minimum-face path.** Figure out which beats genuinely need the presenter's face (credibility beats, the price/guarantee, the CTA) versus which can run as voiceover over screen capture or B-roll with zero eyeline cost. Four beats on camera is often enough for an eight-beat structure.
- **Record voiceover first, in one sitting**, before any face shooting. It's fast, forgiving to redo, and tells you the real runtime before a single light gets set up.
- **Record voiceover per-beat, in separate files**, not one long continuous take. Cheaper to re-record a single flubbed beat, and it avoids hunting for boundaries in post.
- **Leave a few seconds of room-tone silence before each take** so joins between beats can be smoothed later without an audible edit.

## The process

1. **Understand the offer.** Ask what's being sold, to whom, at what price, and what makes it credible. Don't assume any of Beat 1-8's specifics, this is a fresh conversation every time.
2. **Diagnose the value equation.** Which leg (Dream Outcome, Perceived Likelihood, Time Delay, Effort & Sacrifice) is weakest for this specific offer and audience? That answer shapes where the script spends the most time.
3. **Adapt the beat map.** Walk through the eight beats, reorder/merge/drop as the offer calls for, and draft what each beat needs to say and (if applicable) show. Confirm the beat map with the user before writing full script language.
4. **Write the script**, bullets for prompter beats, verbatim text for the promise-bound beats (guarantees, prices, closing line). Note which beats are FACE and which are VO.
5. **Produce a shot list**: what footage or recording is needed for each beat (live demo capture, talking-head takes, screen recording, B-roll), and in what order to record it (voiceover first, per the production template).
6. **Hand off to `serious-ai-video-edit`.** Once footage exists, this skill's job is done, everything downstream (transcription, cutting, pacing, grading, subtitles, overlays, self-eval) is that skill's responsibility. If it isn't installed in this environment yet, tell the user and offer to set it up (`https://github.com/serious-ai/serious-ai-video-edit`, its own setup prompt is in its README). Then either invoke it directly if your agent supports cross-skill invocation, or read its `SKILL.md` and follow its process yourself.
7. **Iterate on the cut, not the strategy, unless something in the footage reveals the strategy was wrong.** Most iteration from here on is editorial (pacing, cut points, grade), handled by `serious-ai-video-edit`. Only re-open the beat map if the actual footage surfaces a problem the script didn't anticipate.

## Worked example: an underwriting-software VSL

This structure shipped on a real VSL for an AI underwriting tool, publicly live at `seriousland.capital/install`. How the beats mapped for that offer:

- **Cold open:** opened on loss aversion ("the deal that hurts you is not the one you pass on, it's the one you talk yourself into"), credibility as funded-deal numbers inside the first 30 seconds, named the demonstration to come (underwriting a real, previously-unseen parcel two ways at once).
- **The problem:** named specific real underwriting mistakes (a smuggled comp, a misread deed, an ignored stale listing) rather than a generic "underwriting is slow" pitch.
- **Why listen to me:** one line tying personal capital risk to the claim ("when my number is wrong, it's my capital at title that eats it").
- **The demo:** a manual expert read and the software's run, side by side, on the same real parcel, at the same time, unrehearsed. The reveal stated both results honestly, including admitting the software didn't win the stopwatch race.
- **The simple part:** the entire user manual compressed to "an APN, a county, a state, type them, tell it to go, and walk away," explicitly the dream-outcome-as-absence-of-effort beat.
- **The offer:** three deliverables stacked individually (install, standing access, funding-partner access), each priced and scoped on its own.
- **Price anchor + guarantee:** price anchored to the cost of one bad comp, two guarantees stated verbatim, the "why would you sell me this" objection answered inline (the tool isn't the business, funding deals is).
- **Scarcity + CTA:** scarcity tied to the presenter doing every onboarding personally ("that's not a countdown timer, it's a calendar"), single CTA.

Runtime target was 7-9 minutes on paper; the honest, fully-proof-complete cut ran closer to 20 minutes once "speed up, don't cut" replaced early drafts that had removed footage to hit a shorter number. That tradeoff (completeness of proof vs. runtime) is worth surfacing explicitly with any user building a proof-heavy VSL: longer is fine if the proof is the product, but for cold-traffic content it's a real cost worth naming.

## Anti-patterns

- **Feature-dumping instead of loss-framing the problem beat.** A list of capabilities is weaker than a specific, recognizable failure mode.
- **Manufactured urgency.** A countdown timer with no real constraint behind it reads as fake and undercuts everything else in the video.
- **Scripting around an honest rough edge instead of keeping it.** An unrehearsed discrepancy or an admitted shortfall is stronger proof than a clean, edited-to-perfection result.
- **A bolted-on FAQ or objections section.** Answer objections inline, at the beat where they'd naturally arise, not in a separate section at the end.
- **One bundled price instead of a stacked offer.** Name and price each deliverable individually.
- **Treating the value equation as a scoring checklist to fill in evenly.** Diagnose the weakest leg for this specific offer and spend the script's effort there, not equally across all four.
- **Starting to cut footage before the beat-map script is confirmed.** Strategy first, execution second, exactly as `serious-ai-video-edit` requires strategy confirmation before touching a cut.
- **This skill trying to do its own video editing.** If you're reaching for ffmpeg, a transcript, or a timeline, that's `serious-ai-video-edit`'s job, hand off instead of duplicating it.
