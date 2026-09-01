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
**Verifying the brand brief, and checking the rewrite** (below). Do not quietly generate a plausible brand brief.

## The three steps

| Step | What happens | Where |
|---|---|---|
| **1. Deconstruct the source** | Hook, narrative arc, 5 to 8 story beats, tone and voice, CTA structure. **Structure only, never content** | **The prompt** (below) |
| **2. Research the target brand** | Positioning, values, tone, customer, visual world, products, what makes them different | **The prompt** (below), then ⚠️ **Verifying the brand brief, and checking the rewrite** (below) |
| **3. Rewrite** | Same beats, same arc, every line original, matched length, scene direction in brackets | **The prompt** (below) |

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

**Verifying the brand brief, and checking the rewrite** (below) sets out what to do about it, including how to run this when the brand
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
| **The prompt** (below) | The prompt in full, ready to fill and run |
| **Verifying the brand brief, and checking the rewrite** (below) | ⚠️ **Read before running step 2.** Verifying the brand brief, running it on a brand you do not know, and checking the rewrite |
| **Provenance** (below) | Citing the source, what dates, and what in here is ACA's versus this skill's |

---

## Verifying the brand brief, and checking the rewrite

⚠️ **Read this before running step 2.** Everything in this file is this skill's addition. ACA does
not warn about any of it.

### The problem in one paragraph

Step 2 says *"Using your knowledge of TARGET BRAND, build a brand brief"* and asks for seven things:
positioning, core values, tone of voice, target customer, visual and lifestyle world, key products,
and what makes them different. **A model will produce all seven for any brand name it is given**,
including one it has never encountered, one that changed direction last year, and one that does not
exist. The output will be fluent, specific and internally consistent. Then every line of the final
script is derived from it.

⛔ **The script is downstream of the brief, so a wrong brief does not produce an obviously wrong
script. It produces a good script for a brand that isn't the client.** That is much harder to catch
in review, because the failure is invisible in the artifact where the work is judged.

### How reliable each of the seven outputs is

Not equally, and the differences are predictable:

| Output | Reliability | Why |
|---|---|---|
| **Key products or collections** | ⚠️ Lowest | Product lines change constantly. Names, collections and hero SKUs go stale faster than anything else here |
| **Visual and lifestyle world** | ⚠️ Low | Highly inferable from category, which is exactly what makes a confabulation read as plausible |
| **Core values / what they avoid** | ⚠️ Low | Often reconstructed from what a brand of this type *would* say |
| **Tone of voice** | ⚠️ Medium | Usually directionally right for well-known brands, unreliable for small ones |
| **Target customer** | ⚠️ Medium | An inference from the category and price point. Reasonable as a hypothesis |
| **Brand positioning** | ✅ Higher | The most-written-about fact about any brand, so best represented |
| **What a competitor would never say** | 🔍 The tell | See below |

⭐ **Question 7 is the diagnostic.** *"What would a competitor never say that this brand would?"* A
researched brief answers it with something that would be actively wrong from the brand next door. A
fabricated brief answers it with something any brand in the category could claim: "quality
craftsmanship", "we care about our customers", "sustainability". **If the answer fits three
competitors, the brief is generic and the rewrite will be too.**

### What to do

#### If the tool can browse

**Then do.** The prompt's own ROLE line says the writer *"know how to do independent research"*,
which contradicts step 2's *"using your knowledge"*. Resolve it in favour of research.

Check, in this order, because it is cheapest to most expensive:

1. **The brand's own site** — how they describe themselves, current collections, the language on
   product pages
2. **Their recent ads**, in a public ad library — tone in the medium the rewrite is for, which is not
   the same as tone on the website
3. **Their social** — the voice they use when not selling

Then rewrite the brief from what you found and mark anything you could not confirm.

#### If the tool cannot browse, or the brand is genuinely unknown

⛔ **Do not silently produce the brief anyway.** Two honest routes:

**Route A, preferred: ask for the brief.** The person requesting the rewrite usually works on the
brand and can answer all seven in five minutes, better than any research could. **Ask for questions 1,
2, 3 and 7** and infer the rest. That is a far better use of a round trip than a fabricated brief.

**Route B: produce it as a hypothesis, labelled.** If the request is one-shot and has a deadline,
write the brief, mark it clearly, and say what would change if it is wrong:

> ⚠️ **BRAND BRIEF UNVERIFIED.** Built from general knowledge of [BRAND], not from their current site
> or ads. The positioning and customer profile are the load-bearing assumptions; if either is wrong,
> the script's tone and its central claim both change. Check these before production.

