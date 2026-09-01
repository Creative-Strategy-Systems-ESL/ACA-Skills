# The AI prompts

Ad Creative Academy ships 20 prompts with Course 102. All 20 are here, reproduced as written, but
**grouped by the worksheet section they feed** rather than by ACA's own categories, so you can find
the one that unblocks the section you are stuck on.

The `[BRACKETED]` placeholders are the interface. Fill them; do not rewrite them.

## ⚠️ Read this before running any of them

**These prompts do not check whether you gave them anything.** Prompt 4 asked to map an emotional
transformation with the product field filled and the audience field guessed will produce a complete,
confident, well-written transformation map built on nothing. It reads exactly like one built on 300
reviews.

So the rule from `SKILL.md` applies harder here, not less:

- A prompt whose bracket says `[INSERT CUSTOMER FEEDBACK]` or `[INSERT AUDIENCE DATA/RESEARCH]`
  **needs real material pasted in.** If you have none, that prompt is not available to you yet.
- A prompt that only needs product and audience descriptions can run on what you know, and its
  output goes into the worksheet flagged as an assumption.
- Whatever comes back is a **first draft with no provenance attached**. Attaching it is your job:
  `GROUNDED IN:` if it came from supplied research, `⚠️ ASSUMPTION, NOT VERIFIED:` if it did not.

ACA says the same thing at the end of the pack, and it is worth taking literally:

> These prompts should be adapted to your specific needs and combined with your strategic judgment
> as a Creative Strategist. **They are tools to enhance your process, not replace your expertise.**

## Which prompt for which section

| Worksheet section | Prompts |
|---|---|
| 1 · Audience awareness | 1 (assess the stage) · 3 (market sophistication) |
| 2 · Emotional drivers | 2 (mine the pain points) · 4 (transformation map) · 6 (Life-Force framing) |
| 3 · Persuasion principles | 7 (apply one principle) · 8 (social proof) · 9 (authority) |
| 4 · Message framing matrix | 15 (before-after-bridge) · 17 (five psychological framings) |
| 5 · Hook development | 5 (10 psychological approaches) · 12 (10 structural approaches) · 19 (per platform) |
| 6 · Sequencing plan | 13 (the 4-touch awareness journey) |
| 7 · Evaluation checklist | 16 (audit finished creative) · 14 (objection handling) |
| 8 · Winning creative formulas | none needed, it is printed reference |
| After the worksheet | 10 · 11 · 18 · 20, for whoever writes the creative |

**Run them in worksheet order.** Prompt 5 will generate hooks whether or not you have settled the
awareness stage, and the hooks will be worse and you will not be able to tell.

---

# Section 1 — Audience awareness

### Prompt 1 — Awareness Stage Assessment

Needs real research pasted in. This is the one that grounds Section 1.

```
Analyze the following target audience for [PRODUCT/SERVICE]. Based on market research data below,
identify which stage of awareness they're in (Unaware, Problem Aware, Solution Aware, Product
Aware, or Most Aware) and explain why:

[INSERT AUDIENCE DATA/RESEARCH]

For each awareness stage, suggest how our messaging should shift to match their current
understanding.
```

Take the *why* it gives you, not just the label. Section 1 asks for the evidence, and "problem
aware" with no reasoning attached is the answer the worksheet explicitly rejects.

### Prompt 3 — Market Sophistication Analysis

Needs competitor ads pasted in. Feeds the mechanism frame in Section 4 as much as Section 1.

```
Analyze the current advertising landscape for [PRODUCT CATEGORY]:

[INSERT COMPETITOR ADS/MESSAGING]

Based on Eugene Schwartz's 5 levels of market sophistication:
1. What level of sophistication does this market demonstrate?
2. What claims/promises are becoming cliché or overused?
3. What new angle or mechanism could we focus on to stand out?
4. Draft 3 potential headlines that would break through the current sophistication level.
```

⚠️ Question 3 will invent a mechanism if you let it. **A mechanism has to be true of the actual
product.** Take the direction, then check it against what the thing really does before it reaches
the worksheet.

---

# Section 2 — Emotional drivers

### Prompt 2 — Audience Pain Point Mining

⭐ **The highest-value prompt in the pack for this worksheet.** It is the one that turns a pile of
reviews into Section 2, and it returns the customer's own language, which is what Section 2 is
asking for.

