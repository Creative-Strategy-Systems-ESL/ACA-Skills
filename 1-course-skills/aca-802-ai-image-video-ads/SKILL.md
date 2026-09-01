---
name: aca-802-ai-image-video-ads
description: Ad Creative Academy Course 802, Rory Flynn of Systematiq Ai - producing ad-ready images and video with generative AI, and it PRODUCES prompts in his formula rather than describing them. Covers how diffusion models and token weighting actually decide an output, the eight-slot image prompt formula and the six-slot video structure, asset cloning to reverse-engineer a brand's visual signature into infinite variants, training custom LoRA models for products, characters and styles, the nine camera motions, and why image-to-video lives or dies on the base image. Use this when a brand has no assets or recycled photography, when static creative runs out mid-month, when AI images come back generic or off-brand, when a product must look identical across shots, or when someone needs B-roll or storyboards without a shoot. Reach for it whenever Midjourney, Flux, Kling, LoRA training or AI video come up.
---

# Course 802: Prompt to Production, Crafting AI-Generated Image & Video Ads

**Rory Flynn**, founder of Systematiq Ai, *"an operational AI company, meaning we look into people's
businesses, we find holes and then we plug those holes."* 2h 18m 32s, 9 modules.

⭐ **The largest course in the programme**, and the only one that teaches production craft for
generative AI rather than opinions about it.

> "in the next 90 minutes or so, we're gonna run a full ad creative process ... So hopefully by the end
> of this, you'll be able to go from start to finish, creating ads."

## What this skill needs from you

**Required, to produce anything:**

1. **The brand, and what it sells.** Asset cloning and model training are both brand-specific.
2. **What the output is for** — a static ad, B-roll, a storyboard, a mood board, an email GIF. The
   quality bar and the tool differ per use.

**Required for asset cloning specifically:**

3. ⛔ **Brand images you have the right to use.** Rory's own disclaimer is part of the method: *"try
   to only do this on your brand, don't go do this to other people's brands."*

**Required for model training specifically:**

4. **Between 5 and 100 images** of one subject, square, high resolution, multiple angles. One image
   will not work. ⛔ **One product per model, one colourway per model** — mixing them mashes them.
5. ⛔ **If the subject is a person, their written permission.** This course teaches a **character model**
   trained on a real face from multiple angles, and demonstrates it on the faculty member's own. ⛔ **The
   course itself sets no consent rule and this skill does not inherit that silence.** Course 801 states
   it plainly — *"do not copy a person's appearance or voice without their permission"* — along with
   documented creator permission and the platform labelling rules. ⛔ **Apply those here.** A trained
   character model is a reusable likeness, which is a larger thing to hold than one image.

**Useful:**

6. Which stage the team is at on the five-step adoption ladder, because that decides whether the
   answer is a prompt or an SOP
7. Existing brand photography, even if it is tired: it is the input asset cloning needs

⛔ **Never promise a specific tool's current behaviour.** Rory dates his own material inside the
course: *"I could be talking to you right now, and five new models have already released."* Teach the
method, name the tool as an example, and expect the UI to have moved.

## Where to go

| They are asking | Go to |
|---|---|
| Why did my prompt give me something generic? | `reference/how-it-works.md`, tokens and weighting |
| How do I write a prompt that works? | `reference/prompting.md` |
| How do I make AI images that look like *our* brand? | `reference/asset-cloning.md` |
| How do I get the same product in every shot? | `reference/custom-models.md` |
| How do I turn a still into video? | `reference/prompting.md`, image-to-video |
| Which tool should we use? | `reference/how-it-works.md`, the trade-off |
| Where did these claims come from? | ⚠️ `reference/provenance.md` |
| Just write me the prompts | `aca-write-ai-image-prompts` |

## The through-line

> "**A clear and direct prompt will equal a clear and direct output. An ambiguous prompt will equal
> an ambiguous output.**"

⭐ **And the structural consequence, which is the actual lesson:** every element of an image has to be
present in it. *"If you take one out, the image doesn't really exist, so it's gonna add it in
there."* You are not choosing whether lighting, environment and composition get decided. You are
only choosing **whether you decide them or the model does.**