**Ask and deliver, rather than ask and wait** — unless the person is clearly still in conversation
with you.

#### Marking it inside the document

⛔ **Put the flag in the brief itself, not only in your covering message.** A script gets pasted into
a deck, forwarded, and produced by someone who never saw the conversation. Mark each unverified item
where it sits:

```
Core values: Slow production, material honesty, repair over replacement
              ⚠️ UNVERIFIED — inferred from category, not confirmed on their site
```

That is the only place the caveat still exists when the script reaches the person spending money on
it.

---

### Checking the rewrite

Five checks, in the order they are worth running.

**1. Source-noun sweep.** Search the finished script for every proper noun, place and product from
the source transcript. There should be zero hits. This catches the most common failure, which is a
beat that carried the source's content through step 1.

**2. The lift test.** Put the source and the rewrite side by side, beat for beat. If any line is the
source's sentence with the nouns swapped, it is a lift, not a rewrite. Rewrite that beat from the
*structure* rather than from the source's line.

**3. The question-7 test on the output.** Would this script be wrong coming from the target's nearest
competitor? If it would work equally well for either, the brand brief did not do its job and the
script is category wallpaper.

**4. Length.** ACA asks for approximate parity with the source. Check it, because the original's
length was set by a media slot and drifting 40% longer means it no longer fits what it was modelled
on.

**5. The closing note.** It must name **structural** elements. If the note says "I kept the warm,
authentic feel", that is tone, not structure, and it suggests the deconstruction in step 1 was thin.
A good note reads like *"preserved the five-beat problem-to-proof arc and the cold open on an
unresolved question; translated the factory-access beat into a studio-access beat."*

### When this is the wrong tool

**The source has no script.** A montage with music and three words of supers has no narrative arc to
extract. There is nothing here to reverse-engineer.

**You want several concepts rather than one adaptation.** This produces one script from one source.
For angle variety across an offer, that is a different job.

**The source is not actually working.** The whole method assumes the source ad earned its structure.
Nothing here validates that assumption, so an admired-but-unproven ad transfers its structure just as
willingly as a winner does.

⚠️ **The course's own selection rule is admiration, not performance** — *"pick three ads you
genuinely think are great"*. That is fine for training the eye and weaker as a basis for spending
production money. If run length or performance data is available for the source, use it.

## The prompt

Reproduced as ACA wrote it. Three placeholders to fill: **SOURCE BRAND**, **TARGET BRAND**, and the
**source transcript**.

⚠️ **The shipped prompt has ACA's worked example hardcoded** into the two brand lines: Outer Known as
source, James Perse as target. Those are the same pair the course walkthrough uses. **Replace both**
— it is easy to fill in the transcript and leave someone else's brands sitting above it.

---

```
ROLE
You are an expert brand strategist and advertising copywriter who
specializes in adapting video ad scripts from one brand's voice to
another. You understand how to extract narrative structure and
storytelling technique without copying content — and you know how to do
independent research to make the rewrite feel native to a new brand.

SOURCE BRAND: [NAME] [URL]
TARGET BRAND: [NAME] [URL]

---

TASK
I'm giving you a source video ad transcript from SOURCE BRAND. Your job is
to:
1. Analyze the structure and storytelling of the source transcript
2. Research TARGET BRAND independently to understand their brand voice,
aesthetic, values, customer profile, and product positioning
3. Rewrite the script entirely for TARGET BRAND — same narrative
architecture, completely original content

---

SOURCE TRANSCRIPT
[PASTE FULL TRANSCRIPT HERE]

---

STEP 1 — DECONSTRUCT THE SOURCE
Before writing anything, analyze the source transcript and output:
- Hook: What is the opening technique? (emotion, question, tension, visual
metaphor, etc.)
- Narrative arc: What is the emotional or informational journey the viewer
goes on?
- Story beats: List each beat of the script in sequence (5–8 beats max)
- Tone and voice: How does the brand speak? (aspirational, grounded,
playful, premium, etc.)
- CTA structure: How does the video close and drive action?

Do NOT analyze the specific content (products, people, locations). Only
analyze the structure and technique.

---

STEP 2 — RESEARCH THE TARGET BRAND
Using your knowledge of TARGET BRAND, build a brand brief with:
- Brand positioning: How do they position themselves in the market?
- Core values: What do they stand for? What do they actively avoid?
- Tone of voice: How do they speak in ads, on their website, on social?
- Target customer: Who is this person? What do they care about?
- Visual and lifestyle world: What aesthetics, settings, and cultural
references define this brand?
- Key products or collections: What would naturally be featured in a brand
video?
- What makes them different: What would a competitor never say that this
brand would?

---

STEP 3 — REWRITE THE SCRIPT
Using the narrative structure from Step 1 and the brand brief from Step 2,
write a complete video ad script for TARGET BRAND.

Rules for the rewrite:
- Follow the same story beats and emotional arc — do not invent a new
structure
- Every line of copy must be original — no borrowed phrases, descriptions,
or imagery from the source
- The script must feel like it was written natively for TARGET BRAND —
someone who doesn't know the source video should never be able to tell it
was inspired by another brand
- Match the approximate length and pacing of the source transcript
- Include brief scene direction in [brackets] if it helps communicate the
visual intent

End with a one-paragraph note explaining which structural elements you
preserved and how you translated them into the new brand's world.
```

