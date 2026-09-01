---
name: aca-track-creative-tests
description: Fills Ad Creative Academy's Creative Testing Tracker for a real test or a real backlog, in the workbook's own nineteen columns under its two banner groups. Captures what was tested, the hypothesis, the live date, the result and the learning, alongside ROAS, CPA, CVR, CTR, hook rate, hold rate and average watch time. Flags the three fields the course says to record that the shipped sheet has no column for - KPI, channel and priority - and the metric grouping that contradicts Course 402. Use this when tests need logging before they run, when results have come back and nobody wrote down what they meant, when a team keeps re-testing the same thing, or when someone asks for a creative testing tracker. Requires the tests - it cannot log an experiment it has not been told about.
---

# Fill the Creative Testing Tracker

Produces **Ad Creative Academy's Course 602 artifact** — Carlotta Costanzo's tracker, the one she uses
with her clients.

> "By consistently filling out this tracker, you ensure **every test has a clear purpose, learnings
> are captured, and winning ideas can be scaled efficiently.**"

⚠️ **Course 601 names the same sheet** as the *"Creative Testing Tracker & Pipeline template"*, and
describes it as *"a strategic document that builds institutional knowledge about what works and
why."* One artifact, two courses, two names.

⭐ **This is a memory, not a report.** Mirella is explicit: *"This isn't meant to replace your
reporting tools."* Carlotta's tracker holds the reasoning; the dashboard holds the numbers.

## What this skill needs from you

**Required:**

1. **The tests** — what is being tried, or what was. One row per experiment
2. **What each test changes**, and against what. A row that cannot name the variable cannot be read
   later

**Optional, and each one fills real columns:**

3. The hypothesis, if it was written down before launch
4. Live dates
5. Results, and the metrics behind them: ROAS, CPA, CVR, CTR, hook rate, hold rate, watch time
6. Concept IDs and hook identifiers, if the account uses a naming convention
7. The persona each test targets
8. Whether each is net new or a fix

⛔ **Never invent a metric value, a date or a result.** This sheet is institutional memory: a number
written here is read months later by someone who was not in the room, with no way to tell it was a
guess. **Empty is a usable cell. Wrong is not.**

⛔ **Never write a hypothesis after seeing the result.** A hypothesis recorded retrospectively always
looks confirmed, which quietly destroys the only thing this document is for. If a test ran without
one, write `not recorded before launch`.

## How to run it

**Log tests before they launch where possible**, which is what makes the Hypothesis column mean
anything. When filling in a backlog of completed tests, say so.

1. **Establish whether the test has run yet.** Before-launch and after-the-fact logging fill different
   columns, and conflating them makes the hypothesis meaningless.
2. ⛔ **Write the hypothesis first** if the test has not launched. A hypothesis added after a result is a
   description, not a prediction.
3. **Emit the tracker** from **The Creative Testing Tracker** (below), all of ACA's columns, in their order.
4. ⛔ **Append KPI, Channel and Priority**, and mark them as additions. ACA's sheet has no column for them and
   Course 602's method needs all three.
5. **Fill the creative-metric columns.** ⚠️ ACA never fills its own in the example rows, so there is no model
   to copy — use Course 402's definitions and say which you used.
6. **Give every row a next step**, per the rule below. That is the column that makes this institutional memory
   rather than a log.

**Every row gets a next step.** Carlotta puts it strongest: *"And, **most importantly**, the next
steps based on what you've learned."* A completed row with an empty Action Items cell is a test you
paid for and did not use.

## ⚠️ What this skill is not

**It does not design the tests.** The Level 1 / Level 2 framework, the five iteration types and the
analysis method are `aca-602-creative-testing`.

**It does not define the metrics.** No formula or threshold for ROAS, CPA, hook rate or hold rate
appears in Course 602 or in this sheet. Those are `aca-402-key-metrics`.

**It does not decide how many tests to run.** That is Course 601's volume ladder.

## Reference files

| File | Read it when |
|---|---|
| **The Creative Testing Tracker** (below) | ⭐ All nineteen columns, the two banner groups, ACA's worked rows, and the shape to emit |
| **Provenance** (below) | ⚠️ **Read before treating the metric grouping as intentional.** What the sheet omits, and where it contradicts another ACA course |

