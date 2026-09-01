# ACA's Creative Sprint Planning board

⛔ **Emit the structure below, filled with the user's jobs.** Never with ACA's data.

## The five status sheets

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

## The 28-column job record

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

## The supporting tabs

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

## Emitting it

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

## ⛔ Before delivering

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
