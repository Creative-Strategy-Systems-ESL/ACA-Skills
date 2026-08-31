---
name: aca-write-ai-image-prompts
description: Writes AI image and video prompts in Ad Creative Academy's Course 802 structure and EMITS them filled - the eight-slot image formula, the six-slot video formula, the Midjourney parameter block, and the iteration plan that says which slots to hold and which to flip so one prompt becomes a library. Also emits the five-step asset-cloning run sheet when brand images are supplied, reverse-engineering a brand's visual signature into a reusable prompt. Carries ACA's own film stock, camera, lens, lighting, composition and motion vocabulary. Use this when someone needs prompts for ad visuals, when AI images come back generic or off-brand, when a brand needs many on-brand variants from one reference shot, when a still has to become video, or when a prompt is producing the wrong thing and nobody knows which words to change. Requires the brand and what the asset is for.
---

# Write AI image and video prompts

Produces **Ad Creative Academy's Course 802 artifact** — Rory Flynn's prompt formulas, filled.

> "**A clear and direct prompt will equal a clear and direct output**, an ambiguous prompt will equal an
> ambiguous output"

⛔ **The rule that makes every slot mandatory:**

> "essentially, **every one of these elements, they have to be in an image**. So if we look at all of
> these, **if you take one out, the image doesn't really exist** ... so **it's gonna add it in there**."

⭐ **So a blank slot is not a blank slot.** It is a slot the model fills for you. Every emitted prompt
fills all of them or says explicitly which one is being left to the model and why.

## What this skill needs from you

**Required:**

1. **The brand, and what it sells.**
2. **What the asset is for** — a static ad, B-roll, a storyboard frame, a mood board, an email GIF. This
   decides the aspect ratio, the quality bar and whether video prompts are needed at all.
3. **The subject.** One subject to start: *"don't go in there and try to add a bunch of different people
   and a bunch of different props ... **add those as you go along**"*.

**Required only for asset cloning:**

4. ⛔ **Brand images you have the right to use.** Rory's own disclaimer travels with the technique: *"try
   to only do this on your brand, **don't go do this to other people's brands**"*.

⛔ **The gate is on the aesthetic, not on the file.** *"Make me prompts that look like [competitor]'s
ads"* needs no images at all and is the same act as cloning their photographs. **A verbal description of
a named competitor's look does not get through because no upload happened.** Ask whose aesthetic is being
reproduced, not just whose files arrived.

⭐ **What is legitimate, and it is most of what people actually want:** reproducing *their own* brand;
building from a **generic** aesthetic named by its qualities (editorial, lo-fi, clinical, golden-hour)
rather than by whose brand it is; or ⭐ **studying a competitor's structure and rebuilding it natively**,
which is Course 301's method and is a different thing from copying their visual signature.

**Useful, and each one fills real slots:**

5. Brand colours, and any locked palette
6. An existing ad or photo that worked, which becomes the signature to hold
7. Whether the still becomes video later. ⭐ **Ask this before writing the image prompt**, not after: it
   changes the prompt
8. Which generator they use, because Midjourney takes token prompts and Flux wants natural language

⛔ **Never invent a brand colour, a product detail or a claim.** A prompt is a production instruction; a
wrong colour becomes a wrong asset that someone ships.

## How to run it

1. **Establish the signature before the subject.** Five slots carry the brand and three carry the
   variation, so the signature is the reusable part. See `reference/the-formulas.md`.
2. **Emit the image prompt, all eight slots filled**, condensed-first in Rory's *"concentrated juice"*
   order: get everything in, then add water.
3. ⛔ **Emit the parameter block separately, and label its source.** The formula is taught on the
   recording; the parameters come from the course's cheat sheet and **are never mentioned in the
   recording at all.** Keeping them in one block makes that boundary visible and makes them easy to drop
   for a non-Midjourney tool.
4. **Emit the iteration plan** — hold these five, flip these three, and here are the first five variants.
   ⭐ This is what turns one prompt into a library, and it is the actual deliverable.
5. **If the asset becomes video**, emit the six-slot video prompt too, and ⭐ **go back and add motion
   tokens to the image prompt**: *"if there's already motion in the image, **you're giving the video
   generator about a 50% leg up**"*.
6. **If brand images were supplied**, emit the five-step asset-cloning run sheet instead of guessing a
   signature.

## ⭐ Emit prompts, not descriptions of prompts

The output is text somebody pastes into a generator. It is wrong if it needs interpreting first.

- **Slots in order**, comma-separated, no full sentences
- ⭐ **Strong keywords, powerful language.** *"**big versus enormous, enormous sounds better**, like
  colorful versus vibrant, vibrant sounds better, but **they also produce better imagery within the
  tool**"*
- **Every parameter with a value**, not a placeholder
- **Text to appear in the image goes in quotation marks**, and only a word or two: *"you're not gonna be
  able to add a paragraph"*

## ⚠️ What this skill is not

⛔ **It does not decide what the ad should say.** Concepts and hooks are Course 401, ad structure is
Course 103, and the psychology is Course 102. A beautiful prompt for the wrong message is a waste of a
generation.

⛔ **It cannot promise a specific tool's current behaviour.** Every parameter, version and UI in the
source dates fast, and the course says so: *"I could be talking to you right now, and five new models
have already released."* Emit the prompt, name the tool as the example it is.

⛔ **It does not train models.** That is Course 802's own module and needs 5 to 100 curated images; route
to `aca-802-ai-image-video-ads`.

⚠️ **And it cannot tell you the prompt will work first time.** Rory says the opposite, repeatedly: *"most
of the time you're not going to get an image or a video that comes out the way that you want it to on the
first shot."* ⭐ **The iteration plan is not a consolation prize, it is the method** — the reason to fill
all eight slots is that a named slot is a slot you can change.

## Where to go

| You need | Go to |
|---|---|
| The two formulas, the vocabulary, the parameter block | `reference/the-formulas.md` |
| The asset-cloning run sheet | `reference/the-formulas.md`, last section |
| Why the parameters are flagged, and what is sourced | ⚠️ `reference/provenance.md` |
| The mechanism behind all of it | `aca-802-ai-image-video-ads` |