---

## The Creative Testing Tracker

⛔ **Emit the columns below, in this order, filled.** Not a summary of what a tracker holds.

### The banner row

ACA's sheet carries a banner above the headers, splitting the metrics into two groups:

| Banner | Spans |
|---|---|
| *(none)* | Test Status → Action Items/Learnings |
| **ACTION METRICS** | Live Date → CTR (Link) |
| **CEATIVE METRICS** | HOOK RATE → CTR (All) |

⚠️ **"CEATIVE" is ACA's own typo**, missing its R. Reproduced here because it is what the shipped
file says; correct it silently in anything you hand a client.

⛔ **The ACTION METRICS banner spans Live Date and Results, which are not metrics** — so the merge is
loose. It also puts **CTR (Link) on the action side and CTR (All) on the creative side**, which
inverts Course 402 on both counts. See **Provenance** (below) before treating either as
deliberate.

### The nineteen columns

**The setup half** — what the test is:

| # | Column | What goes in it |
|---|---|---|
| 1 | **Test Status** | ACA's own values: `Waiting` · `Live` · `Completed` |
| 2 | **Asset Type** | ACA's own values: `Net New` · `Fix` |
| 3 | **Concept ID** | `C1`, `C3`, `C5` in ACA's rows — ties the test to a concept |
| 4 | **Hook** | `A`, `C` — the hook identifier |
| 5 | **Concept/Ad Type** | Street Interview · Podcast · Before and After · Tutorial |
| 6 | **Persona** | ⚠️ Present in the sheet and **empty in every one of ACA's worked rows** |
| 7 | **What are we testing?** | The variable. *"Bizarre texture hook"*, *"Text to voice over and no music"* |
| 8 | **Hypothesis** | *"Will increase TSR and CTR"* |
| 9 | **Action Items/Learnings** | ⭐ The next step. *"Test other textures"*, *"Keep using actor VO"* |

*(A blank spacer column sits here in the workbook.)*

**The results half:**

| # | Column | Group |
|---|---|---|
| 10 | **Live Date** | ACTION METRICS |
| 11 | **Results** | ACTION METRICS |
| 12 | **ROAs** | ACTION METRICS |
| 13 | **CPA** | ACTION METRICS |
| 14 | **CVR** | ACTION METRICS |
| 15 | **CTR (Link)** | ⚠️ ACTION METRICS |
| 16 | **HOOK RATE** | CEATIVE METRICS |
| 17 | **HOLD RATE** | CEATIVE METRICS |
| 18 | **AVG WATCH TIME** | CEATIVE METRICS |
| 19 | **CTR (All)** | ⚠️ CEATIVE METRICS |

**And an asset link** sits above the table: *"ASSET: Add link to asset here."*

### ACA's worked rows

Reproduced exactly. ⚠️ **Note that all four leave every creative metric empty** — ACA's own example
fills only ROAS and CPA.

| Status | Asset Type | Concept | Hook | Concept/Ad Type | What are we testing? | Hypothesis | Action Items/Learnings | Live Date | Results | ROAs | CPA |
|---|---|---|---|---|---|---|---|---|---|---|---|
| Waiting | Net New | C1 | A | Street Interview | New talent, Female 40+ | Same script will work with a new older creator | Keep using younger talent, 20-30 | 01/11/2022 | Higher CPA | 1.7 | 42 |
| Waiting | Fix | C3 | C | Podcast | Add promo + urgency message to CTA | Will increase CTR and lower CPA | Add promo + urgency to other winning concepts | 14/11/2022 | Higher CTR and Lower CPA | 3.4 | 28 |
| Live | Fix | C5 | A | Before and After | Bizarre texture hook | Will increase TSR and CTR | Test other textures | 18/11/2022 | Higher TSR and CTR | 4.1 | 25 |
| Live | Fix | C6 | A | Tutorial | Text to voice over and no music | Will increase TSR and CTR | Keep using actor VO | 18/11/2022 | No impact | 3.1 | 32 |

