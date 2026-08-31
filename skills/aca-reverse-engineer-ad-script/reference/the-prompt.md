# The prompt

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

## What each step is actually doing

### Step 1: Deconstruct the source

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

### Step 2: Research the target brand

Seven outputs. ⚠️ **Read `reference/verify-and-use.md` before running this step.** It is the step
that decides whether the output is worth anything.

The seventh is the sharpest and the most useful:

> "What makes them different: What would a competitor never say that this brand would?"

⭐ **That question is a good test of whether the brief is real.** A fabricated brand brief answers it
with something any brand in the category could say. A real one produces a line that would be
actively wrong coming from the competitor next door. **If the answer to question 7 would suit three
brands, the brief has not been researched.**

### Step 3: Rewrite

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