```
Review these [CUSTOMER REVIEWS/SURVEY RESPONSES/SOCIAL MEDIA COMMENTS] about [PRODUCT CATEGORY]:

[INSERT CUSTOMER FEEDBACK]

Identify:
1. The top 5 emotional pain points expressed
2. The specific language patterns customers use to describe their problems
3. Which of the Life-Force 8 drives these pain points connect to
4. How I should frame my messaging to address these specific emotional triggers
```

Ask it to quote, not paraphrase. Output 2 is only worth having if the phrases come back intact.

### Prompt 4 — Emotional Transformation Mapping

Produces the FROM/TO transformation Section 2 ends on.

```
For [PRODUCT/SERVICE], help me identify the emotional transformation it provides:

Product details: [INSERT PRODUCT INFORMATION]
Target audience: [INSERT AUDIENCE DESCRIPTION]

Create a detailed transformation map showing:
1. The "BEFORE" state (negative emotions, frustrations, pains)
2. The "AFTER" state (positive emotions, benefits, outcomes)
3. Connect each transformation to specific Maslow's needs or Life-Force 8 drives
4. Generate 5 powerful hooks that highlight this transformation journey
```

⚠️ This one runs on descriptions alone, so it is the easiest in the pack to run on nothing. Paste
the output of Prompt 2 into `[INSERT AUDIENCE DESCRIPTION]` rather than describing the audience
from memory, and the map arrives grounded.

Check the BEFORE state is an emotion and not a purchase. "Has not bought yet" is the failure
Section 2 names.

### Prompt 6 — Life-Force 8 Messaging Development

Run after you have picked the drive. Tests whether the drive actually produces copy, which is the
real check on whether you picked the right one.

```
Our product [PRODUCT] addresses the Life-Force drive of [SPECIFIC DRIVE]. Create 5 messaging
frameworks that tap into this fundamental desire:

Product details: [PRODUCT DETAILS]
Target audience: [AUDIENCE DETAILS]

For each framework provide:
1. A headline that triggers this drive
2. Supporting body copy (2-3 sentences)
3. A call-to-action that reinforces the drive
```

---

# Section 3 — Persuasion principles

### Prompt 7 — Strategic Principle Application

Run it once per principle you shortlisted. Output 1 is what fills the "How I'll use it" column, and
output 4 is what stops the principle being used badly.

```
I want to apply the persuasion principle of [PRINCIPLE] to my ad for [PRODUCT].

Product details: [PRODUCT DETAILS]
Target audience: [AUDIENCE DETAILS]
Current messaging: [CURRENT MESSAGING]

Provide:
1. 3 specific ways to incorporate this principle authentically
2. Examples of how this principle could be visualized in creative
3. How to phrase my CTA to reinforce this principle
4. Potential pitfalls to avoid when applying this principle
```

Works for any of the fourteen in `frameworks.md`, not only the ten printed on the worksheet grid.

### Prompt 8 — Social Proof Strategy

⚠️ Needs your real metrics. Social proof with invented numbers is the fastest way to make a
worksheet dangerous, because the number travels into the ad and the ad is checkable.

```
Help me develop a social proof strategy for [PRODUCT/SERVICE]:

Our key metrics: [INSERT RELEVANT METRICS]
Audience: [AUDIENCE DETAILS]

Generate:
1. 5 ways to present our customer numbers/reviews most effectively
2. How to frame testimonials for maximum impact
3. Social proof elements to include in different ad placements
4. Language templates that convert abstract social proof into concrete emotional benefits
```

### Prompt 9 — Authority Building Elements

Same warning: `[INSERT CREDENTIALS/EXPERTISE]` means credentials you actually hold.

```
Create an authority-based messaging strategy for [PRODUCT/SERVICE]:

Our credentials: [INSERT CREDENTIALS/EXPERTISE]
Audience pain points: [INSERT PAIN POINTS]

Provide:
1. How to present our expertise without sounding boastful
2. Ways to connect our authority directly to customer benefits
3. Authority signals to include in different parts of our funnel
4. Trust-building language that establishes credibility quickly
```

---

# Section 4 — Message framing matrix

### Prompt 15 — Before-After-Bridge Frameworks

Feeds the matrix directly: five versions off one transformation is close to the five frames the
section wants, and it is built from Section 2 rather than alongside it.

```
Using the Before-After-Bridge framework, create 5 different messaging structures for [PRODUCT]:

Product details: [PRODUCT DETAILS]
Target audience: [AUDIENCE DETAILS]
Key transformation: [KEY TRANSFORMATION]

For each version:
1. Before: Vividly describe the painful/frustrating "before" state
2. After: Paint an emotionally compelling picture of the "after" state
3. Bridge: Position our product as the path between these states

Each version should focus on a different emotional driver or pain point.
```

