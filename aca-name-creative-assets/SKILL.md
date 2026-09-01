---
name: aca-name-creative-assets
description: Builds a creative naming convention and emits Ad Creative Academy's Ad Naming Convention Generator, all three sheets - the settings tab with its eight tracked dimensions and dropdown values, the generator tab that assembles the name string, and the ad type library of 18 video types, 16 graphic types and 8 triggers. Flags the six naming elements Course 601 teaches that the sheet has no column for, and the defects in ACA's shipped file including two dimensions sharing a code and three inconsistent code sets. Use this when nobody can tell which ads worked because of how they are named, when creative and media teams need a shared convention, when setting up a new account, or when someone asks for a naming convention or UTM structure. Requires knowing what you want to compare later - the convention is designed backwards from that.
---

# Name creative assets

Produces **Ad Creative Academy's Course 601 artifact** — Mirella Crespi's naming generator.

> "Let's start with something that **seems simple but is incredibly powerful**: naming conventions."

⭐ **The convention is designed backwards from the comparisons you want to run.** ACA's own argument:

> "Are image ads working better than video ads? Is UGC working better than studio production? Are ads
> with the VO better than ads with just music? And are funny hooks working better than hooks that
> show the problem first? **You can't answer any of these questions if your creatives are not named
> or tagged effectively.**"

⛔ **Ask what they want to compare before building anything.** A convention assembled without that
question will be missing exactly the field they need, which is what happened to ACA's own sheet.

## What this skill needs from you

**Required:**

1. **What you want to be able to compare later.** The four questions above are the starting set; the
   real ones are whatever this account argues about
2. **Who has to use it** — this is a joint document. *"This is a combined effort between creative
   strategists and media buyers. There's simply no way around it"*

**Optional, and each fills real dropdown values:**

3. The products or bundles being advertised
4. Who produces the creative: agencies, in-house, creators — by name
5. The talent that appears, or whether it is mashups, AI avatars or text-to-video
6. Asset lengths that actually get made
7. Landing page types
8. Whether the account already has a convention, and whether it is being followed

⛔ **Never invent a dropdown value.** The settings tab is what every future name is built from: a
producer or product name that does not exist becomes a category nobody can fill and a comparison that
never resolves.

⚠️ **Ask whether they will actually maintain it.** ACA names the alternative: *"if you're using a
tool like Motion... **you don't have to actually be using these naming conventions**, you can tag the
assets directly."* ⭐ A half-followed convention is worse than no convention, because it produces
comparisons that are silently wrong rather than obviously missing.

## How to run it

1. **Start from the comparisons**, and derive the dimensions each one needs
2. **Emit all three sheets** in ACA's structure — see **ACA's Ad Naming Convention Generator** (below)
3. ⛔ **Flag the six elements Course 601 teaches that ACA's sheet omits**, and say whether this
   account needs them. Three of the four questions above cannot be answered without them
4. ⛔ **Fix the code collisions**, and say you fixed them. ACA's file gives two dimensions the same
   code and uses three different code sets across its own tabs
5. **Name the delimiter and the separator explicitly**, and state what happens to spaces

## ⚠️ What this skill is not

**It is not a UTM or tracking-link builder.** ACA's second tab assembles a parameter string, and
verifying that a link resolves and reports correctly in analytics is a media-buying task the sheet's
own instructions hand back to the buyer.

**It does not tell you what to name a concept.** Concept IDs and hook identifiers come from the work;
this is the container for them.

**It does not decide what to test or track.** That is `aca-602-creative-testing`, and
`aca-track-creative-tests` for the log.

## Reference files

| File | Read it when |
|---|---|
| **ACA's Ad Naming Convention Generator** (below) | ⭐ All three sheets, every dimension and value, and the shape to emit |
| **Provenance** (below) | ⚠️ **Read before reproducing a code.** The defects in ACA's shipped workbook, and what its ad-type library does not match |

---

## ACA's Ad Naming Convention Generator

⛔ **Emit all three sheets, filled.** Not a description of what a naming convention contains.

**ACA's own description of how it works:** *"On the first tab, you'll build out all the parameters
you want to track. **The second tab includes dropdowns that automatically generate URL parameters**
when you make selections."*

---

### Sheet 1 — Paid Media Name Settings

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

### Sheet 2 — the generator

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

### Sheet 3 — Ad Types

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

### ⛔ The six elements Course 601 teaches that this sheet omits

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

### Emitting it

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

## Provenance

### Source

**Ad Creative Academy** — the **Ad Naming Convention Generator**, the downloadable artifact of Course
601: Launching Ad Campaigns. **Mirella Crespi**, Creative Milkshake.

**A three-sheet workbook**, received 2026-W33. Its structure is reproduced exactly: *Paid Media Name
Settings*, *Facebook-Ad*, and *Ad Types*.

⭐ **Two of the three sheets were never held before.** The library previously carried a PDF whose own
filename ends *"- Paid Media Name Settings"* — an export of the **first sheet only**. The generator
tab and the ad-type library arrive with the workbook. **Measured: the workbook shares 15.2% with that
PDF.**

