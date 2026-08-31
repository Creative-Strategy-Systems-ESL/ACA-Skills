# Provenance

## Source

**Ad Creative Academy** — the **Creative Sprint Planning Template**, the downloadable artifact of
Course 703: Sprint Planning & Creative Volume. **Chloe Rhys**, Ex-TubeScience, now at OpenStore.

**An eleven-sheet workbook**, received 2026-W33.

⭐ **Ten of the eleven sheets had never been held.** The library previously carried a PDF export of
the **Home tab alone** — 86 extractable words. The 28-column job record, the five-stage status flow
and every supporting tab arrive with the workbook.

## ⛔ ACA shipped a working board, not a blank template

**Measured from the file.** It contains third-party operational data that is not course material:

| What | Extent |
|---|---|
| **Client brand names** | **47 distinct**, in the promo calendar |
| ⛔ **Live Facebook Ads Manager URLs** | **6**, carrying real `act=`, `business_id=`, campaign, ad set and ad IDs |
| **Staff first names** | 2, on real job records |
| **Real job records** and weekly performance | Including a named launch, and 265 rows of delivery and performance history |

**How this library handled it:** the byte-exact workbook is kept unchanged, and **the greppable text
layer is redacted** — 205 brand-name occurrences, 6 URLs and 2 staff names replaced by markers naming
what was removed. **Nothing structural was changed.** It is the only redacted text layer in the
library and its header says so.

⛔ **The rule this skill inherits: emit the structure, never the data.** No brand from ACA's calendar,
no person, no ads-manager link, not even as an illustrative example. Placeholders instead.

⚠️ **This matters more than it looks.** A filled sprint board is a document a team pastes into a
shared drive. A client brand name carried across from ACA's file would arrive in someone else's
workspace looking like their own data.

## ⚠️ Defects in the shipped workbook

| | |
|---|---|
| ⛔ **Three `#REF!` errors in the header row** | Columns 2, 4 and 21 have no readable name. The Launched sheet resolves column 21 as **# of Deliverables**; the other two are unrecoverable from the file |
| ⚠️ **The Planning sheet declares 50,500 rows** | They are blank checkbox defaults, not data. Only the first ~20 carry anything |
| ⚠️ **The Launched sheet has 48 columns**, not 28 | It adds performance and channel fields the earlier stages lack |
| ⚠️ **A stray "s"** | Two sheets are headed `www.adcreativeacademy.coms` |

⭐ **The `#REF!` errors are the same defect class found in ACA's storyboard template and its naming
generator** — three separate ACA workbooks shipping with broken formula references in structural
cells. Worth knowing as a pattern when reading any ACA workbook.

## ⭐ How the board implements Course 703

The **Job Type** column's values are the course's four request types — **MORE, FIX, ADAPT, NEW** —
and the status sheets are the sprint's stages. **This is the tightest course-to-template fit in the
programme**: unlike Course 601's naming generator, which implements five of the eleven elements it
teaches, this board implements what the course describes.

⚠️ **One thing the course specifies that the board does not enforce:** the sprint *mix*. The board
records each job's type and gives no view that totals them against the 30-40 / 20-30 / 20-30 / 10-20
targets. This skill checks the mix in the output instead.

## What is reproduced and what is added

**Every sheet name, column header, status value and event type is ACA's**, in ACA's order.

**This skill's organisation, not ACA's:** the split into status sheets and job record, rendering the
columns as a table, the CSV emit shape, and the pre-delivery checks.

**This skill's additions, drawn from the material rather than stated by it:**

- ⛔ **The redaction rule** — emit structure, never ACA's data, not even as an example.
- ⛔ **The rule that Creative Link and Launch Date stay blank** until the asset exists and the launch
  has happened or is scheduled, because those two columns are what distinguish planned from live.
- ⭐ **The reading that Complete and Launched are deliberately separate**, and that the gap between
  them is where approved creative dies quietly.
- ⭐ **The point that Base Job is what makes the board a system rather than a list** — it traces a
  MORE back to its win and a FIX back to its near-miss. The column exists; the course never says why
  it is load-bearing.
- ⭐ **The observation that the Angles tab is the most valuable and least obvious sheet**, because it
  attaches per-angle performance and turns angle choice into an evidence question.
- ⛔ **Checking the sprint mix in the output**, since the board records types and never totals them.
- ⛔ **Naming the three `#REF!` columns** rather than reproducing the error as a header.
- ⚠️ **The note that a MORE with no Base Job is a mislabelled NEW.**
- ⚠️ **Typing untyped jobs and showing the working**, since an untyped board cannot be mix-checked at
  all.

## ⚠️ How old this material is

ACA stamps no date on the workbook. Its promo calendar is headed **2025** and its job records carry
2025 dates. Received into this library in **2026-W33**.

⭐ **The durable parts:** the column set, the status flow, the four job types and the supporting-tab
structure.

⛔ **What dates fastest:** the aspect-ratio columns, the channel list, and the event types in the
promo calendar.

## Credit

Ad Creative Academy's template and Chloe Rhys's teaching are their own work. This skill fills their
board's structure for a new team; it does not originate it, and it deliberately carries none of the
client data ACA's file contains.