### Prompt 17 — Creative Variation Generator

Its five framings are not the worksheet's five frames, but they overlap enough to be useful when
the matrix has three good rows and two empty ones. Its instruction to keep the core benefit
constant is exactly the matrix's own rule.

```
Create 5 variations of this ad concept, each using a different psychological approach:

Original concept: [ORIGINAL CONCEPT]
Product details: [PRODUCT DETAILS]
Target audience: [AUDIENCE DETAILS]

Generate variations using:
1. Fear of loss framing
2. Aspiration/identity framing
3. Proof/credibility framing
4. Curiosity/mystery framing
5. Belonging/tribal framing

Keep the core benefit consistent but change the psychological angle.
```

---

# Section 5 — Hook development

### Prompt 5 — Multi-Angle Hook Generator

The ten **psychological** approaches: what the hook does to the viewer.

```
For our [PRODUCT/SERVICE], generate 10 scroll-stopping hooks using different psychological
approaches:

Product: [PRODUCT DESCRIPTION]
Audience: [AUDIENCE DESCRIPTION]
Awareness level: [AWARENESS STAGE]

Create hooks using:
- Fear of missing out (FOMO)
- Curiosity gap
- Identity reinforcement
- Unexpected statement/statistic
- Problem agitation
- Dream scenario
- Pattern interrupt
- Status elevation
- Loss aversion
- Before/after contrast
```

Note the awareness field. Fill it from Section 1, and the hooks arrive aimed at somebody.

### Prompt 12 — Multiple Hook Variations

The ten **structural** approaches: what shape the sentence takes. Running 5 and 12 and crossing
them is how you get past the two or three hook shapes everyone defaults to.

```
For our upcoming ad about [PRODUCT/FEATURE], generate 10 different hook variations:

Current messaging: [CURRENT MESSAGING]
Target audience: [TARGET AUDIENCE]
Key benefit: [KEY BENEFIT]
Awareness level: [AWARENESS LEVEL]

Create hooks using different approaches:
- Question-based hook
- Statistic-based hook
- Story-based hook
- Identity-based hook
- Pain-point hook
- Curiosity hook
- Counterintuitive statement hook
- Bold promise hook
- Future-pacing hook
- Exclusivity hook
```

⚠️ Statistic-based and bold-promise hooks will arrive with invented numbers unless you supplied
real ones. Strike them or mark them for verification before they leave the worksheet.

### Prompt 19 — Meta/TikTok Ad Hooks Based on Awareness

Section 5 does not ask for platform splits, but if you know where this is running, this produces
better hooks than the generic version.

```
Create platform-specific hooks for [PRODUCT] targeting [AWARENESS LEVEL] audiences:

Product details: [PRODUCT DETAILS]
Key benefit: [KEY BENEFIT]
Target audience: [TARGET AUDIENCE]

Generate 5 scroll-stopping hooks optimized for Meta and 5 for TikTok that:
1. Address the specific awareness level
2. Use platform-appropriate language/style
3. Connect to a core emotional driver
4. Create immediate interest in the first 2-3 seconds
```

---

# Section 6 — Sequencing plan

### Prompt 13 — Awareness Journey Sequencing

Maps straight onto the four rows. The starting and goal awareness levels come from Section 1, which
is what stops the sequence repeating instead of advancing.

```
Help me create a sequenced messaging strategy that moves customers from [STARTING AWARENESS LEVEL]
to [GOAL AWARENESS LEVEL] for [PRODUCT]:

Product details: [PRODUCT DETAILS]
Audience characteristics: [AUDIENCE DETAILS]

Develop a 4-part messaging sequence with:
1. Initial message focus and hook
2. Second touch messaging evolution
3. Third touch messaging evolution
4. Final conversion-focused message

For each stage, explain which psychological elements to emphasize and why.
```

Skip this entirely if the brief is one ad. Section 6 says so and it is right.

---

# Section 7 — Evaluation

### Prompt 16 — Psychology-Based Creative Audit

**This is the Section 7 gate, run by machine.** Point it at finished creative, not at the
worksheet. Its six questions cover most of the ten checklist items.

