---
name: aca-reverse-engineer-ad-script
description: Takes a video ad script that works for one brand and rewrites it natively for another - Ad Creative Academy's Course 301 artifact. Deconstructs the source into its hook, narrative arc, 5 to 8 story beats, tone and CTA structure, builds a brand brief for the target, then rewrites every line from scratch on the same skeleton, ending with a note on which structural elements were preserved and how they were translated. Use this when someone has a competitor ad or a winning ad from another category and wants their own version, when a script that worked for one brand needs adapting for another, when someone asks how to use a competitor's ad without copying it, or when a swipe-file video needs turning into a usable script. Reach for it whenever there is a specific ad transcript on the table and a specific brand it should be rewritten for.
---

# Reverse Engineering Ad Scripts

**Ad Creative Academy**, Course 301 (Zach Murray). The prompt that turns the course's central idea
into one repeatable operation.

> "This prompt takes a winning video ad from one brand and rewrites it natively for another. Same
> narrative structure, entirely original content."

It is the productised version of the course's own walkthrough, which reverse-engineered
**Outerknown's** longest-running video for **James Perse**. Those two brands are still hardcoded in
the shipped prompt as the worked example.

## What this skill needs from you

**Required, both of them:**

1. **The source ad's full transcript.** Not a description, not a link — the actual words. The whole
   method is structural analysis of a script, so there is nothing to analyse without one.
2. **The target brand**, ideally with its URL. This is who the rewrite is for.

**Optional, and it materially improves the output:**

3. **What you know about the target brand** — positioning, tone, what they would never say. See the
   warning below; this is the input that most changes the quality of the result.
4. The source ad's performance, if known, and why you picked it
5. Where the rewrite will run, and its length target

⛔ **If the transcript is missing, ask for it and stop.** This is the one input the skill cannot work
around. A rewrite built from "it's the one where the founder walks through the warehouse" is a new
ad, not a reverse-engineered one, and it will not carry the structure that made the original work.

⚠️ **If the target brand is one you do not genuinely know, say so before writing step 2**, and see
`reference/verify-and-use.md`. Do not quietly generate a plausible brand brief.

## The three steps

| Step | What happens | Where |
|---|---|---|
| **1. Deconstruct the source** | Hook, narrative arc, 5 to 8 story beats, tone and voice, CTA structure. **Structure only, never content** | `reference/the-prompt.md` |
| **2. Research the target brand** | Positioning, values, tone, customer, visual world, products, what makes them different | `reference/the-prompt.md`, then ⚠️ `reference/verify-and-use.md` |
| **3. Rewrite** | Same beats, same arc, every line original, matched length, scene direction in brackets | `reference/the-prompt.md` |

Then ACA's closing requirement, which is the audit trail:

> "End with a one-paragraph note explaining which structural elements you preserved and how you
> translated them into the new brand's world."

## ⛔ The rule that makes this legal and useful

Step 1 carries ACA's own firewall, and it is the most important line in the prompt:

> "Do NOT analyze the specific content (products, people, locations). Only analyze the structure and
> technique."

**What transfers is the skeleton. What must not transfer is anything on it.** This is the course's
"you're not stealing the price point, you're stealing the structure" turned into an instruction.

If the deconstruction in step 1 names the source's products, spokespeople or locations, the rewrite
will inherit them. **Check step 1's output for source-specific nouns before running step 3.**

## ⚠️ The trap in step 2, and it is the thing to get right

The prompt says *"Using your knowledge of TARGET BRAND, build a brand brief"*, and asks for
positioning, core values, tone of voice, customer profile, visual world, key products, and what
competitors would never say.

**A model will produce all seven confidently for a brand it knows nothing about.** They will be
plausible, internally consistent, and in some cases invented. Every line of the final script is then
built on them.

⛔ **The brand brief is the highest-risk output here, not the script.** A slightly-off script is
fixable. A script built on a fabricated brand position is wrong in a way that reads as fine.

`reference/verify-and-use.md` sets out what to do about it, including how to run this when the brand
is genuinely unknown.

## How to run it

1. **Take the transcript.** Confirm it is the full thing.
2. **Run step 1 and read it before going on.** Check for source-specific nouns.
3. **Run step 2, then verify it** against the brand's actual site and ads. This is the step that
   earns the output.
4. **Run step 3** on the verified brief.
5. **Deliver with the preservation note**, and with the brand brief's unverified items flagged
   inside the document.

## Reference files

| File | Read it when |
|---|---|
| `reference/the-prompt.md` | The prompt in full, ready to fill and run |
| `reference/verify-and-use.md` | ⚠️ **Read before running step 2.** Verifying the brand brief, running it on a brand you do not know, and checking the rewrite |
| `reference/provenance.md` | Citing the source, what dates, and what in here is ACA's versus this skill's |
