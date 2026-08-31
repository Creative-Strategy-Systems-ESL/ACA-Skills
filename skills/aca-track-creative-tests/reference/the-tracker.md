# The Creative Testing Tracker

⛔ **Emit the columns below, in this order, filled.** Not a summary of what a tracker holds.

## The banner row

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
inverts Course 402 on both counts. See `reference/provenance.md` before treating either as
deliberate.

## The nineteen columns

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

## ACA's worked rows

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

## ⛔ Three fields the course requires that this sheet has no column for

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

## Emitting it

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
