# Provenance

## Source

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

## ⛔ The sheet does not implement the convention its course teaches

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

## ⛔ Defects in the shipped workbook

All four were read directly from the file and none is silently corrected in what this skill emits.

### 1. Two dimensions share a code

**Asset Length** and **Landing Page** are both labelled `(al)` on the settings sheet. Any assembled
name using both is ambiguous.

### 2. Three code sets, no two agreeing

| Dimension | Settings sheet | Generator header | Assembled string |
|---|---|---|---|
| Product | `pr` | `fu` | `fu` |
| Concept | `ct` | `ct` | `aa` |
| Ad Type | `at` | `at` | `cs` |
| Talent | `tt` | `tt` | ⚠️ `pr` |

⛔ **`pr` means Product on one sheet and Talent in the generated string.** The example string also
contains `pe`, which appears nowhere else, and an empty `at:`.

### 3. A `#REF!` error

The generator's second data row is `#REF!`, so a single row is the only worked example.

### 4. Broken dropdown numbering

The Ad Type list numbers three rows **28** and skips 30, 32 and 34. Cosmetic, but the list cannot be
referenced by number.

⚠️ **And a duplicate in the ad-type library:** *"Problem > Solution"* and *"Problem Solution"* are
both in the video list.

## ⚠️ Its ad-type library is not Course 401's

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

## ⚠️ The date format is ambiguous

The generator instructs *"Manually enter this value, DDMMYY"* and its example is `170223`. ⛔ **For
the first twelve days of any month `DDMMYY` and `MMDDYY` are indistinguishable**, and a naming
convention is exactly the place where that error survives for years. The course never raises it.

## What is reproduced and what is added

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

## ⚠️ How old this material is

ACA stamps no date on the workbook. Its worked example carries a `170223` launch date. Received into
this library in **2026-W33**.

⭐ **The durable parts:** the dimensional approach, the definitions, and the two verification steps.

⛔ **What dates fastest:** the Google Analytics verification path (*Real-Time > Traffic Source*), the
sheet named *Facebook-Ad*, and the ad-type vocabulary.

## Credit

Ad Creative Academy's template and Mirella Crespi's teaching are their own work. This skill fills and
corrects their workbook for a new account; it does not originate it.
