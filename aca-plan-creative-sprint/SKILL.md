---
name: aca-plan-creative-sprint
description: Fills Ad Creative Academy's Creative Sprint Planning board for a real sprint, in the workbook's own 28-column job record and its five-stage status flow from Planning through In Progress, Review, Complete and Launched. Every job carries its request type (MORE, FIX, ADAPT or NEW), concept, angle, product, format, variant count, aspect ratios, launch date and channel, and the board's supporting tabs cover per-brand goals, products, an angle library with per-angle performance, a promo calendar and weekly delivery. Use this when a creative team needs a shared pipeline, when jobs keep getting lost between brief and launch, when planning a week or a quarter of creative, or when someone asks for a sprint tracker. Requires the jobs - it cannot plan a sprint it has not been told about.
---

# Fill the Creative Sprint Planning board

Produces **Ad Creative Academy's Course 703 artifact** — Chloe Rhys's planning board, the one her
team runs at OpenStore.

⭐ **The board is a pipeline, not a list.** A job has one row and moves through five status sheets;
the row is the same 28 columns at every stage.

## ⛔ Read this before producing anything

**The workbook ACA ships is a working board, not a blank template.** It contains real third-party
data: client brand names in its promo calendar, live Facebook Ads Manager links carrying real
account, business and campaign IDs, and staff names on real job records.

⛔ **Never reproduce any of it.** Emit the **structure** — sheet names, column headers, status values,
request types — and fill it only with what the user gave you. **No brand from ACA's calendar, no
person, no ads-manager URL, ever**, including as an example.

⚠️ **Use placeholders when you need to show the shape**: `[BRAND]`, `[REQUESTER]`, `[CREATOR]`,
`[LINK]`.

## What this skill needs from you

**Required:**

1. **The jobs** for this sprint — what is being made, and why
2. **The request type of each** — MORE, FIX, ADAPT or NEW. ⛔ If they were not typed, the mix cannot
   be checked, and the mix is the point of a sprint

**Optional, and each one fills real columns:**

3. Brand, product and angle for each job
4. Format, and how many variants each concept needs
5. Which aspect ratios are required
6. Requester and creator, if the board is shared
7. Due dates, and whether a job is business-as-usual or time-sensitive
8. Base job, for MOREs and FIXes — what this one iterates on
9. Reference links and creative direction

⛔ **Never invent a job, a date, a launch channel or a variant count.** This board is a team's shared
source of truth: a row somebody did not ask for becomes work somebody is expected to deliver.

⛔ **Never fill a Creative Link or a Launch Date that has not happened.** Those two columns are how
the board distinguishes planned from live, and a speculative entry makes a sprint look shipped.

## How to run it

1. **One row per job**, in the earliest status that honestly applies
2. ⭐ **Check the mix before delivering** — the four request types against ACA's target shares. A
   sprint that is all NEW has no pipeline behind it; a sprint that is all MORE is not learning
   anything
3. **Group by status**, since that is how the board is read at a standup
4. **Leave unknowns blank rather than guessed**, and list them

## ⚠️ What this skill is not

**It does not decide how many jobs a sprint should hold.** The five variables that set volume are
`aca-703-sprint-planning`, and Course 601's competing ladder is in `aca-plan-creative-volume`.

**It is not the test log.** A creative test's hypothesis, result and learning belong in
`aca-track-creative-tests`. This board tracks *production*; that one tracks *evidence*.

**It does not automate anything.** ACA's *Sprint Planning Operation System Worksheet* documents the
engineering stack OpenStore built around this board — Apps Script, n8n, Slack, a dashboard. It is
not a fillable worksheet, and it is carried inside `aca-703-sprint-planning`.

## Reference files

| File | Read it when |
|---|---|
| **ACA's Creative Sprint Planning board** (below) | ⭐ All 28 columns, the five status sheets, the supporting tabs, and the shape to emit |
| **Provenance** (below) | ⚠️ **Read before reproducing anything from ACA's file.** What was redacted and why, and the defects in the shipped workbook |

---

## ACA's Creative Sprint Planning board

⛔ **Emit the structure below, filled with the user's jobs.** Never with ACA's data.

### The five status sheets

A job is one row and moves between sheets. **The same 28-column record travels with it.**

| # | Sheet | What sits there |
|---|---|---|
| 1 | **📝 Planning** | Briefed, not started |
| 2 | **🧑‍💻 In Progress** | With an editor or designer |
| 3 | **👀 Review** | Awaiting QA or sign-off |
| 4 | **✅ Complete** | Approved, not yet live |
| 5 | **🌐 Launched** | In the ad account |

