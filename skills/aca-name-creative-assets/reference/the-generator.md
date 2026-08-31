# ACA's Ad Naming Convention Generator

⛔ **Emit all three sheets, filled.** Not a description of what a naming convention contains.

**ACA's own description of how it works:** *"On the first tab, you'll build out all the parameters
you want to track. **The second tab includes dropdowns that automatically generate URL parameters**
when you make selections."*

---

## Sheet 1 — Paid Media Name Settings

> "This is where you can customize the core traffic tag settings that your team uses. If you don't
> want to use this feature, simply erase what's listed. **Otherwise, whatever you list here will show
> up in the dropdowns of the other sheet.**"

**Eight dimensions.** Each column header carries a code in brackets, and ACA writes a one-line
definition above each.

| Dimension | Code | ACA's definition | Their example values |
|---|---|---|---|
| **Product** | `pr` | *"The name of the product or bundle the ad is for"* | Product name · Bundle Name · Offer |
| **Concept ID** | `ct` | *"The concept is the main message of the ad, how we attack the problem and present the solution"* | XXX · YYY · ZZZ |
| **Hook ID** | `hk` | *"A hook is an opening statement in a social video that attempts to grab the viewer's attention so that they want to continue watching"* | XXX · YYY · ZZZ |
| **Ad Type** | `at` | *"Certain ad types should perform better based on audience, funnel stage, or vertical"* | ProblemSolution · Storytelling · BeforeAfter · Greenscreen · Tutorial · CompetitorComparison · Mashup · ReactionVideo · CustomerReview · Unboxing · CommentResponse · POV · StylingReel · ComedySkit · Trend · ASMR · Listicle · BoldClaim · KeyBenefits · KeyPainPoints · Comparison · BeforeandAfter · BPR · Review · UGCReview · PR · SplitScreen · PriceBreakdown · GridSwap · HybridOverlay · SocialComments · HowTo · TextMessage |
| **Producer Name** | `st` | *"Identify if this was created by an agency, your in-house team or external creators"* | CreativeMilkshake · Internal |
| **Talent** | `tt` | *"Identify the talent featured in the ad, or if it's a mahsup or AI generated VOs and Avatars"* | Talent Name · Mashup · T2V · AI Avatar 1 |
| **Asset Length** | ⚠️ `al` | *"For non-vidoe assets, select IMG."* | IMG · 06sec · 10sec · 15sec · 30sec · 60sec · 90sec · 120sec |
| **Landing Page** | ⚠️ `al` | *"This is the landing page, or where the users goes after click on the ad."* | Homepage · PDP · Collection · LP-Listicle · Blog |

⛔ **Asset Length and Landing Page are both coded `al` in ACA's file.** Two dimensions cannot share a
code — the assembled name becomes ambiguous. **Change one and say you changed it.** `lp` for landing
page is the obvious fix.

⚠️ **ACA's Ad Type dropdown numbering is broken**: three rows are numbered 28, and 30, 32 and 34 are
skipped. Cosmetic, but it means the list cannot be referenced by number.

---

## Sheet 2 — the generator

**Ten columns.** The last one assembles the name and ACA marks it:

> "This part is **generated automatically** as you enter data in the columns to the left."

| # | Column | Code row |
|---|---|---|
| 1 | **Product** | `fu` ⚠️ |
| 2 | **Concept ID** | `ct` |
| 3 | **Hook ID** | `hk` |
| 4 | **Ad Type** | `at` |
| 5 | **Studio/Producer** | `st` |
| 6 | **Talent** | `tt` |
| 7 | **Asset Length** | `al` |
| 8 | **Destination URL** | `du` |
| 9 | **Date Launched** | `dl` — *"Manually enter this value, DDMMYY"* |
| 10 | **Program** | the assembled string |

**ACA's own worked row**, reproduced exactly:

```
fu:Product name_aa:YYY_hk:XXX_at:_cs:BeforeAfter_st:CreativeMilkshake_pr:Talent Name _pe:_al:06sec_du:_dl:170223
```

⛔ **Three different code sets appear in this one file, and no two agree.**

| Dimension | Sheet 1 says | Sheet 2 header says | The assembled string uses |
|---|---|---|---|
| Product | `pr` | `fu` | `fu` |
| Concept | `ct` | `ct` | `aa` |
| Ad Type | `at` | `at` | `cs` |
| Talent | `tt` | `tt` | ⚠️ `pr` — **which sheet 1 uses for Product** |

**The string also contains keys that appear nowhere else** (`pe`, and an empty `at:`), and leaves
`du` empty while a Destination URL column exists.

