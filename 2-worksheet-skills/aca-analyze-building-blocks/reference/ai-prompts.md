# The AI prompts

ACA ships two prompt assets with Course 103. The ones that serve a teardown are here, verbatim,
with the mega-prompt reproduced in full because it is the single most useful one for this job.

The `[BRACKETED]` placeholders are the interface. Fill them; do not rewrite them.

## ⚠️ Every one of these runs on a pasted ad description

`[PASTE AD SCRIPT/DESCRIPTION]` is not decoration. Given an empty bracket, or a brand name where a
description should be, these prompts will produce a fully-formed teardown of an ad that was never
seen, and it will read exactly like one of an ad that was. That is the failure `SKILL.md` is built
around and no prompt here defends against it.

**Paste a real description or do not run the prompt.**

## Which prompt for which job

| You want | Use |
|---|---|
| The full worksheet in one pass | **The mega-prompt.** It teaches the framework then runs all five sections |
| A fast structural read before committing to the sheet | **Ad Structure Breakdown** |
| Just the block inventory with ratings | **Building Block Identification** |
| To diagnose your own underperformer | **Block Performance Diagnosis**, then the sheet |
| To turn a finished teardown into a test | **A/B Test Designer** |
| To build with the formula you found | **Building Block Mixer** · **Hook Generator**, after the sheet |

---

## The Building Blocks Analysis mega-prompt

A separate one-page asset, designed to be pasted whole into any AI assistant. It teaches the
framework first and then asks for the analysis, which is why it is far longer than the others. It
covers Sections 1 through 5 of the worksheet in a single pass.

ACA's usage note:

> Copy this entire prompt and paste it into your AI assistant (like ChatGPT or Claude). Then add
> your ad description at the end where indicated. The prompt first teaches the AI the ad building
> blocks framework, then guides it to help analyze your specific ad.

```
I need your help analyzing an ad using the "Ad Building Blocks Framework" - a modular approach
to understanding creative structure. First, I'll teach you the framework, then ask you to
analyze a specific ad.

THE AD BUILDING BLOCKS FRAMEWORK

Effective ads follow a three-part structure (Hook-Body-CTA) and use modular building blocks
from three categories:

STRUCTURE BLOCKS - these form the backbone of any ad:
1. Hook (0-3 seconds): The attention-grabbing opener that stops the scroll. Effective hooks use
   pattern interrupts, curiosity gaps, bold claims, or relatable problems.
2. Body: The main content that builds desire and addresses objections. This typically includes
   product demonstration, benefits explanation, and credibility elements.
3. CTA (Call to Action): The closing segment that drives specific action, often with urgency or
   special offers.

PRODUCT BLOCKS - these showcase the offering:
1. Product Introduction: How the product is first revealed (direct, problem-then-solution,
   benefit-first, etc.)
2. Demonstration: Showing the product in action (how-to usage, before/after, comparison, etc.)
3. Features/Benefits: Highlighting key selling points (feature→advantage→benefit structure)
4. Buying Experience: Making the purchase process clear (pricing, shipping, guarantees)
5. Unboxing: Creating anticipation and trust through packaging reveals

PERSON BLOCKS - these create emotional connection:
1. Problem Statement: Articulating the pain point (personal story, common frustration, scenario)
2. Failed Alternative: What didn't work before this solution (prior solutions, competing
   products)
3. Desired Result: The transformation promised (emotional, physical, lifestyle improvement)
4. Before & After: Visual proof of change (side-by-side, sequential, timeline)
5. Social Proof: Testimonials and validation (customer reviews, user counts, expert
   endorsements)
6. Storytelling: Narrative that ties everything together (journey, origin story, day-in-life)

ANALYSIS INSTRUCTIONS

Based on this framework, please analyze the ad I'll describe. For your analysis:
1. Identify the Hook-Body-CTA structure with approximate timing
2. List all Product and Person blocks used, with timestamps if possible
3. Evaluate how effectively each block was executed (1-10 scale)
4. Identify which blocks work particularly well together
5. Note any missing blocks that might have strengthened the ad
6. Determine the primary awareness stage targeted (Unaware, Problem Aware, Solution Aware,
   Product Aware, Most Aware)
7. Identify the dominant emotional driver
8. Summarize the core building block sequence that makes this ad work
9. Suggest 2-3 ways the ad could be improved using the building blocks approach

AD FOR ANALYSIS

[DESCRIBE THE AD HERE IN DETAIL. Include the product/service, format (video, image, etc.),
length, what happens in the ad, key messaging, and any other relevant details. For video ads,
try to describe the content chronologically with approximate timestamps. The more detail you
provide, the more thorough the analysis will be.]
```

**Two things it does not ask for**, both of which the worksheet wants and both worth adding when
you use it:

- **The absent blocks, marked as absent.** Instruction 2 asks for the blocks used, so absences
  arrive only via instruction 5's judgement call about what would have helped. Ask for every block
  marked present or absent.
- **What the analysis was based on.** Add a line asking it to flag anything it could not observe
  from the description rather than scoring it anyway.

---

## Ad Structure Breakdown

The fast structural read. Covers Section 1 plus the Section 5 awareness question, and it is the
right first pass when you have a lot of ads and want to know which deserve the full sheet.

