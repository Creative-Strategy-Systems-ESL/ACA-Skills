# The AI prompts

Two packs ship with Course 103: a set of analysis and development prompts, and one self-contained
mega-prompt that teaches the framework to an AI before asking it to analyse. Reproduced with
`[BRACKETED]` placeholders intact, because those are the interface.

## Contents

- [Competitor ad reverse engineering](#1-competitor-ad-reverse-engineering) — 2 prompts
- [New creative concept development](#2-new-creative-concept-development) — 2 prompts
- [Performance analysis and iteration](#3-performance-analysis--iteration) — 2 prompts
- [The standalone Building Blocks Analysis mega-prompt](#the-building-blocks-analysis-mega-prompt)
- [Three strategic workflows](#strategic-workflows-for-creative-strategists)

---

## 1. Competitor ad reverse engineering

### Ad Structure Breakdown

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

### Building Block Identification

```
Deconstruct this competitor ad into the specific building blocks framework:

[PASTE AD SCRIPT/DESCRIPTION]

Identify each of these elements:
- Structure Blocks: Which Hook, Body, and CTA approaches?
- Product Blocks: How do they introduce and demonstrate their product?
- Person Blocks: How do they use problem statements, social proof, and storytelling?

For each block identified, rate its effectiveness on a scale of 1-10 and explain why.
```

⚠️ In ACA's pack this second prompt is headed "Audience Pain Point Mining", which does not describe
what it does. Its body is a building-block deconstruction, and it is referred to elsewhere in
ACA's own workflows as the "Building Block Identification" prompt. Named here for what it does.

---

## 2. New creative concept development

### Building Block Mixer

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

### Prompt 6 — Hook Generator

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

---

## 3. Performance analysis & iteration

### Prompt 7 — Block Performance Diagnosis

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

### Prompt 8 — A/B Test Designer

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

---

## The Building Blocks Analysis mega-prompt

A separate one-page asset, designed to be pasted whole into any AI assistant. It teaches the
framework first, then asks for the analysis, which is why it is much longer than the others.

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

---

## Strategic workflows for creative strategists

Three workflows that chain the prompts into a repeatable cycle.

⚠️ In ACA's pack this section is stamped **Course 704: AI Powered Iterations & Creative
Improvement**, not Course 103, though it ships inside the Course 103 prompt pack. Included here
because it is what the pack contains and because it is the practical assembly of these prompts.

### Workflow 1 — Competitor Analysis Cycle

1. **Collect competitor creatives.** Use ad intelligence tools (Facebook Ad Library, TikTok
   Creative Center). Identify top performers by engagement metrics.
2. **Reverse engineer with AI.** Run the Ad Structure Breakdown prompt on each, then the Building
   Block Identification prompt for deeper deconstruction.
3. **Create a competitor block database.** Organise findings in a spreadsheet: hooks by type and
   emotional appeal, body blocks by demonstration style and objection handling, CTAs by urgency
   mechanism and value proposition.
4. **Pattern identification.** Look for commonalities among top performers. Identify gaps or
   approaches competitors are not using.
5. **Concept development.** Use the Building Block Mixer to create concepts that leverage
   successful patterns and fill the gaps.

### Workflow 2 — Performance Diagnosis Cycle

⚠️ ACA titles this "Competitor Analysis Cycle" as well, which appears to be a copy-paste error:
its content is performance diagnosis, not competitor analysis. Retitled here for what it does.

1. **Performance breakdown.** Segment performance data by ad element (hook retention, mid-video
   engagement, CTA clickthrough). Identify drop-off points in the viewer journey.
2. **Block-level diagnosis.** Use the Block Performance Diagnosis prompt. Determine whether issues
   are with the Hook (attention), the Body (desire) or the CTA (action).
3. **Targeted block testing.** Use the A/B Test Designer to create controlled variables. Test one
   block variation at a time to isolate impact.
4. **Performance learning database.** Document which block variations performed best for specific
   audiences (demographics, interests), platforms (Meta, TikTok, YouTube) and objectives
   (awareness, consideration, conversion).
5. **Scale winning block combinations.** Recombine highest performers into new variations.
   Gradually replace underperforming blocks while retaining top performers.

### Workflow 3 — New Campaign Development

1. **Awareness stage mapping.** Determine the audience's awareness level and select block types
   appropriate to it.
2. **Block library audit.** Review existing blocks. Identify gaps needing new development.
3. **Block generation.** Use the Hook Generator for multiple hook options. Create product and
   person blocks aligned to campaign objectives.
4. **Modular ad assembly.** Mix and match blocks into complete concepts.

The three workflows map onto the three states a strategist is usually in: starting from nothing
(3), fixing something live (2), or learning from the market (1).