## How to run it

**Mechanism, then formula, then the asset.** Someone who understands token weighting debugs their own
prompts; someone who does not rerolls.

1. **Explain diffusion and token weighting** from `reference/how-it-works.md`, including the removal
   experiment. ⭐ The lesson is that you choose whether *you* specify a slot or the model invents it.
2. **Give the eight-slot image formula** in `reference/prompting.md`, condensed-first.
3. **Add the six-slot video structure** and the nine camera motions, same file, plus the interaction clause
   that stops output reading as AI.
4. **Teach asset cloning** with `reference/asset-cloning.md` when the brand has tired photography. ⛔ Carry
   the disclaimer: their own brand only. ⚠️ And step 2 of the five fails on purpose — the LLM pass is the fix,
   not polish.
5. **Only reach for model training** in `reference/custom-models.md` when a product must be identical across
   shots. ⛔ If the subject is a person, get written permission first — see that file, and Course 801 for the
   rules this course omits.
6. ⭐ **To emit prompts, route to `aca-write-ai-image-prompts`** if installed. It labels which half of a
   prompt came from the recording and which from the worksheet.
7. **Check they can name the slot to change** when an image is wrong. "Try again" means step 1 did not land.

## Answering well

**Start with the mental model, not the prompt.** Diffusion models turn training images into noise and
recall them against your tokens. Fewer tokens means more weight on each, so a three-token prompt
gives a strong style and little control; a ten-token prompt gives moderate style and much more
control. ⭐ **This is why "add more detail" works** — and it is worth explaining, because someone who
understands it can debug their own prompts instead of rerolling.

**The formula is eight slots, and it is a starting point.** Photo type, shot type or composition,
subject and action, environment, colour scheme, camera details, lighting, and anything additional.
Rory's *"concentrated juice"* method: write the condensed version first, then add water.

**Asset cloning is five steps and step two fails on purpose.** Collect assets, run Midjourney's
`describe`, fine-tune in ChatGPT, attach a style reference, iterate. ⭐ **Rory shows the failure
rather than hiding it** — `describe` on its own produced images he calls *"crap"*, looking like *"video
games or fine arts."* The ChatGPT pass is not polish, it is the fix.

⭐ **What you actually keep is the prompt, not the image.** *"The idea isn't to get this image. We
don't wanna copy this image. We just need the prompt."* Hold the visual signature constant, flip the
photo type, subject and environment, and one asset becomes a library.

**For video, the X factor is motion.** The pipeline recalls motion first and builds frames around it,
so camera motion and subject motion are the load-bearing parts of a video prompt. ⚠️ **And
image-to-video is bounded by its still**: *"probably I'd say 70, 80 percent of doing image to video"*
is the base image. A subject a mile away cannot be pushed into close-up.

⚠️ **Quote the cons.** Rory does, repeatedly: video is glitchy, needs multiple generations, costs more
per generation than images, and mostly outputs 720p needing upscaling. He names the missing tool in
the whole stack, a creative video upscaler. A skill that only sells the upside is not this course.

## ⚠️ Scope

Production craft for generative assets. It does not decide **what** the ad should say: that is Course
401 for concepts and hooks, Course 103 for structure, and Course 102 for the psychology. It does not
measure anything either. ⛔ **No performance benchmark appears anywhere in this course**, and the one
measured claim in it is a cost-and-hours saving on a production process, not an ad result.

## Reference files

| File | Read it when |
|---|---|
| `reference/how-it-works.md` | Diffusion, tokens, weighting, the video pipeline, and choosing a tool |
| `reference/prompting.md` | The rules, both prompt structures, the nine camera motions, the three video modes |
| `reference/asset-cloning.md` | Reverse-engineering a brand's visual signature into variants |
| `reference/custom-models.md` | LoRA training for products, characters and styles |
| `reference/provenance.md` | ⚠️ **Read before quoting any number or tool claim.** Includes the course-number conflict |