---

### What each step is actually doing

#### Step 1: Deconstruct the source

Five outputs, and one prohibition.

| Output | What good looks like |
|---|---|
| **Hook** | The *technique*, not the line. "Opens on an unresolved question about the viewer's own habit", not "opens with 'ever wonder why...'" |
| **Narrative arc** | The emotional or informational journey, start to end state |
| **Story beats** | 5 to 8, in sequence, each one a move rather than a sentence |
| **Tone and voice** | Aspirational, grounded, playful, premium, and so on |
| **CTA structure** | How it closes and what action it drives |

> "Do NOT analyze the specific content (products, people, locations). Only analyze the structure and
> technique."

⛔ **This prohibition is the whole firewall.** A beat written as *"the founder shows the Portuguese
factory where the shirts are cut"* has smuggled the source's content into the skeleton, and step 3
will dress it up rather than replace it. The same beat written as *"proof by access: the viewer is
shown a part of the operation customers never see"* transfers cleanly to any brand.

**Check before continuing:** read the beats back and count the proper nouns. There should be none.

⚠️ **"5 to 8 beats max" is a real constraint, not a suggestion.** A 12-beat deconstruction is a
transcription, and it will produce a rewrite that tracks the source line by line, which is exactly
the outcome the originality rule forbids. If a script genuinely will not compress below 8, that is
worth saying: it usually means the source is two ads stitched together.

#### Step 2: Research the target brand

Seven outputs. ⚠️ **Read **Verifying the brand brief, and checking the rewrite** (below) before running this step.** It is the step
that decides whether the output is worth anything.

The seventh is the sharpest and the most useful:

> "What makes them different: What would a competitor never say that this brand would?"

⭐ **That question is a good test of whether the brief is real.** A fabricated brand brief answers it
with something any brand in the category could say. A real one produces a line that would be
actively wrong coming from the competitor next door. **If the answer to question 7 would suit three
brands, the brief has not been researched.**

#### Step 3: Rewrite

Five rules. Four are craft; one is the point.

| Rule | Note |
|---|---|
| Follow the same beats and arc, do not invent a new structure | This is what makes it a reverse-engineering rather than a new brief |
| **Every line original, no borrowed phrases, descriptions or imagery** | ⛔ The rule that matters |
| Feel native to the target brand | |
| Match the approximate length and pacing | Length is a proxy for the media slot the original was cut for |
| Scene direction in [brackets] where useful | |

⚠️ **One rule is worded as concealment and should not be read that way.** ACA writes: *"someone who
doesn't know the source video should never be able to tell it was inspired by another brand."*

**Undetectable is not the same as original.** A script can pass that test while still being a
find-and-replace of the source. The rule immediately above it — every line original, nothing
borrowed — is the one that does the work, and it is the one to check against. If the only argument
for the rewrite is that nobody would notice, it has failed.

**The closing note is not optional.** *"Which structural elements you preserved and how you
translated them"* is the audit trail: it is what lets a reviewer see the borrowing was structural,
and it is the first thing to produce if anyone ever asks.

## Provenance

### Source

**Ad Creative Academy** — *AI Prompt for Reverse Engineering Ad Scripts*, shipped with **Course 301:
Reverse Engineering Winning Ads: The Creative Research System**, taught by **Zach Murray**, founder
of **Foreplay**.

Five pages: a one-page usage guide, the prompt itself across two pages, and ACA's back matter.

⭐ **It is the only tracked download attached to Course 301.** ACA's asset list runs to 46 rows
covering 45 distinct titles, and this course carries exactly one of them.

