# Provenance

## Source

**Ad Creative Academy** — Course 103: Creative Fundamentals (100-Level), taught by **Mirella
Crespi**, ACA's founder, of **Creative Milkshake**.

Three artifacts from that course are what this skill runs:

- **The Ad Building Blocks Analysis Worksheet** — 5 sections, reproduced in `reference/worksheet.md`
  with every field and every execution-style option intact.
- **AI Prompt for Ad Building Blocks Analysis** — the one-page mega-prompt, reproduced in full.
- **AI Prompts for Creative Analysis & Development: Consumer Psychology Edition** — the prompts
  from that pack which serve a teardown, plus the two that consume its output.

The modular building blocks framework itself comes from the course, not from the worksheet, which
prints the fields without the definitions behind them.

The worksheet's stated purpose, in ACA's words:

> "By breaking down ads into their core components, you'll develop the ability to identify what
> makes great creative work and how to replicate success."

## ⚠️ Two labelling errors in ACA's own materials

Both look like copy-paste slips in the PDF. Neither changes the framework, and both would confuse
anyone filling the printed sheet.

**1. Section 3's first block is headed "Product Introduction".** That is the Section 2 heading
repeated. Its fields are all problem-framing — personal story / experience, common pain point,
question-based — and ACA's own AI prompt names the first Person block **Problem Statement**. This
skill uses Problem Statement, and `worksheet.md` flags the discrepancy where a reader would hit it.

**2. Section 3's "Failed Alternative" block carries the field header "Demonstration Type".**
Another Section 2 heading repeated. The options under it are prior-solutions options, so the block
is right and only the field label is wrong.

⚠️ **A third apparent error is not one.** In the prompt pack, the second prompt under "Competitor
Ad Reverse Engineering" is headed **"Audience Pain Point Mining"** — a title carried over from the
Course 102 pack, where a prompt of that name genuinely exists and does something else. Its body
here is a building-block deconstruction. Named **Building Block Identification** in
`ai-prompts.md`, which is what ACA's own workflows call it.

## The block count, and why the worksheet appears to disagree with itself

The framework has **14 blocks**: 3 structure, 5 product, 6 person.

The worksheet's Section 1 handles the three structure blocks as sections rather than as
present/absent blocks, because every ad has all three. So the sheet's checkbox-style blocks number
11, and the framework's 14 includes hook, body and CTA. Both counts are correct and describe the
same thing.

## What is reproduced and what is this skill's

**Reproduced as written:** every worksheet section and field, all the execution-style options, the
Section 5 example formula, the mega-prompt in full including its framework-education half and its
nine analysis instructions, and each carried prompt with its `[BRACKETED]` placeholders.

**This skill's, drawn from the course rather than stated by it:**

- **The three-state input rule** — described ad, reference only, partial description — and the
  instruction to stop and ask when only a link or a name arrives. Not in the course. It is here
  because a teardown is written in the language of observation, so a fabricated one is
  indistinguishable from a real one and the reader cannot check it without doing the work
  themselves.
- **The distinction between a block being absent and a block being unobservable**, and the
  `NOT OBSERVABLE FROM THE DESCRIPTION GIVEN` and `PRESENT, EXECUTION NOT ASSESSABLE` markers. The
  worksheet has one column for present/absent, which silently merges the two.
- **The warning that some blocks' execution cannot be scored from a written description at all** —
  storytelling and before/after in particular, where the judgement rests on delivery, pacing and
  face rather than on what happens.
- **The separation of craft judgement from performance claims.** The worksheet asks which blocks
  "contribute most to this ad's effectiveness"; with no performance data supplied, that is an
  opinion about the creative and should not be written as a statement about results.
- The `ANALYSED FROM:` / `PERFORMANCE DATA:` header, the "what its absence usually means" column in
  `blocks.md`, the metric-points-at-the-block diagnostic, and the guidance on writing the Section 5
  formula.

**No worked example ships with this skill**, because the course does not provide one and inventing
a teardown of an invented ad would model exactly the behaviour the skill warns against. The
✅/⛔ examples in `worksheet.md` are illustrations of answer *quality* and are marked as such.

## Deliberate overlap with `aca-103-creative-fundamentals`

Both skills carry this framework and this worksheet, on purpose. Each has to run with nothing else
installed, so neither can point at the other for its content.

The split is by job:

- **`aca-103-creative-fundamentals`** teaches the framework, and covers the angle types and the
  wider creative-strategy vocabulary alongside it. Someone who wants to understand how ads are
  built wants that one.
- **This skill** tears down one specific ad and does not teach. Someone with a piece of creative in
  front of them wants this one.

Route on whether there is a specific ad on the table.

## Credit

The course, the framework, the worksheet and the prompts are Ad Creative Academy's work. This skill
organises that material so it can be run; it does not originate it.