⛔ **So the generated example cannot be used as a specification.** Pick one code set, apply it
consistently across all three places, and say that you did.

⚠️ **A `#REF!` error sits in the row below**, so only the one row above is a worked example.

**ACA's verification instruction, which belongs in the output:**

> "Please test the code by 1) **clicking the code to be sure it takes you to the correct URL**, and
> 2) **verify in Google Analytics the traffic source is coming through as expected** (Real-Time >
> Traffic Source)."

---

## Sheet 3 — Ad Types

**Three lists.** Counted directly from the workbook.

**Video Ad Types — 18:** Problem > Solution · Storytelling · Before and After · Greenscreen ·
Tutorial · Competitor Comparison · Mashup · Reaction Video · Customer Review · Unboxing · Comment
Response · POV · Styling Reel · Problem Solution · Comedy Skit · Trend · ASMR · Listicle

⚠️ **"Problem > Solution" and "Problem Solution" are both in that list** — the same type twice under
two spellings. Deduplicate before using it as a dropdown.

**Graphic Ad Types — 16:** Bold Claim · Key Benefits · Key Pain Points · Comparison · Before and
After · Benefit-Product-Review · Featured Review · UGC Review · PR Feature · Split Screen · Price
Breakdown · Grid Swap · Hybrid Overlay · Social Comments · How To · Text Message

**Triggers — 8:** Social Proof · Scarcity · Authority · Curiosity · Cliffhanger · Specificity ·
Shocking · Bargains

⭐ **The Triggers column has no dimension in the settings sheet and no column in the generator.** It
is a vocabulary ACA ships and never wires up. If the account wants to compare ads by psychological
trigger, that is a ninth dimension to add.

⚠️ **This library is not the same as Course 401's.** That course teaches **10 video** and **16
static** ad types under different names. Two ACA taxonomies for the same thing; do not conflate them,
and pick one per account.

---

## ⛔ The six elements Course 601 teaches that this sheet omits

The course lists **eleven** things a naming structure should track. The sheet implements **five**.

| Missing | The comparison it makes impossible |
|---|---|
| **Format** | *"Are image ads working better than video ads?"* |
| **VO Type** | *"Are ads with the VO better than ads with just music?"* |
| **Hook Category** | *"Are funny hooks working better than hooks that show the problem first?"* |
| **Concept Stage** | Net-new against iteration — the split every volume tier is expressed in |
| **Date** | Anything time-based. ⚠️ The generator has *Date Launched*, which is not the same as created |
| **File Name** | A unique identifier independent of the assembled string |

⛔ **Three of the four questions ACA gives as the reason for naming cannot be answered by ACA's own
sheet.** Add the missing dimensions the account needs, and mark them as additions.

---

## Emitting it

**Sheet 1**, as a settings table:

```csv
Dimension,Code,What it records,Values
```

**Sheet 2**, as the generator:

```csv
Product,Concept ID,Hook ID,Ad Type,Producer,Talent,Asset Length,Destination URL,Date Launched,Assembled Name
```

**Sheet 3**, as three lists.

**Plus the assembled-name spec**, which ACA never states in one place:

```
<code>:<value>_<code>:<value>_ ...
```

⛔ **Before delivering:**

1. **One code set, used identically** in all three places. ⛔ Say which of ACA's you kept and what you
   changed
2. ⛔ **Ask whether assets already exist under an older convention.** Fixing ACA's codes is right for
   a new account and destructive for a running one: **a code that changes mid-account splits the
   history in two**, and every comparison spanning the change silently comes back wrong — which is
   the one thing naming exists to prevent. If prior assets exist, either keep the existing codes
   however flawed, or deliver a migration note saying which assets need retagging and from what date
   the new convention starts. **Never hand over a corrected convention without asking what it
   replaces.**
2. **No two dimensions sharing a code**
3. **A stated rule for spaces** — ACA's own example contains `Product name` and `Talent Name ` with a
   trailing space, which will break a parser
4. **Every dropdown value real**, or the dimension left empty with a note
5. ⛔ **The added dimensions marked as additions**, and the omitted ones listed with the comparison
   each unlocks
6. **The date format stated** — ACA uses `DDMMYY`, which is ambiguous against `MMDDYY` for the first
   twelve days of any month. Say which, or use `YYYY-MM-DD`
7. **ACA's two verification steps carried through** to whoever runs the links

⚠️ **Keep names short enough to survive the platform.** ACA's example assembles ten key-value pairs
into a single string and never mentions a length limit; ad platform name fields and URL parameters
both have them.