```
Evaluate this ad creative against consumer psychology best practices:

[INSERT AD COPY/CREATIVE]

Analyze:
1. Which awareness stage does this address? Is it appropriate?
2. Which emotional drivers does it trigger, if any?
3. Which persuasion principles are used effectively or missed?
4. How clear is the transformation being offered?
5. Rate the hook's stopping power (1-10) and suggest improvements
6. Is the CTA psychologically aligned with the emotional appeal?

Provide specific recommendations for psychological enhancement.
```

⚠️ It does not ask the checklist's question 7: *would I be excited to see this if I were the target
customer?* That one is not a machine's to answer. Ask it yourself after this runs.

### Prompt 14 — Objection Handler Development

Serves checklist item 9, *does it address objections the audience might have?* Best run against
objections you found in real research rather than ones you imagined.

```
Based on these common objections to [PRODUCT/SERVICE]:

[LIST OBJECTIONS]

Create persuasive responses that:
1. Acknowledge the concern empathetically
2. Reframe the objection using psychological principles
3. Provide evidence that overcomes the objection
4. Return to the core emotional benefit

Address each objection using at least one persuasion principle from Cialdini's framework.
```

⚠️ Point 3, "provide evidence", is an invitation to fabricate. Evidence you do not have is not
evidence.

---

# After the worksheet

These four are not part of filling it. They are what the person you hand the worksheet to does
next, and they are here so the artifact travels with the tools that use it. Each one is best run
with the filled worksheet pasted in as context.

### Prompt 10 — Awareness-Matched Ad Scripts

```
Create 3 different ad scripts for [PRODUCT], each targeting a different awareness level:

Product details: [PRODUCT DETAILS]
Key benefits: [KEY BENEFITS]
Unique mechanism: [UNIQUE MECHANISM]

Develop 15-second scripts for:
1. Problem Aware audience (focus on problem validation)
2. Solution Aware audience (focus on unique mechanism)
3. Most Aware audience (focus on special offer)

Each script should include a hook, body, and CTA that align with the specific awareness level.
```

### Prompt 11 — Emotional Driver Script Development

```
Write an ad script that leverages the emotional driver of [SPECIFIC EMOTIONAL DRIVER] for
[PRODUCT]:

Product details: [PRODUCT DETAILS]
Target audience: [AUDIENCE DETAILS]
Key message: [KEY MESSAGE]

The script should:
1. Open with a hook that triggers this specific emotion
2. Build emotional intensity in the body
3. Connect the product directly to emotional relief/fulfillment
4. Close with a CTA that reinforces the emotional benefit
```

### Prompt 18 — AI-Enhanced Ad Script Polishing

```
Enhance this ad script by strengthening its psychological impact:

[INSERT DRAFT SCRIPT]

Improve:
1. Make the hook more emotionally compelling and pattern-interrupting
2. Strengthen the connection to core human drives
3. Make the transformation more vivid and concrete
4. Add sensory language that triggers emotional responses
5. Ensure the CTA leverages psychological momentum

Provide the enhanced version and explain the psychological improvements made.
```

### Prompt 20 — Video Script Structure Based on Consumer Psychology

```
Create a video ad script structure for [PRODUCT] that follows optimal psychological sequencing:

Product: [PRODUCT DETAILS]
Audience: [AUDIENCE DETAILS]
Awareness level: [AWARENESS LEVEL]
Key emotional driver: [EMOTIONAL DRIVER]

Develop a 30-second script structure with:
1. Pattern-interrupt opening (first 3 seconds)
2. Problem/pain point agitation (seconds 3-8)
3. Emotional intensification (seconds 8-12)
4. Solution introduction (seconds 12-18)
5. Proof/credibility element (seconds 18-22)
6. Transformation reinforcement (seconds 22-26)
7. Clear CTA with urgency (seconds 26-30)

For each section, note which psychological principle it leverages.
```

---

## ACA's own guidance on sequence

Reproduced because it is the pack's intended order, and it is worth knowing that the regrouping
above is this skill's, not theirs:

> Start with audience analysis prompts to understand your target's awareness level and emotional
> drivers. Use the emotional driver prompts to identify the psychological core of your message.
> Apply persuasion principle prompts to add proven psychological triggers to your creative. Develop
> complete scripts with the ad script development prompts. Plan campaign sequences that move
> customers through awareness stages. Evaluate and enhance existing creative with the audit and
> polishing prompts. Customize for platforms with the specialized application prompts.

> Remember that AI tools work best when you provide specific details about your product, audience,
> and objectives. The more context you give, the more relevant and powerful the outputs will be.
