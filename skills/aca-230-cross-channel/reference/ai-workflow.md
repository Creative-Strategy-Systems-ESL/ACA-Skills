# The four-step AI workflow

Carlotta's answer to the question the course sets up:

> "How can I move faster, come up with more creative ideas, and make sure my messaging is always
> relevant — no matter the channel or stage of the funnel? **This is where AI can become your secret
> weapon.**"

Four steps, each with a prompt, reproduced as written. They run in sequence — each takes the
previous step's output as its input, which is what makes it a workflow rather than four prompts.

> "You can save these prompts and reuse them for any campaign, adjusting the details for your brand
> and audience."

## ⚠️ Before running any of them

**Step 1 is the only step that touches reality.** Steps 2, 3 and 4 all build on its output, so if
step 1 is run thin, everything downstream is confident and ungrounded — and it will not look it.

Two specific cautions:

- **Step 1 asks for "five surprising statistics about the product or service category."** A model
  will supply five. ⛔ **Treat every one as unverified until checked** — a fabricated category
  statistic that reaches a client deck is the most likely way this workflow causes real damage.
- **The output of step 2 is a claim about your brand.** Check it is true of the actual product
  before it becomes the anchor for everything else.

---

## Step 1 — Research & Insight Generation

> "Our goal is to uncover what really drives your audience — their frustrations, desires, and unmet
> needs — not just with your brand, but across the whole category. This ensures your messaging is
> rooted in real, relevant insights."

```
Act as a creative strategist.

Identify the main pain points, unmet needs, and emotional drivers that lead potential customers to
brands like [brand X]. Do not focus on pain points about [brand X] itself; instead, focus on the
broader frustrations, desires, or human needs that would motivate someone to seek out a brand in
this category. List key language around benefits, pain points, features, objections, and failed
solutions. Provide five surprising statistics about the product or service category.
```

⭐ **Note the deliberate instruction to look past the brand.** *"Do not focus on pain points about
[brand X] itself"* — the point is category-level human need, which is what a cross-channel message
has to connect to. A brand-level answer produces messaging only existing customers understand.

⚠️ **The five statistics are the risk.** Everything else this prompt returns is a hypothesis you can
test cheaply; a statistic is a claim that will get repeated. Verify or drop them.

---

## Step 2 — Core Message Generation

> "Now it's time to condense those insights into a single, powerful message that sets your brand
> apart and connects emotionally and rationally with your audience. **This core message anchors your
> campaign and ensures consistency.**"

```
Based on the previous research insights, write one clear, compelling core message for [brand X]
that:
- Clearly differentiates the brand from mainstream competitors
- Appeals to both the emotional and rational needs of the target audience
- Uses vivid, memorable language
- Addresses the audience's main pain points and aspirations
- Is concise enough to be used as the foundation for campaign messaging
```

> "With this, you're not just creating a tagline — you're defining the story you'll tell across every
> channel and touchpoint."

⭐ **This is the thing principle 3 says to hold constant.** Everything in step 3 and step 4 is a
restatement of it, so a weak or untrue core message multiplies rather than dilutes.

---

## Step 3 — Funnel Stage Message Adaptation

> "Adapt your core message for each stage of the funnel, so it remains relevant as your audience
> moves from discovery to decision."

```
Take this core message: [insert message].

Rewrite it for each stage of the funnel:
- Awareness: curiosity-driven and emotionally resonant
- Consideration: informative and trust-building
- Conversion: urgent and action-oriented.
```

**Note the register named for each stage** — curiosity, then information, then urgency. That is the
Ffern progression in three words, and it is the concrete version of *"stay consistent but evolve
your story."*

⚠️ **Check the three still say the same thing.** The failure mode is three messages that read as
three different products. If the conversion version could belong to another brand, the core message
was not carried through.

---

## Step 4 — Channel-Specific Creative Tests & Hypotheses

> "The purpose here is to make sure your campaign is not only consistent, but also optimized for how
> people interact on platforms like Meta, TikTok, and Google."

```
Based on the adapted funnel messages, suggest one creative test idea for Meta, TikTok, and Google.
For each, specify the funnel stage (TOFU, MOFU, BOFU), describe the creative concept, define the
target audience, and state the main hypothesis for why it should work on that platform and at that
funnel stage.
```

⭐ **The hypothesis requirement is what makes this a test rather than a list of ideas.** *"State the
main hypothesis for why it should work on that platform and at that funnel stage"* — an idea with no
stated reason cannot teach you anything when it wins or loses.

⚠️ **The output is a starting point for a media conversation, not a media plan.** It has no budget,
no duration, no measurement design. Take the concepts and hypotheses; build the test properly with
whoever owns the buy.

---

## What the workflow is and is not

> "By moving through these steps — research, core messaging, funnel adaptation, and channel-specific
> testing — you can use AI not just to speed up your process, but to create smarter, more effective
> campaigns."

**It is:** a fast route from category insight to a consistent, stage-adapted, platform-specific set
of testable concepts. Genuinely useful, and the sequencing is the value.

**It is not:** research. Step 1 asks a model what it thinks the category's pain points are; that is
a hypothesis generator, not evidence from your customers. Where real customer research exists, paste
it in rather than asking the model to imagine it.

> "Start with these prompts, adapt them to your brand, and watch how much faster and more
> confidently you can move from insight to execution."