⭐ **Complete and Launched are deliberately separate**, and the gap between them is where creative
dies quietly. A concept that is approved and never launched has cost everything and taught nothing.

⚠️ **The Launched sheet carries extra columns** the earlier stages do not — the live performance and
channel fields — because that is where the job stops being a production record and starts being a
performance one.

### The 28-column job record

| # | Column | What goes in it |
|---|---|---|
| 1 | **📍 Status** | The stage. Matches the sheet |
| 2 | ⚠️ *(a `#REF!` error in ACA's header)* | See below |
| 3 | **💼 Brand** | ⛔ The user's brand. Never one from ACA's file |
| 4 | ⚠️ *(a second `#REF!`)* | |
| 5 | **👤 Requester** | Who asked for it |
| 6 | **👤 Creator** | Who is making it |
| 7 | ⭐ **🧪 Job Type** | **MORE · FIX · ADAPT · NEW** — Course 703's four request types |
| 8 | **✏️ Concept Name** | |
| 9 | **⏩ Base Job** | ⭐ What this iterates on. Required for MORE and FIX |
| 10 | **Base Job #** | |
| 11 | **👁️‍🗨️ Angle** | Drawn from the Angles tab |
| 12 | **📦 Product** | Drawn from the Products tab |
| 13 | **👀 Reference** | The inspiration or the ad being adapted |
| 14 | **💡 Direction** | Creative direction for the maker |
| 15 | **💾 Format** | Video, static, and so on |
| 16 | **Variants** | ⭐ How many. Course 703 recommends 3-6 per concept |
| 17 | **1x1** | Required? |
| 18 | **4x5** | Required? |
| 19 | **9x16** | Required? |
| 20 | **16x9** | Required? |
| 21 | ⚠️ *(a third `#REF!`; the Launched sheet calls this column **# of Deliverables**)* | |
| 22 | **Job #** | The unique identifier |
| 23 | **🔗 Creative Link** | ⛔ Only once the asset exists |
| 24 | **🚀 Launch Date** | ⛔ Only once it is live or scheduled |
| 25 | **✅ Completed** | |
| 26 | **📺 Channel** | Meta, TikTok, and so on |
| 27 | **📝 Notes** | |
| 28 | **Ad Status** | Live, paused, and so on |

⛔ **Three of ACA's header cells are `#REF!` errors**, not column names. Do not reproduce `#REF!` as a
header. The Launched sheet resolves one of them as *# of Deliverables*; name the other two from what
the account needs, and say you named them.

⭐ **Column 9, Base Job, is the one that makes the board a system rather than a list.** It is what
lets you trace a MORE back to the win it came from, and a FIX back to the near-miss. Without it the
four request types are just labels.

### The supporting tabs

| Tab | What it holds |
|---|---|
| **🏠 Home** | Per-brand: paid social DRI, creative lead, the quarter's creative-delivery goal, jobs-per-month goal against last-30-days pacing, backlog, wins, upcoming events |
| **Products** | Brand, brand code, product name — the source for column 12 |
| **Angles** | ⭐ An angle library: name, description, jobs ready, jobs launched, and **per-angle average spend, hook rate, CTR, CVR, ROAS, CPA and win %** |
| **🧰 Resources** | SOPs and tutorials |
| **Events** | A promo calendar: brand, event type, campaign, start and end dates |
| **Weekly Performance** | By week: creative delivered (jobs, ads), creative launched (jobs, ads), and performance (hook, CTR, CVR, ROAS, CPA, wins) |

⭐ **The Angles tab is the most valuable thing in the workbook and the least obvious.** It turns
angles from a brainstorm into a ranked asset with performance attached, which is what lets a team
answer `which angle should we brief next?` with evidence.

⚠️ **ACA's Events tab lists ten event types**: Discount · Product Discount (in cart) · Order Discount
· Buy X Get Y · GWP · Strikethrough · Shipping · Product Launch · Refresh · Evergreen. ⛔ The brands
beside them are ACA's clients and are not reproduced.

### Emitting it

```csv
Status,Brand,Requester,Creator,Job Type,Concept Name,Base Job,Base Job #,Angle,Product,Reference,Direction,Format,Variants,1x1,4x5,9x16,16x9,# of Deliverables,Job #,Creative Link,Launch Date,Completed,Channel,Notes,Ad Status
```

⚠️ **Illustrative rows, with placeholders where real data would go.**

| Status | Brand | Job Type | Concept Name | Base Job | Angle | Format | Variants | 9x16 | Job # | Launch Date | Channel |
|---|---|---|---|---|---|---|---|---|---|---|---|
| Planning | `[BRAND]` | **MORE** | Sleep-angle static, new headline set | J-104 | Sleep | Static | 4 | ✓ | J-118 | *(blank until live)* | Meta |
| Planning | `[BRAND]` | **FIX** | Tutorial re-cut, stronger opener | J-097 | Ease of use | Video | 3 | ✓ | J-119 | *(blank until live)* | Meta |
| In Progress | `[BRAND]` | **ADAPT** | Reviews-mashup format on Product B | J-088 | Social proof | Video | 5 | ✓ | J-120 | *(blank until live)* | TikTok |
| Review | `[BRAND]` | **NEW** | Sceptical-voice opener, unproven | — | Doubt | Video | 4 | ✓ | J-121 | *(blank until live)* | Meta |

⭐ **Note the Base Job column on rows 1 to 3 and the dash on row 4.** That is the difference between a
sprint that compounds and one that starts over every week.

### ⛔ Before delivering

1. ⛔ **No brand, person or URL from ACA's workbook appears anywhere.** Placeholders instead
2. **Every MORE and FIX names its Base Job.** A MORE with no parent is a NEW that has been mislabelled
3. ⭐ **The mix is stated and checked** against Course 703's targets — MORE 30-40% · FIX 20-30% ·
   NEW 20-30% · ADAPT 10-20%. Say the actual split and flag it if it is off
4. **Creative Link and Launch Date are blank** unless the asset exists and the launch has happened or
   is scheduled
5. **The three `#REF!` columns are named**, not reproduced as errors
6. ⛔ **A line naming every cell left blank because it was not supplied**, so nobody reads a gap as a
   decision

⚠️ **If the jobs were given without request types, type them and say you did.** Guessing the mix is
worse than asking, but an untyped board cannot be checked at all — so type them, show your working,
and let the user correct it.

## Provenance

### Source

**Ad Creative Academy** — the **Creative Sprint Planning Template**, the downloadable artifact of
Course 703: Sprint Planning & Creative Volume. **Chloe Rhys**, Ex-TubeScience, now at OpenStore.

**An eleven-sheet workbook**, received 2026-W33.

⭐ **Ten of the eleven sheets had never been held.** The library previously carried a PDF export of
the **Home tab alone** — 86 extractable words. The 28-column job record, the five-stage status flow
and every supporting tab arrive with the workbook.

### ⛔ ACA shipped a working board, not a blank template

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

### ⚠️ Defects in the shipped workbook

| | |
|---|---|
| ⛔ **Three `#REF!` errors in the header row** | Columns 2, 4 and 21 have no readable name. The Launched sheet resolves column 21 as **# of Deliverables**; the other two are unrecoverable from the file |
| ⚠️ **The Planning sheet declares 50,500 rows** | They are blank checkbox defaults, not data. Only the first ~20 carry anything |
| ⚠️ **The Launched sheet has 48 columns**, not 28 | It adds performance and channel fields the earlier stages lack |
| ⚠️ **A stray "s"** | Two sheets are headed `www.adcreativeacademy.coms` |

⭐ **The `#REF!` errors are the same defect class found in ACA's storyboard template and its naming
generator** — three separate ACA workbooks shipping with broken formula references in structural
cells. Worth knowing as a pattern when reading any ACA workbook.

### ⭐ How the board implements Course 703

The **Job Type** column's values are the course's four request types — **MORE, FIX, ADAPT, NEW** —
and the status sheets are the sprint's stages. **This is the tightest course-to-template fit in the
programme**: unlike Course 601's naming generator, which implements five of the eleven elements it
teaches, this board implements what the course describes.

⚠️ **One thing the course specifies that the board does not enforce:** the sprint *mix*. The board
records each job's type and gives no view that totals them against the 30-40 / 20-30 / 20-30 / 10-20
targets. This skill checks the mix in the output instead.

### What is reproduced and what is added

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

### ⚠️ How old this material is

ACA stamps no date on the workbook. Its promo calendar is headed **2025** and its job records carry
2025 dates. Received into this library in **2026-W33**.

⭐ **The durable parts:** the column set, the status flow, the four job types and the supporting-tab
structure.

⛔ **What dates fastest:** the aspect-ratio columns, the channel list, and the event types in the
promo calendar.

### Credit

Ad Creative Academy's template and Chloe Rhys's teaching are their own work. This skill fills their
board's structure for a new team; it does not originate it, and it deliberately carries none of the
client data ACA's file contains.