### ⚠️ The PDF stamps a different course number than the curriculum does

The asset's own footer reads *"Course 302: Reverse Engineering Winning Ads"*. ACA's shipping
curriculum numbers this course **301**, and 302 is Mirella Crespi's Research for Creative Strategy.

**This is not a filing error.** ACA renumbered the programme for launch, and their worksheet PDFs
were stamped before that. The titles agree in both numbering schemes; only the numbers moved. This
skill uses **301**, the shipping number.

⚠️ **Worth knowing because anyone opening the PDF will read 302 on every page.** If someone cites the
document's own stamp, they are not wrong about what it says.

### ⭐ It is the course walkthrough, productised

The prompt ships with **Outer Known** as source brand and **James Perse** as target, hardcoded into
the two brand lines. Those are the same two brands module 2 of the course uses: Outerknown's
longest-running video, an employee store tour, analysed as the "home run" example, and James Perse
as the brand being remixed for.

So the example is not arbitrary, and reading the course's module 2 alongside this shows the intended
use. **But both names must be replaced before running it**, and the transcript placeholder is the
more obvious of the three things to fill.

⚠️ ACA writes the source brand as *"Outer Known"*; the brand styles itself **Outerknown**.

### What is reproduced and what is this skill's

**Reproduced as written:** the prompt in full, including the ROLE block, the three-step structure,
all five step-1 outputs, all seven step-2 outputs, all five step-3 rules and the closing-note
requirement. ACA's usage guide is carried as its own summary of what each step does.

**This skill's, drawn from the material rather than stated by it:**

- ⛔ **The entire verification discipline in `verify-and-use.md`.** ACA presents step 2 as a solved
  problem: *"the AI handles the rest"*. It is the step most likely to produce confident fiction, and
  ACA does not warn about it anywhere. The reliability ranking of the seven outputs, the two routes
  when the brand is unknown, and the instruction to mark unverified items inside the document are all
  this skill's.
- **Reading question 7 as a diagnostic.** *"What would a competitor never say?"* is presented by ACA
  as one output among seven. It doubles as the fastest test of whether the brief was researched or
  generated, because a fabricated brief cannot answer it distinctively.
- ⛔ **The reframing of one step-3 rule.** ACA writes that *"someone who doesn't know the source video
  should never be able to tell"*. That is a concealment test, and a find-and-replace can pass it.
  This skill says plainly that undetectable is not the same as original and points at the
  every-line-original rule as the one that governs.
- **The emphasis on step 1's prohibition as a firewall**, the proper-noun count as the check on it,
  and the worked contrast between a beat that smuggles content and one that does not.
- **The reading of "5 to 8 beats max" as a real constraint**, and the note that a longer
  deconstruction produces a line-by-line tracking of the source.
- **The five output checks**, including the lift test and the note that a closing note about tone
  rather than structure signals a thin step 1.
- **The three cases where this is the wrong tool**, and the caution that the course's selection rule
  is admiration rather than performance.
- The point that the prompt's ROLE line (*"you know how to do independent research"*) contradicts
  step 2's *"using your knowledge"*, and that the contradiction should be resolved in favour of
  research.

### ⚠️ How old this material is

ACA stamps no date on the asset. It was received into this library in **2026-W33**, which is a "no
later than" and not a publication date.

**What dates here is thin, which is a point in this asset's favour.** The prompt is method rather
than platform mechanics, and nothing in it depends on a product, a platform behaviour or a metric.

⛔ **What does not age well is the output, every single time.** Step 2's brand brief is generated at
run time from whatever the model knows, so its accuracy is a property of the run and not of ACA's
document. Product lines and collections in particular go stale fastest. This is the reason the
verification step exists.

### Deliberate overlap with `aca-301-reverse-engineering-ads`

Both skills relate to Course 301, on purpose, and each must run with nothing else installed.

The split is by job:

- **`aca-301-reverse-engineering-ads`** teaches the course: why nothing is original, the
  six-dimension pattern framework, the five-step competitor audit, and building a team creative
  engine. It produces a Pattern Map and Remix across **three** ads and names this prompt rather than
  reproducing it.
- **This skill** runs one operation on **one** source script for one target brand, and does not
  teach the research method.

**Route on the input.** A full transcript plus a named target brand is this skill. Three admired ads
and a brand that needs ideas is the course skill.

### Credit

The prompt and its usage guide are Ad Creative Academy's work, by Zach Murray. This skill organises
that material so it can be run safely; it does not originate it.
