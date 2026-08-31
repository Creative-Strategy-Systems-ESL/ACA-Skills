# Provenance

## Source

**Ad Creative Academy** — Course 802: *Prompt to Production: Crafting AI-Generated Image & Video Ads*
(800-Level), **Rory Flynn**, 2h 18m 32s, 9 modules. **Two sources, and they were made separately:**

| Source | What it gives this skill |
|---|---|
| **The recorded course**, 29,461 words | The five prompting rules, both prompt structures, the eight photographic elements, the five asset-cloning steps, the nine camera motions, the interaction principle, the motion-baking technique, every worked prompt |
| **The Midjourney cheat sheet**, ACA's listed worksheet for the course | ⭐ **All twenty-two parameters**, the vocabulary lists (film stocks, cameras, lenses, lighting, composition, motion, photography styles), the token-position rule, and the moodboard image-count ladder |

⭐ **Both are needed and neither is sufficient.** The recording teaches the method and never names a
parameter. The sheet lists the parameters and teaches almost no method.

---

## ⭐ Where the two sources corroborate each other

This is unusual in this programme, where courses normally agree by accident or not at all. **These two
artifacts state the same three things independently:**

| | Recording | Cheat sheet |
|---|---|---|
| **The prompting rules** | Five, spoken | ⭐ **Six, numbered** — the same five plus *"separate key elements with commas"* broken out |
| **The prompt slots** | Nine elements, listed in speech | ⭐ **Seven, printed** as *"Photo Type Shot Type Subject Environment Tech Details Lighting Modifiers"* |
| ⭐ **Which slots to hold and which to flip** | *"flip the photo type, the subject and the action and the environment"* | *"**keep:** Color scheme, technical details, composition, lighting, modifiers"* |
| **The data-volume rule** | *"more data, more varied results. Less data, tighter results"* | The same rule: more images equals less consistency, fewer images equals a more defined style ⚠️ (see the doubled-text note below) |

⭐ **The hold/flip split is the important one.** It is the mechanism that turns one prompt into a brand
library, and it is stated twice, in different media, in near-identical terms. **Treat it as the most
reliable thing in the 800-Level.**

⚠️ **The slot counts differ because the two lists are cut differently.** The recording names *subject and
action* as one element and adds *colour scheme* and *composition* separately; the sheet compresses camera,
lens and film stock into *"Tech Details"*. **This skill emits eight slots, which is this skill's
reconciliation of the two**, not a number either source states.

---

## ⛔ The parameters are not taught anywhere in the course

**Measured, not assumed.** In the 29,461-word transcript:

- The literal string `--` appears **exactly twice**
- `--sref` appears **zero** times
- `stylize` appears **zero** times
- **Not one of the twenty-two parameters is named**

⛔ **This is why the emitted parameter block is labelled and kept separate.** Someone reading the output
must be able to tell which half carries the faculty's instruction and which half is a reference card for
one tool at one version.

⚠️ **The recording does teach style reference as a concept** — the phrase appears 7 times — and the sheet's
`--sref` is the flag for it. So the *idea* is taught and the *syntax* is not.

---

## ⛔ The cheat sheet contradicts itself on prompt order

Its prose says:

> "Beginning of prompt: Midjourney places the most focus on these tokens. end of prompt: Midjourney places
> the least focus on these tokens."

Its diagram labels say:

> "End of Prompt More Importance ... Beginning of Prompt Less Importance"

⛔ **These are opposites and nothing in the artifact resolves them.** The recording never mentions
token position at all, so there is no third source to break the tie.

⚠️ **This may be an artifact of reading a wall-sized board rather than a page** — the two labels could be
axis captions belonging to a diagram whose orientation cannot be recovered from the text. Either way, **it
is unresolved, and this skill says so rather than picking one.** Load-bearing tokens go early, because
that is what the prose says and what the recording's token-weight demonstration implies.

---

## ⚠️ The worksheet is third-party material, and it is a board not a document

- **No ACA branding and no course code appear on it.** It is attributed to Rory personally and distributed
  through the course. ACA's own curriculum sheet names it as this course's worksheet, which is why it
  belongs here.
- ⚠️ **It is a single page roughly 296 × 352 inches** — a wall-sized reference board exported as one page.
  Everything read from it comes from a spatial reconstruction of that canvas into reading order, not from
  normal page extraction. Layout-dependent meaning, like the order-of-importance diagram above, is exactly
  where that reconstruction is weakest.
- ⚠️ **It documents Midjourney V7.** The recording predates it: Rory references version 6.1 as current and
  5.2 as *"almost a year and a half removed"*. **The two sources are not contemporaneous.**

⚠️ **The sheet lists example `--profile` codes.** Those are personal style codes belonging to whoever
generated them; this skill does not reproduce them, because a stale or private code produces either
nothing or someone else's aesthetic.

⛔ **One region of the sheet has a doubled text layer.** Measured: **79 tokens** in and around the
moodboards panel render with every character duplicated, so *Moodboards* extracts as `MMooooddbbooaarrddss`
and *how many images to use* as `hhooww mmaannyy iimmaaggeess ttoo uussee`. The text is recoverable by
de-duplicating characters, but it is **not quotable verbatim**, which is why the moodboard ladder and the
data-volume rule appear here as readings rather than quotations. ⚠️ **The affected region includes the
moodboard image-count ladder**, so treat those numbers as read, not as quoted.

---

## What is quoted and what is organised

**Everything in quotation marks is ACA's**, from the recording or the sheet, checked character by character
against the source, with compressions marked by an ellipsis.

**This skill's organisation, not ACA's:**

- ⭐ **The eight-slot table with the hold/flip column.** Both sources state the rule; neither prints it as a
  table, and neither numbers the slots
- Separating the parameter block from the prompt, and labelling its source
- The interaction-clause table, assembled from six worked examples scattered across one module
- The motion-baking table, and moving it to a decision made *before* the image prompt is written
- The vocabulary lists regrouped by slot, since the sheet arranges them spatially

**This skill's additions, drawn from the material rather than stated by it:**

- ⛔ **The measurement that the parameters are untaught**, and the resulting source-boundary rule
- ⛔ **The finding that the sheet contradicts itself on prompt order**
- ⭐ **Naming the iteration plan as the deliverable** rather than the single prompt. Both sources imply it;
  neither says the output of prompt-writing is a plan
- ⭐ **The note that `--sref`, `--sw` and `--oref` do in one flag what asset cloning does in five steps**,
  when a usable reference image exists. Neither source connects them
- ⭐ **Making "does this become video?" a question asked before the image prompt.** The technique is
  ACA's; putting the question first is this skill's, because the source teaches it inside the video module
  where an image-stage reader will not find it
- ⚠️ **The gate on whose images these are**, promoted from a passing disclaimer to a required input
- ⚠️ **Treating environment as variable**, and saying why the sources are ambiguous about it

## Scope

Prompt production. ⛔ **It does not decide the message** (Courses 102, 103, 401), **does not measure
anything** (Courses 402, 701), and **does not train models** (Course 802's own module). ⛔ **No performance
benchmark exists anywhere in Course 802** — no CPA, ROAS, CTR or hook rate — so no emitted prompt should
carry a predicted result.

## Credit

Ad Creative Academy's curriculum and Rory Flynn's teaching are their own work; the cheat sheet is his. This
skill organises that material for reference and emits it filled; it does not originate it.
