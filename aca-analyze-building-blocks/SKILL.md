---
name: aca-analyze-building-blocks
description: Takes one ad apart into its modular building blocks and produces a filled Ad Building Blocks Analysis Worksheet - Ad Creative Academy's Course 103 artifact. Five sections - the Hook-Body-CTA structure with timestamps, the five product blocks, the six person blocks, an overall assessment of what combines well and what is missing, and a reverse-engineering summary ending in the reusable block formula. Use this when someone wants an ad broken down, asks why a competitor's ad works, wants a teardown or reverse-engineering of a specific piece of creative, needs to understand the structure behind an ad that is performing, or wants to extract a repeatable formula from something they have seen. Reach for it whenever there is one specific ad on the table and the job is to take it apart rather than to learn the framework.
---

# Break an ad into its building blocks

Ad Creative Academy's Course 103 artifact, produced for one specific ad. This skill runs the
teardown. It does not teach the framework beyond what is needed to fill each section correctly.

**The output is a structured worksheet, not an essay.** It gets compared against other teardowns,
argued with, and mined for the formula at the end. Produce it as filled sections with headings.

## What this skill needs from you

**Required:**

1. **The ad**, described in enough detail to analyse. What that means is the whole question, so
   there is a section on it below.

**Optional, and it sharpens the analysis:**

2. **Whose ad it is** and what they sell
3. **How it performed**, if known, even roughly ("this one scaled", "this beat our control")
4. **What you are analysing it for** — building a swipe file, diagnosing your own underperformer,
   briefing a competitor response
5. **The other ads from the same advertiser**, which makes the formula far more reliable

### ⛔ The failure this skill exists to avoid

**A teardown of an ad you cannot see reads exactly like a teardown of an ad you can.**

This is worse than a fabricated strategy document, because a teardown is written in the language of
observation. "The hook opens on a close-up of the founder's face at 0:02" is a claim about what is
on screen. Invented, it is indistinguishable from the real thing, and the person reading it has no
way to check without going and watching the ad themselves, which is the work they asked you to do.

So: **what arrives determines what can be filled.** Three situations.

**1. A described ad.** A chronological description, ideally with timestamps, covering what is seen
and what is said. Everything is fillable. This is what the worksheet is built for.

**2. ⚠️ A link, a name, or a reference only.** `Analyse this ad` with a URL. *"Break down that
Ryan Reynolds Mint Mobile one."* `Do the Athletic Greens ad everyone's running.`

**You cannot see it.** Say so plainly and ask for a description. Do not produce a teardown from
what you may know about the brand, the category, or ads of that type, and do not produce one "as an
illustration" — it will be read as analysis.

Ask for what is actually needed, and make it easy:

> I can't watch it from here. Walk me through it start to finish: what's on screen, what's said or
> on-screen text, and roughly when things happen. Even 'first 3 seconds: X, then Y, ends with Z' is
> enough to run the full sheet.

ACA's own prompt asks for exactly this, and its bracket is worth quoting at whoever is pasting:
*describe the ad in detail, chronologically, with approximate timestamps.*

**3. A partial description.** Copy but no visuals, or visuals but no timings, or a summary rather
than a sequence. **Fill what the description supports and mark the rest `NOT OBSERVABLE FROM THE
DESCRIPTION GIVEN`.** Do not leave a field blank, because a blank reads as "block absent" and an
unobserved block is not an absent block. That distinction is the entire content of Section 4's
missing-blocks question.

### ⚠️ Effectiveness ratings are judgement, and one kind of them is invention

The worksheet asks for a 1-10 score on nearly every block. Two separate cautions:

- **With the ad described, a rating is an informed judgement.** Say what it rests on. "7 — the demo
  is clear but it arrives before the problem has landed" is arguable. "7" alone is a number with no
  content.
- **⛔ A rating on something you cannot see is invention wearing a number.** Facial expression,
  tone of voice, pacing, music, whether a delivery feels authentic: these are not derivable from a
  written description of what happens. If the description says "the founder talks to camera about
  why she started the company", you know a Storytelling block is present. You do not know whether
  it works, and scoring it 8 is making that up. Mark it `PRESENT, EXECUTION NOT ASSESSABLE`.

The same rule covers performance claims. **Never infer that a block worked because the ad ran for a
long time or has a lot of views.** If performance data was supplied, use it and say so. If not, the
ratings are craft judgements about the creative, not statements about results.

## How to run it

**Work the sections in order.** Section 5's formula is a compression of everything above it, and
written first it becomes a guess the rest of the sheet then gets bent to fit.

1. **Confirm you can see the ad.** If what arrived is a link or a name, stop and ask. Everything
   below depends on this.
2. **Section 1, structure.** Hook, body, CTA with timestamps. Get the boundaries right first; the
   product and person blocks are then placed inside them.
3. **Sections 2 and 3, the blocks.** Walk all eleven and mark each present or absent. **Absent is a
   finding, not a gap in the analysis** — the blocks an ad declines to use are half of what makes
   it distinctive.
4. **Section 4, the assessment.** Combinations, missing blocks, replication potential, structure,
   key drivers, improvements.
5. **Section 5, the summary.** Awareness stage, dominant emotional driver, and the block formula.

`reference/worksheet.md` has all five sections with every field. `reference/blocks.md` defines all
fourteen blocks with their execution styles and what the absence of each usually means.

## Getting the output right

**The formula in Section 5 is the deliverable.** Everything above it is working. Someone who reads
only the last section should still get the transferable thing:

> `Hook (Question) → Problem → Failed Alternatives → Demonstration → Social Proof → CTA with Scarcity`

The ad itself is not reusable; copying it produces a worse version of someone else's creative. The
sequence is reusable against a different offer and audience, and that is the technique.

**Rate what is there, not what you would have made.** A block that is well executed but wrong for
the ad scores low. A rough, badly lit block that carries the whole emotional arc scores high.

**Section 4's missing-blocks question earns its place.** It is easier to describe what an ad does
than to notice what it declines to do, and the absent block is often the opportunity. Answer it
properly rather than listing every block that is not present.

**One ad at a time.** Timestamps and per-block ratings only mean something against a specific piece
of creative. For a whole competitor library, run the sheet per ad and compare formulas — and say
so, because comparing three formulas from one advertiser reveals more than any single teardown.

## The AI prompts

`reference/ai-prompts.md` carries ACA's Building Blocks Analysis mega-prompt in full, plus the
Course 103 prompts that serve a teardown. Use them to do the work, or run the equivalent directly.

## Reference files

| File | Read it when |
|---|---|
| `reference/worksheet.md` | Producing the artifact. All 5 sections and every field |
| `reference/blocks.md` | Any lookup: the 14 blocks, their execution styles, and what an absence means |
| `reference/ai-prompts.md` | Running the teardown with AI, including ACA's full mega-prompt |
| `reference/provenance.md` | Citing the source, and two labelling errors in ACA's own worksheet |