⭐ **Read row 1 carefully — it is the most instructive one in the sheet.** The hypothesis was *"same
script will work with a new older creator"*; the result was *"Higher CPA"*; the learning was *"keep
using younger talent, 20-30."* **A failed test with a clear learning is a successful row.** Three of
the four rows are marked `Fix` rather than `Net New`, and one records *"No impact"*.

⚠️ **The status values are inconsistent with the data.** Two rows are `Waiting` and already carry
results and live dates in the past. Treat `Waiting / Live / Completed` as the intended vocabulary and
set it honestly.

### ⛔ Three fields the course requires that this sheet has no column for

Carlotta says to capture, per test: *the concept name and specific variation · **the KPI** · **the
channel** · the test hypothesis · **the priority** and live date · a clear summary of results · the
next steps.*

| Missing | Why it matters |
|---|---|
| **KPI** | Which metric this test is judged on. Without it, a row with four numbers has no verdict — every reader picks the metric that suits them |
| **Channel** | ⛔ A Meta test and a TikTok test are not comparable, and the sheet gives no way to tell them apart |
| **Priority** | What to run next when the backlog is longer than the budget |

⭐ **Add them as three extra columns and say you added them.** Santi's instruction for this round was
to ship ACA's template as it ships and flag the gap, so: emit the nineteen in ACA's order first, then
the three appended, clearly marked as additions the course asks for and the sheet omits.

### Emitting it

```csv
Test Status,Asset Type,Concept ID,Hook,Concept/Ad Type,Persona,What are we testing?,Hypothesis,Action Items/Learnings,Live Date,Results,ROAs,CPA,CVR,CTR (Link),HOOK RATE,HOLD RATE,AVG WATCH TIME,CTR (All),KPI [added],Channel [added],Priority [added]
```

⛔ **Before delivering:**

1. **Every row names its variable** in "What are we testing?", in a form another person could
   reproduce. *"New creative"* is not a variable
2. **Every completed row has a learning**, including the failures. ⭐ *"No impact"* is a result and
   the row still needs its next step
3. **Every hypothesis predates its result**, or is marked `not recorded before launch`
4. ⛔ **No invented numbers, dates or outcomes.** Blank beats plausible
5. **A note saying which columns are ACA's and which three were added**
6. **The KPI column filled for every row**, since it is the column that turns numbers into a verdict

⚠️ **If several rows share a concept ID, check they are actually variations of one concept.** That is
what makes the Level 2 validation argument work, and a tracker where every row is a new concept is
recording a series of guesses rather than a test programme.

## Provenance

### Source

**Ad Creative Academy** — the **Creative Testing Tracker**, the downloadable artifact of Course 602:
Creative Testing Best Practices. **Carlotta Costanzo**, GAIN.

**Held in two forms**, and this skill reads the second:

| Form | Why it matters |
|---|---|
| A **PDF export** of the sheet | ⛔ Its text extraction interleaves characters across cells — *"S ne a w m e o l s d c e r r ip c t r e w a il t l o w r ork with a"* — so the columns are unreadable |
| The **.xlsx workbook**, received 2026-W33 | ⭐ Clean cell values, the merged banner ranges, and the true column order. **This is the source of record.** Measured overlap with the PDF: 55.7% |

**Named in two courses.** Carlotta calls it *"the Creative Test Tracker I use with most of my
clients"*; Mirella's Course 601 calls it the *"Creative Testing Tracker & Pipeline template"* and the
*"creative pipeline document"*. **One artifact, three names.**

### ⛔ The sheet does not capture what the course says to capture

**Measured against the workbook.** Carlotta lists seven things to record per test. Three have no
column:

| She says to capture | Column exists? |
|---|---|
| The concept name and specific variation | ✅ Concept ID · Hook · Concept/Ad Type · What are we testing? |
| ⛔ **The KPI you're measuring** | **No** |
| ⛔ **The channel the test is running on** | **No** |
| Your test hypothesis | ✅ Hypothesis |
| ⛔ **The priority** and live date | **Live Date only** |
| A clear summary of results | ✅ Results |
| The next steps | ✅ Action Items/Learnings |

⭐ **KPI is the most consequential omission.** A row carrying ROAS, CPA, CVR and CTR with no stated
KPI has no verdict — whoever reads it later picks whichever number supports what they already think.