⭐ **This closed a standing gap.** ACA's tracked-download list named an *Ad Naming Convention Sheet*
that the coverage manifest reported as not held. The workbook is it.

### ⛔ The sheet does not implement the convention its course teaches

**Measured against the workbook.** Course 601 lists **eleven** elements a naming structure should
track. The settings sheet has **eight** dimensions, of which **five** correspond.

| | |
|---|---|
| **Both** | Producer · Ad Type · Concept ID · Hook Identifier · Talent Name |
| ⛔ **Taught, no column** | **Date · File Name · Concept Stage · Format · Hook Category · VO Type** |
| **In the sheet, never taught** | Product · Asset Length · Landing Page |

⛔ **The consequence is specific, not general.** The course gives four comparative questions as the
whole reason for naming. **Three of them cannot be answered by this sheet**: *image against video*
needs Format, *VO against music* needs VO Type, *funny hooks against problem-first hooks* needs Hook
Category. Only *UGC against studio* survives, on Producer.

### ⛔ Defects in the shipped workbook

All four were read directly from the file and none is silently corrected in what this skill emits.

#### 1. Two dimensions share a code

**Asset Length** and **Landing Page** are both labelled `(al)` on the settings sheet. Any assembled
name using both is ambiguous.

#### 2. Three code sets, no two agreeing

| Dimension | Settings sheet | Generator header | Assembled string |
|---|---|---|---|
| Product | `pr` | `fu` | `fu` |
| Concept | `ct` | `ct` | `aa` |
| Ad Type | `at` | `at` | `cs` |
| Talent | `tt` | `tt` | ⚠️ `pr` |

⛔ **`pr` means Product on one sheet and Talent in the generated string.** The example string also
contains `pe`, which appears nowhere else, and an empty `at:`.

#### 3. A `#REF!` error

The generator's second data row is `#REF!`, so a single row is the only worked example.

#### 4. Broken dropdown numbering

The Ad Type list numbers three rows **28** and skips 30, 32 and 34. Cosmetic, but the list cannot be
referenced by number.

⚠️ **And a duplicate in the ad-type library:** *"Problem > Solution"* and *"Problem Solution"* are
both in the video list.

### ⚠️ Its ad-type library is not Course 401's

**Counted from both.**

| | Video | Static / graphic |
|---|---|---|
| **This workbook** | **18** | **16** |
| **Course 401** | **10** | **16** |

The names overlap heavily and do not match. ⛔ **Two ACA taxonomies for the same thing.** Course 401
is explicit that its names are a shared vocabulary rather than a standard — *"These names are what
make sense to me and my team"* — which applies here too. Pick one per account.

⭐ **The workbook's Triggers column has no home.** Eight triggers — Social Proof, Scarcity, Authority,
Curiosity, Cliffhanger, Specificity, Shocking, Bargains — ship in the ad-type sheet with no
corresponding dimension in the settings tab and no column in the generator. A vocabulary ACA supplies
and never wires up.

### ⚠️ The date format is ambiguous

The generator instructs *"Manually enter this value, DDMMYY"* and its example is `170223`. ⛔ **For
the first twelve days of any month `DDMMYY` and `MMDDYY` are indistinguishable**, and a naming
convention is exactly the place where that error survives for years. The course never raises it.

### What is reproduced and what is added

**Every sheet name, dimension, code, definition, dropdown value, column and worked string is ACA's**,
in ACA's order and wording, including the defects.

**This skill's organisation, not ACA's:** rendering the sheets as tables, stating the assembled-name
spec in one place, and the pre-delivery checks.

**This skill's additions, drawn from the material rather than stated by it:**

- ⛔ **The measurement that five of eleven taught elements are implemented**, and that three of the
  four comparative questions cannot be answered by the sheet.
- ⛔ **Naming all four defects**, with the instruction to fix the code collisions and say so rather
  than shipping an ambiguous convention.
- ⭐ **Designing the convention backwards from the comparisons**, which the four questions imply and
  the course never states as a method.
- ⚠️ **The date-format ambiguity**, and the suggestion to use `YYYY-MM-DD`.
- ⚠️ **The rule for spaces**, because ACA's own example contains `Talent Name ` with a trailing space
  that will break a parser.
- ⚠️ **The note that names have length limits** on both ad platform name fields and URL parameters,
  which the workbook never mentions while assembling ten key-value pairs.
- ⭐ **The observation that the Triggers list is unwired**, and would be a ninth dimension.
- ⭐ **The point that a half-followed convention is worse than none**, because it produces comparisons
  that are silently wrong rather than obviously missing. ACA names the tagging alternative and does
  not draw this conclusion.
- ⚠️ **The comparison against Course 401's library.**

### ⚠️ How old this material is

ACA stamps no date on the workbook. Its worked example carries a `170223` launch date. Received into
this library in **2026-W33**.

⭐ **The durable parts:** the dimensional approach, the definitions, and the two verification steps.

⛔ **What dates fastest:** the Google Analytics verification path (*Real-Time > Traffic Source*), the
sheet named *Facebook-Ad*, and the ad-type vocabulary.

### Credit

Ad Creative Academy's template and Mirella Crespi's teaching are their own work. This skill fills and
corrects their workbook for a new account; it does not originate it.
