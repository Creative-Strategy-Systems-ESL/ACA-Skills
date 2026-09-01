# Producing the read-out and the insights log

> "Your job is to diagnose, not just report."

Two artifacts. **Emit them as tables that paste into a sheet**, not as prose about what a read-out
would contain.

⚠️ **Provenance, stated up front because it matters here.** ACA ships no worksheet with this course.
The **insights log's columns are Chloe's**, taken from the four questions she says to ask of every
high-CTR ad and the running doc she says her team kept. **The read-out table's layout is this
skill's**, built from her metrics, her bands and her two-line diagnostic. Say so when you hand it
over; do not present either as an ACA template.

---

## ⛔ Four rules before you fill a cell

1. **Never invent a number.** If it was not supplied, the cell reads `not supplied`. Not a
   plausible-looking estimate, not a category average.
2. **Never derive a metric you were not given the parts for.** Thumbstop needs 3-second views *and*
   impressions. Two of three is nothing.
3. **Every verdict names the band it was judged against, and the band names its advertiser.**
   `0.8% — below Jack Archer's 0.9-1.3% band` is a usable sentence. `0.8% — below benchmark` is not.
4. **The account's own baseline outranks every band in this course.** If prior performance was
   supplied, judge against that first and mention Chloe's bands second.
5. ⛔ **Never state a cause you have not been shown.** The four rules above guard the numbers; this
   one guards the two columns that are prose, and they are the ones that get quoted. *"The landing
   page is failing"* is a diagnosis of a page nobody sent you. **A cause outside the supplied data
   is a hypothesis, and it gets written as one:** *"check whether the landing page carries the same
   promise"*, not `the landing page is the problem`. Chloe's own diagnostics are phrased as
   questions and the table below keeps them that way.

---

## 1. The creative read-out

**One row per ad.** Columns, in order:

```csv
Ad,Format,Hook (first line),Angle,Impressions,3s Views,Thumbstop,Link Clicks,CTR (Link),Clicks,Purchases,CVR,Spend,CPA,CPM,What the numbers say,What to change next
```

⛔ **The last two columns are the deliverable.** A read-out that stops at the numbers is the report
the course tells you not to write.

### Worked example

⚠️ **Illustrative figures, to show the shape.** Replace every one of them with the real account's.

