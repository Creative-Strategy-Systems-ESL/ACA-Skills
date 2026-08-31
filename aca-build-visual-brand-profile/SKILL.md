---
name: aca-build-visual-brand-profile
description: Builds and EMITS a Visual Brand Profile in Ad Creative Academy's Course 803 structure - the six sections (core identity, composition, subject styling, imagery, style, signature details) extracted from a brand's own images, plus the system prompt that turns it into a repeatable generator. This is the artifact ACA's own Weavy workflow template names as its third step and the course calls the only thing that needs to change to point a whole AI workflow at a new brand. Use this when AI images come back off-brand, when a workflow built for one brand must serve another, when several people generate creative and none of it matches, or when someone needs a written definition of what a brand looks like. Requires around 10 of the brand's own images.
---

# Build a Visual Brand Profile

Produces **Ad Creative Academy's Course 803 artifact** — the profile that makes an AI workflow brand-aware.

⭐ **Why it is worth building.** In the course, this one document is the difference between a workflow that
serves one brand and a workflow that serves any:

> "**a visual brand profile is the only thing that really needs to change in all of this**, right? So if we
> want to do this for a different brand, **we just have to change the visual brand profile**"

⭐ **ACA's own workflow template makes it Step Three**, with the instruction to upload ten brand images and ask for a
visual profile usable to generate new images in the same style. **Both sources name the same
artifact**, which is rare in this programme.

## What this skill needs from you

**Required:**

1. ⛔ **Around 10 of the brand's own images.** Both sources say ten. ⛔ **Fewer than about five and there is
   no profile to extract** — you get a description of one photo. ⚠️ **And they must be the brand's**: Course
   802's disclaimer governs the whole technique, *"try to only do this on your brand, don't go do this to
   other people's brands."*
2. **The brand name, and what it sells.**

**Useful, and each one sharpens a section:**

3. **Which images are the brand at its best**, if the set is mixed. A profile averaged over on-brand and
   off-brand images describes neither
4. **Anything locked** — a palette, a logo rule, a packaging shot that cannot change
5. **What the profile is for**: static ads, website assets, B-roll stills. ⭐ The course uses one profile
   across all three
6. Whether more than one person will use it, since a written profile is how output stays consistent between
   people

⛔ **Never invent a brand attribute.** The whole value is that the profile is *extracted* from real images. A
guessed colour or a guessed material becomes every future asset's error, multiplied by the batch size.

⛔ **Ask where the images came from, and reject the workflow's own output.** The obvious next move once a
generator is running is to re-extract a profile from its best generations. ⛔ **Do not.** Each pass then
describes the model's interpretation of the last pass rather than the brand, and the drift compounds
silently: nothing looks wrong in any single cycle, and after three the profile describes a brand that does
not exist.

⭐ **Re-extract from real photography only** — a shoot, the site, the packaging. ⚠️ **If a set is mixed,
say which images were real and which were generated**, and build from the real ones. This is the one
failure in the whole skill that produces confident, plausible, worsening output, and neither ACA source
mentions it.

⚠️ **If fewer than five images exist, say so and stop.** Offer the alternative: build the profile from the
brand's guidelines document if one exists, and mark it as declared rather than observed.

## How to run it

1. **Read the images and write the six sections.** See `reference/the-profile.md` for what each one holds.
2. ⭐ **Do the extraction in two passes.** The course does: *"I think I did it twice"* — write the profile,
   then feed the images back and ask what is missing. ⚠️ **One pass produces a thin profile**, which is the
   most common failure here.
3. ⛔ **Separate observed from declared.** Anything read off the images is observed; anything the brand told
   you is declared. They fail differently, and a reader must be able to tell.
4. **Emit it as text that can be pasted into a system prompt**, not as prose about the brand. It is a tool
   component.
5. **Emit the pairing system prompt too**, so the profile is usable immediately rather than being a document
   nobody wires up.
6. ⚠️ **Name what the profile cannot hold** — the product's fine details. Those come from the image input and
   the keep-this-change-that instruction, not from the profile.

## ⭐ Emit the artifact, not a description of it

The output is a component someone pastes into a workflow. It is wrong if it reads like a brand deck.

- **Six sections, each with concrete visual attributes**, not adjectives about the brand's values
- ⛔ **No marketing language.** `premium and trustworthy` generates nothing; `matte black surfaces, hard
  sidelight, deep shadow, 50mm, centred product` generates something
- **Every attribute expressed as something a generator can act on**: a colour, a material, a light
  direction, a lens, a crop, a texture
- ⭐ **Then the swap test**: state what would change if this profile were replaced with another brand's, and
  confirm nothing else in the workflow would need touching. That is the profile's whole job

## ⚠️ What this skill is not

⛔ **It is not brand guidelines.** It carries no logo rules, no typography, no tone of voice, no legal
requirements. It is the visual half, written for a generator.

⛔ **It does not make the product consistent.** The profile carries the *aesthetic*; the product's fine
details are held by the input image and the *keep:* clause. ⚠️ **Confusing the two is the failure mode** —
someone writes an excellent profile, gets on-brand images, and the packaging is still wrong.

⛔ **It does not build the workflow.** That is `aca-803-creative-automation`. This produces the piece the
workflow swaps.

⚠️ **And it does not survive a rebrand.** It is a snapshot of how the brand currently looks. Re-extract when
the photography changes.

## Where to go

| You need | Go to |
|---|---|
| The six sections and what belongs in each | `reference/the-profile.md` |
| The system prompt that consumes it | `reference/the-profile.md`, last section |
| Why ten images, and what is sourced | ⚠️ `reference/provenance.md` |
| The workflow this plugs into | `aca-803-creative-automation` |
| Prompts for a single asset instead | `aca-write-ai-image-prompts` |
