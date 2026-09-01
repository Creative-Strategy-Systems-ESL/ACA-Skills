# The twelve AI prompts

> "These prompts will help you analyze the data you extract, identify patterns, and generate
> insights. **Use these prompts after you've pulled the relevant data from your ad platforms.**"

⛔ **Every one of the twelve takes pasted data.** None of them find anything. That is the design, and
it is why this pack is safer than most prompt packs: it cannot invent an account's performance
because it is never asked to.

**The failure mode is the reverse one** — running a prompt on too little data and getting a confident
pattern out of noise. See the checks at the bottom.

## The three categories

### Data Analysis Assistance — prompts 1 to 5

| # | Prompt | What you paste | What it returns |
|---|---|---|---|
| **1** | **Pattern Identification in Top Performers** | Top performers from the last 30 days: brief creative description, key metrics (ROAS, CPA, CTR), format, key message points, target audience | Common visual elements · messaging patterns · format preferences · outliers · initial hypotheses about what is driving performance |
| **2** | **Hook & Hold Rate Analysis** | Creative name/ID, hook rate, hold rate, conversion rate, brief description of the video opening | Patterns in high-performing hooks · the relationship between hook rate and conversion · patterns in strong hold rates · **3 to 5 specific hooks to test** · elements for better retention |
| **3** | **Creative Fatigue Assessment** | How top creatives have performed over time | Typical fatigue patterns · **average effective lifespan** · creatives showing unusual resistance to fatigue · an optimal refresh cadence · tactics to extend lifespan |
| **4** | **Format Performance Comparison** | Performance across creative types | Which formats suit which objectives · an optimal format distribution · underutilised formats showing promise · use cases per format · formats to scale back or eliminate |
| **5** | **Audience Response Analysis** | Audience response differences | Which approaches work per segment · surprising audience affinities · targeted approaches for key segments · segments needing specialised creative · testing priorities |

⭐ **Prompt 2 is the highest-value one in the pack**, because its fourth output (3 to 5 specific hooks
to test) is the only place in the audit where analysis turns directly into something producible.

### Strategic Interpretation — prompts 6 to 10

| # | Prompt | What it returns |
|---|---|---|
| **6** | **Creative Test Plan Generator** | Control and variation descriptions per test · key metrics per test · testing schedule and hypotheses · a timeline and priority order · success criteria |
| **7** | **Creative Brief Development** | Background from audit findings · creative objectives and KPIs · audience definition · key messaging priorities · creative direction and style · asset requirements (formats, quantities) |
| **8** | **Performance Improvement Roadmap** | Specific measurable goals · week-by-week action items · testing schedule and hypotheses · refresh cadence · review milestones. **A 90-day roadmap** |
| **9** | **Competitive Creative Analysis** | Key differences from competitors · advantages not being leveraged · elements worth testing from their approaches · where you have an edge · recommended strategy adjustments |
| **10** | **Creative Element Impact Calculation** | Performance lift or decline per element tested · elements ranked by impact · interaction effects between elements · which elements to standardise · which warrant further testing |

⚠️ **Prompt 9 is the odd one out.** Every other prompt in this pack works on data you exported from
your own account. This one asks about competitors, whose real numbers you do not have. **Its output
is inference about other people's performance**, so treat it as hypothesis generation and route
competitor work to the dedicated competitor analysis rather than trusting this prompt's confidence.

⭐ **Prompt 10 is the one that repays a real testing history.** Element-level lift only exists if
tests were run cleanly enough to attribute it. On an account that has never isolated a variable, it
will produce correlations dressed as impact.

### Data Visualization Requests — prompts 11 to 12

| # | Prompt | What it returns |
|---|---|---|
| **11** | **Creative Performance Visualization** | Designs for effective visualisations of creative performance |
| **12** | **Creative Decision Tree** | A decision tree for creative development: when to use which format, matching approaches to funnel stages, which hooks for which message types, selecting elements by audience segment, when to refresh versus iterate |

⭐ **Prompt 12 produces the most reusable artifact in the pack.** A decision tree outlives the audit
that generated it, and it is the thing to hand a designer or a junior strategist.

---

## Checking what comes back

**1. Sample size.** Ask how many creatives each conclusion rests on. A "pattern" across four ads is
an observation. The prompts will not volunteer this.

**2. Correlation stated as cause.** Prompts 1, 2 and 10 all produce claims about what is "driving"
performance. Nothing in the exported data establishes causation, and top performers are a
survivor-selected sample by definition. **Rewrite "X drives performance" as "X appears in top
performers", unless a clean test produced it.**

**3. Invented benchmarks.** If any output contains an industry average or a "good" threshold, it did
not come from your data and it did not come from this course. Strip it or source it.

**4. Confounded elements.** If UGC ads also happen to be the short ones, "UGC outperforms" and
"short outperforms" are the same finding. Ask which elements co-occur before treating any as
independent.

**5. Hypotheses that are not testable.** Prompt 6 asks for hypotheses. *"More engaging hooks will
improve performance"* is not one. *"Opening on the problem scenario will beat opening on the product
on hook rate"* is.

## What the pack cannot do

- **It cannot pull your data.** Stated by ACA and worth repeating to anyone who expects otherwise
- **It cannot see the creatives.** Everything depends on the descriptions you paste, so thin
  descriptions produce thin analysis regardless of how much data comes with them
- **It cannot validate the North Star metric.** If you paste ROAS and the business runs on
  contribution margin, every output is precisely wrong