| Ad | Format | Hook (first line) | Angle | Impressions | 3s Views | Thumbstop | Link Clicks | CTR (Link) | CVR | CPA | What the numbers say | What to change next |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
| A1 | UGC video | *"Why do men over 30 waste money on mediocre pants?"* | Persona callout | 240,000 | 108,000 | **45%** | 2,640 | **1.1%** | 3.4% | $38 | Thumbstop very strong (above Jack Archer's 40% mark); CTR inside the 0.9-1.3% band. Both creative-owned metrics healthy | Nothing on the hook. **Scale it**, and reuse the persona callout on two other personas |
| A2 | Static promo | `40% off everything` | Discount | 190,000 | not supplied | not supplied | 4,180 | **2.2%** | 0.9% | $91 | ⚠️ CTR well above the band, CVR the lowest here. Matches Chloe's curiosity-click pattern **and** her note that promo statics inflate CTR | Check whether the landing page carries the same 40% message. If it does, the traffic is unqualified, not misled |
| A3 | Polished video | `Introducing the new collection` | Brand launch | 210,000 | 27,300 | **13%** | 1,050 | **0.5%** | 4.1% | $44 | Thumbstop below the 20% iterate line; CTR at the red-flag edge. **But CVR is the best in the set** | Hook problem, not offer problem. Keep the body and the angle, replace the opener |
| A4 | UGC video | *"I'll never wear jeans again"* | Review pull | 165,000 | 49,500 | **30%** | 1,320 | **0.8%** | 3.6% | $41 | Solid thumbstop, CTR just under the band | Header is doing less than the visual. Test three headers against this same opener |

### How to write the verdict column

**Chloe's own two-line diagnostic is the spine:**

| What you see | What it points at |
|---|---|
| Strong thumbstop **and** strong CTR, poor purchases | *"Fix the landing page or review your offer"* — ⛔ written as **check the landing page and the offer**, unless you were actually shown them |
| Low CTR | *"Test a new concept"* |

**Extended with what she says elsewhere in the course:**

| What you see | Read it as |
|---|---|
| Low thumbstop, healthy CTR among those who stayed | The opener is failing, the rest is not. Replace the first shot, keep the ad |
| High thumbstop, low CTR | Stopped them, gave them no reason to click. The header is the suspect |
| High CTR, low CVR | Curiosity clicks **or** an over-promising hook. ⛔ These look identical in the numbers — read the ad against the landing page to tell them apart |
| Low CTR, high ROAS | ⚠️ Not a failure. *"The few people who did click were actually ready to convert"* |
| Modest thumbstop, strong CVR | Stops fewer people, better qualified. Leave it alone |
| High CTR, high CPC or high CPM | Working creative, expensive delivery. ⚠️ Not a creative problem |
| Everything decaying at once | Fatigue, not quality. *"Sometimes CTR tanks because the audience is tired of seeing the same concept"* |

⛔ **Say when a row is not a creative problem.** Targeting, seasonality, product-market fit and
campaign structure all produce bad numbers, and the course is explicit that they do. A read-out that
attributes every result to creative is wrong in the direction that costs your team credibility.

---

## 2. The CTR insights log

> "At Jack Archer, we maintained a running doc of CTR insights across quarters, and over time we
> started predicting which creative would outperform, just based on hook + angle."

**One row per ad worth learning from**, accumulated over quarters. Not a report — a memory.

```csv
Quarter,Ad,Angle,First line of copy,Was the VO doing the heavy lifting?,UGC or polished,Thumbstop,CTR (Link),CVR,Pattern noted
```

⭐ **Columns 3 to 6 are Chloe's four questions verbatim.** *"When you find a high-CTR ad, don't just
rerun it, study it. What was the angle? What was the first line of copy? Was the voiceover doing the
heavy lifting? Was it a UGC format or more polished?"*

### Worked example

| Quarter | Ad | Angle | First line of copy | VO carrying it? | UGC or polished | Thumbstop | CTR (Link) | CVR | Pattern noted |
|---|---|---|---|---|---|---|---|---|---|
| Q1 | A1 | Persona callout | *"Why do men over 30 waste money on mediocre pants?"* | No, the header carries it | UGC | 45% | 1.1% | 3.4% | Age callout in the header outperformed the same ad without it |
| Q1 | A3 | Brand launch | `Introducing the new collection` | No | Polished | 13% | 0.5% | 4.1% | Launch language does not stop anyone, but converts the few it reaches |
| Q2 | B4 | Review pull | *"I'll never wear jeans again"* | Yes | UGC | 30% | 0.8% | 3.6% | Review-sourced lines hold thumbstop; CTR needs a second line |

⭐ **The log's value is the last column, and it only appears after several quarters.** Fill it even
when the pattern is provisional; a wrong noted pattern gets corrected by the next entry, an unwritten
one is lost.

⚠️ **Log the losers too.** She only says to study high-CTR ads, but a log of winners cannot tell you
what does not work, and *"is this ad even making sense to the viewer?"* is answered by the failures.

---

## Delivering it

1. **Both tables**, as CSV or as markdown that pastes into a sheet
2. **A one-line summary per ad** in the verdict column, never a paragraph
3. ⛔ **A line naming every cell that was estimated or inferred**, and every metric that could not be
   computed because the inputs were not supplied
4. **The band you judged against, with its advertiser named**, stated once at the top rather than
   repeated in every row
5. ⭐ **What to test next**, as specific creative changes: which shot, which header, which variant
   count. `Test a stronger hook` is not an instruction anyone can act on

⚠️ **If you were given numbers with no creative attached, say so and stop at description.** A row of
metrics without the ad it came from can be summarised but not diagnosed, and diagnosing it anyway
means inventing the creative that produced it.
