# Provenance

## Source

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

## ⛔ The sheet does not capture what the course says to capture

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

## ⛔ Its metric grouping contradicts Course 402

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

## ⚠️ Defects in the shipped file

| | |
|---|---|
| **"CEATIVE METRICS"** | ACA's typo, missing its R. Reproduced verbatim in the emitted structure |
| **Status values contradict the data** | Two rows are marked `Waiting` while carrying results and past live dates |
| **The Persona column is empty in all four worked rows** | The column exists and ACA never demonstrates it |
| **All creative metrics are empty in all four rows** | ROAS and CPA are the only numbers ACA fills, in a sheet whose second banner is dedicated to creative metrics |

⭐ **The last one is worth noticing rather than dismissing.** The columns Carlotta's own course argues
hardest for — hook rate, hold rate, watch time — are the ones her example never fills.

## What is reproduced and what is added

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

## ⚠️ How old this material is

ACA stamps no date on the workbook. Its worked rows carry **November 2022** dates. Received into this
library in **2026-W33**.

⭐ **The durable parts:** the column structure, the status vocabulary, and the discipline of a
hypothesis before launch and a learning after.

⛔ **What dates fastest:** the metric grouping, which platform norms and Course 402 both bear on, and
the 2022 example rows.

## Credit

Ad Creative Academy's template and Carlotta Costanzo's teaching are their own work. This skill fills
their sheet; it does not originate it.
