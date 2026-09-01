# Testing, measurement and attribution

Modules 5 and 6. The half of the course about proving whether anything worked.

---

# Test and learn

> "Test and learn means testing your campaign based on a hypothesis and then learning whether that
> hypothesis is proven true or not."

Digital's advantage over every other medium is that testing is *"relatively easy, fast, and
inexpensive"*, so *"you'd be silly not to test on every single campaign."*

⭐ **It is continuous, not an event.** The clients Ashley sees performing best *"are always in a
constant state of testing and learning. No campaign goes live without something being tested, even
if it's just ads with a different colored background."*

⚠️ **The complacency trap:** *"it's critical to never get too comfortable and think, okay, we found
out exactly what works on Meta, so now let's do that forever."* Algorithms and consumer preference
both move; a fixed formula decays.

## Have a plan, and have it early

Start the testing plan **before the creative is made**, so the creative is built to answer the
question. For established brands, plan at least a quarter ahead, ideally a year — it keeps briefs
on a structured path.

**Write down everything you want to learn, then sequence it so each test builds on the last.** Her
example progression: which ad type drives more awareness → does adding creator content to those ads
help → then formats, placements, copy, visuals.

⛔ **One element per test.** *"If you test multiple factors at once, you won't be able to isolate
what caused the difference or the improvement."* Each test is a stepping stone.

## Meta's testing tools

| Tool | What it does |
|---|---|
| **A/B testing** | Two or more ad variations against each other |
| **Sales testing** | How ads drive sales or conversions |
| **Meta Experiments** | A section of Ads Manager; test across placements, audiences or creative formats |
| **Brand survey test** | Good option for brands testing awareness |
| **Brand lift / sales lift studies** | ⚠️ Require a Meta representative and a much higher budget threshold. Worth it if you have both — *"they help you measure true impact"* |

The **sales lift study** is called out as *"the gold standard for measuring the true impact of
campaigns on sales, but it's not always available."*

## The test setup, and a worked example

Four things define a test:

1. **Campaign objective** — the clear goal
2. **Hypothesis** — what you think will achieve it
3. **Metrics to measure** — how success is tracked
4. **Test parameters** — how long it runs (**typically about four weeks**) and the **holdout group
   size**

**Ashley's example, in full:**

| Field | Value |
|---|---|
| Campaign objective | Increase brand awareness by 5% over previous campaigns |
| Hypothesis | Adding creator content to our ads will drive more brand awareness than previous campaigns |
| Metrics | A three-question brand survey comparing the exposed group to the control |
| Parameters | Four weeks, 5% holdout group |

### ⭐ Reading the result, including the null one

If creator-plus-brand content beat brand alone, you can conclude creator content boosted
performance and keep using and testing it.

If there was little difference, **do not dismiss creator content altogether**:

> "It's possible the specific content didn't resonate or other factors influence results. In that
> case, test different content or adjust another variable."

Then form a new hypothesis and go again. *"Test, learn, iterate and optimize."*

---

# Measurement and attribution

## The honest position, and it is the course's

> "It's very difficult to prove that your campaign was the sole reason for growing awareness or
> selling a product. Most brands are doing other things beyond your campaign."

⭐ **Ashley's Twitter interview story**, which is the module's argument in narrative form. Final
round, needed the job, asked how she would prove to a CMO that Twitter ads drove sales. She could
have shown click-through and engagement and implied the rest.

> "But, I knew that would be a lie. I refuse to lie about attribution I'll lie about the color of my
> hair (I'm a real blond!) because I have my standards! So I gave the honest answer: **“I can’t prove it.”**"
>
> "Unless that ad on Twitter was the only one ever run and it was for a product that could only be
> bought through that ad, I cannot honestly claim that Twitter drove that sale. **However, I can
> certainly make a case that it likely contributed to the sale.**"

She got the job. The lesson to carry: the professional answer is the contribution case, not
manufactured certainty.

## Brand metrics are proxies

For awareness, reach and consideration objectives, *"most digital metrics are proxies."* A strong
view-through rate looks good on paper and does not mean anyone registered your brand.

> "You can't get inside the heads of your audience. Maybe your ad had a cute kitten, and sure,
> people noticed the kitten, but did they notice your product?"

Ashley's name for how budget gets allocated across uploaded ads: **the hunger games of ad spend** —
upload 20, and the system funds whichever seem to be hitting the objective.

⚠️ **Read as a description of how budget flows, not as an instruction to upload 20 near-identical
ads.** Module 8 is explicit that ten ads which are the same idea with tiny changes have not given
the system much more to work with. See `andromeda-update.md`.

## Meta's attribution models

Six, all customisable to the campaign and customer journey:

| Model | Credit goes to |
|---|---|
| **Last click** | 100% to the final interaction |
| **First click** | The first interaction |
| **Linear** | Split equally across all touchpoints |
| **Time decay** | More credit the closer a touchpoint is to conversion |
| **Position based** | First and last get the credit, the middle shares the rest |
| **Data driven** | Machine learning assigns credit by each touchpoint's actual impact |

Ashley notes these get complicated enough that *"you've got a lot of times that you're gonna have
to have a marketing data scientist hanging around"*, and points to Meta's business help centre for
implementation.

### ⛔ Why not just use last click

It is the easy option and many clients want it. The analogy she borrows:

> "Think of last click attribution, like it's going out, you're having 12 beers and then finishing
> the night with a tequila shot. The next morning, you're nursing your mom, the next morning, you're
> nursing a brutal hangover and you think, "Hmm, that tequila did me in." But realistically, it's
> probably the beers that played a bigger part"

Last click blames the tequila and ignores the beers.

## Which metric proves what

### Performance metrics — *"more straightforward and clear cut and sometimes brutal"*

| Metric | What it tells you, and the caveat |
|---|---|
| **Clicks** | Feel good, rarely the point unless traffic is the goal. Meta may find *"click happy"* people who never convert |
| **CPC** — cost per click | Useful against benchmark when traffic is the goal. Meaningless for awareness |
| **CPV** — cost per view | Video campaigns. High CPV → adjust targeting or creative |
| **VTR** — view-through rate | How much of the video is watched. Past that 1.7-second average suggests the creative is resonating, but *"we don't know for a fact that it's the most perfect metric"* |
| **ROAS** — return on ad spend | Revenue per dollar spent. *"A crucial metric for performance"* |
| **Cost per download** | Apps. Too high → revisit targeting or creative |

Ashley's Dutch phrase for click-happy non-buyers: *kijken, kijken, niet kopen* — look, look, don't
buy.

### Brand metrics — *"trickier, but still important"*

Without a brand lift study or survey, these infer brand success:

| Metric | What it tells you, and the caveat |
|---|---|
| **CPM** — cost per thousand impressions | Below benchmark suggests the algorithm finds your ad relevant and well-targeted. ⚠️ Fluctuates seasonally — Q4 is expensive |
| **VTR** | Also a brand-recall signal, especially with brand front-loaded |
| **Engagement** | Reactions, comments, shares, clicks. Some brands use it for affinity — but *"a high engagement rate doesn't always mean you're driving sales or brand growth"* |
| **Reach** | Unique people reached. Critical for brand campaigns, especially CPG. ⭐ **Aim for a frequency of 2 to 3** so the message sticks |

## Getting closer to the truth

On Meta's own attribution: *"it's not all-encompassing."* Consider third-party measurement — Google
Analytics, TripleLift, or multi-touch attribution — to see touchpoints across platforms.

> "Measurement and attribution is an art form and there is no 100% truth. Now be careful with
> proxies and use all the available measurement tools to get as close to the truth of how"