⛔ **Channel is the most dangerous.** Course 402 establishes that CTR bands are not portable across
platforms; a tracker that cannot say whether a row is Meta or TikTok invites exactly that comparison.

### ⛔ Its metric grouping contradicts Course 402

**The workbook's merged banner ranges, read directly from the file:**

| Banner | Merged range | Covers |
|---|---|---|
| **ACTION METRICS** | `K3:P3` | Live Date · Results · ROAs · CPA · CVR · **CTR (Link)** |
| **CEATIVE METRICS** | `Q3:T3` | HOOK RATE · HOLD RATE · AVG WATCH TIME · **CTR (All)** |

**Course 402 (Chloe Rhys) argues the reverse on both counts:**

- *"Engagement metrics like thumbstop and **CTR**? That's all you. That's your script. Your image.
  Your format. Your hook."* — CTR is one of the two metrics **creative owns**, and this sheet files
  CTR (Link) under **action**.
- On CTR (All): *"**Don't use it to evaluate creative effectiveness**, because not all of those clicks
  are meaningful."* This sheet files it under **creative**.

⚠️ **The evidence that this may be sloppiness rather than a position:** the ACTION METRICS merge also
spans **Live Date and Results**, which are not metrics at all. A banner that reaches two columns too
far to the left plausibly reaches one too far to the right.

⛔ **So carry it as a discrepancy, not as ACA's settled view.** When someone uses this sheet, the
useful thing to say is: pick which CTR you mean, say which platform it came from, and know that ACA's
own metrics course would put CTR (Link) in the other column.

### ⚠️ Defects in the shipped file

| | |
|---|---|
| **"CEATIVE METRICS"** | ACA's typo, missing its R. Reproduced verbatim in the emitted structure |
| **Status values contradict the data** | Two rows are marked `Waiting` while carrying results and past live dates |
| **The Persona column is empty in all four worked rows** | The column exists and ACA never demonstrates it |
| **All creative metrics are empty in all four rows** | ROAS and CPA are the only numbers ACA fills, in a sheet whose second banner is dedicated to creative metrics |

⭐ **The last one is worth noticing rather than dismissing.** The columns Carlotta's own course argues
hardest for — hook rate, hold rate, watch time — are the ones her example never fills.

### What is reproduced and what is added

**Every column name, banner, status value and worked row is ACA's**, in ACA's order and wording,
including the typo.

**This skill's organisation, not ACA's:** the split into a setup half and a results half, rendering
the columns as tables, and the pre-delivery checks.

**This skill's additions, drawn from the material rather than stated by it:**

- ⛔ **The three appended columns** — KPI, Channel, Priority — marked as additions rather than folded
  in silently. Santi's instruction for this round was to ship ACA's template as it ships and flag the
  gap.
- ⛔ **The rule that a hypothesis must predate its result**, or be marked `not recorded before
  launch`. A retrospective hypothesis always looks confirmed, which destroys the only thing the
  document is for. The course never raises it.
- ⛔ **The rule that no number, date or outcome may be invented**, because this sheet is read months
  later by someone who was not in the room and has no way to tell a guess from a measurement.
- ⭐ **The reading of row 1 as the most instructive row**: a failed hypothesis with a clear learning
  is a successful row. ACA supplies the example and never points at it.
- ⭐ **The note that a completed row with an empty Action Items cell is a test you paid for and did
  not use.**
- ⚠️ **The check that rows sharing a concept ID really are variations of one concept**, since that is
  what makes Course 602's validation argument work.
- ⚠️ **The observation that the status values contradict the worked data**, so the vocabulary is the
  intent rather than the example.
- **The note that this is a memory and not a report**, which Mirella states and Carlotta implies.

### ⚠️ How old this material is

ACA stamps no date on the workbook. Its worked rows carry **November 2022** dates. Received into this
library in **2026-W33**.

⭐ **The durable parts:** the column structure, the status vocabulary, and the discipline of a
hypothesis before launch and a learning after.

⛔ **What dates fastest:** the metric grouping, which platform norms and Course 402 both bear on, and
the 2022 example rows.

### Credit

Ad Creative Academy's template and Carlotta Costanzo's teaching are their own work. This skill fills
their sheet; it does not originate it.