```
Analyze this competitor ad and break it down using the Hook-Body-CTA framework:

[PASTE AD SCRIPT/DESCRIPTION]

Please identify:
1. The Hook (first 0-3 seconds): What technique is used to stop the scroll?
2. The Body (middle section): Which building blocks are used (demos, testimonials, etc.)?
3. The CTA (closing section): What action are they driving and how?
4. Which emotional drivers and persuasion principles are being leveraged?
5. What awareness stage does this ad target?
```

---

## Building Block Identification

The block inventory with ratings. Covers Sections 2 and 3.

```
Deconstruct this competitor ad into the specific building blocks framework:

[PASTE AD SCRIPT/DESCRIPTION]

Identify each of these elements:
- Structure Blocks: Which Hook, Body, and CTA approaches?
- Product Blocks: How do they introduce and demonstrate their product?
- Person Blocks: How do they use problem statements, social proof, and storytelling?

For each block identified, rate its effectiveness on a scale of 1-10 and explain why.
```

⚠️ In ACA's pack this prompt is headed **"Audience Pain Point Mining"**, which does not describe
what it does — its body is a building-block deconstruction, and ACA's own workflows refer to it as
the Building Block Identification prompt. Named here for what it does. See `provenance.md`.

Note *"For each block identified"*: like the mega-prompt, this returns the blocks that are present
and says nothing about the ones that are not. Ask for the absences explicitly.

---

## Block Performance Diagnosis

For your own underperformer rather than a competitor's ad. Run the worksheet first: this prompt
asks which block is causing the problem, and that is much easier to answer against a completed
teardown than against the raw ad.

```
My ad for [PRODUCT] is underperforming with a [METRICS e.g., high CPM but low CTR]. Here's the
current ad:

[PASTE CURRENT AD]

Using the building blocks framework, identify:
1. Which blocks might be causing the performance issue?
2. What specific elements within those blocks could be improved?
3. Generate 3 alternative versions of the problematic blocks while keeping high-performing
   elements intact.
```

⭐ **The metric points at the block.** High CPM with low CTR is a hook problem. Good CTR with poor
hold is usually the hook-to-body transition. Good hold with no conversion points at the CTA or the
buying experience block. Say which you are inferring and why, because that inference is the
diagnosis and it should be arguable.

---

## A/B Test Designer

What a finished teardown is for: turning "this block is weak" into something testable. Its
insistence on changing **one** block is the whole discipline of the modular approach.

```
Help me design an A/B test to improve my ad performance using the building blocks approach.

Current ad: [PASTE CURRENT AD]
Current performance: [CURRENT METRICS]
Goal: [SPECIFIC GOAL e.g., improve CTR, reduce CPA]

Based on the modular framework:
1. Which single block should I test changing first? (Hook, specific Body element, or CTA?)
2. Generate 2 alternative versions of this block while keeping everything else the same
3. What specific metrics should I track to determine which version performs better?
4. What is the minimum test duration and audience size needed for statistical significance?
```

⚠️ **Question 4 will produce a confident number.** Sample size and duration depend on your baseline
conversion rate and traffic, which this prompt does not have. Treat whatever comes back as a
prompt to do the calculation, not as the answer.

---

## After the teardown

These two are not part of filling the sheet. They are what the formula in Section 5 is *for*, and
they are here so the artifact travels with the tools that consume it. Run either with the completed
worksheet pasted in as context.

### Building Block Mixer

Takes the formula and builds with it. Its three preset combinations are a starting point; the more
useful version substitutes the formula your teardown actually found.

```
Help me develop new ad concept variations for [PRODUCT] targeting [AUDIENCE] at the
[AWARENESS LEVEL] stage.

Product details: [PRODUCT DESCRIPTION]
Key benefits: [LIST BENEFITS]
Main pain points: [LIST PAIN POINTS]

Generate 3 different ad concepts using different combinations of these building blocks:

Concept 1: Use a [PROBLEM] hook, [DEMONSTRATION] body, and [SCARCITY] CTA
Concept 2: Use a [SOCIAL PROOF] hook, [STORYTELLING] body, and [TRANSFORMATION] CTA
Concept 3: Use a [PATTERN INTERRUPT] hook, [BEFORE & AFTER] body, and [RISK REVERSAL] CTA

For each concept, provide a brief script outline showing how these blocks would flow together.
```

⚠️ The awareness level and pain points come from Section 5 and from research, not from the ad you
tore down. **The competitor's audience is not automatically yours**, and inheriting their awareness
stage without checking is how a teardown turns into a copy.

### Hook Generator

Ten hook variations. Useful when the teardown found the hook was the weak block.

```
Create 10 different hook variations for my [PRODUCT] using different approaches to stop the
scroll:

Product: [PRODUCT DESCRIPTION]
Target audience: [AUDIENCE DESCRIPTION]
Current pain points: [PAIN POINTS]
Key benefit: [MAIN BENEFIT]

Generate hooks using these different approaches:
1. Question-based hook
2. Shocking statistic hook
3. Problem-agitation hook
4. Curiosity gap hook
5. Pattern interrupt hook
6. Identity-based hook
7. Contrarian statement hook
8. "What if..." scenario hook
9. Urgent news-style hook
10. Bold promise hook

Each hook should be 1-2 sentences that could be delivered in the first 3 seconds of a video ad.
```

⚠️ The shocking-statistic and bold-promise hooks will arrive with invented numbers unless you
supplied real ones. Strike them or mark them for verification before they go anywhere.
