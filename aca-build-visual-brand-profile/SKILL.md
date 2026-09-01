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

1. **Read the images and write the six sections.** See **The Visual Brand Profile** (below) for what each one holds.
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
| The six sections and what belongs in each | **The Visual Brand Profile** (below) |
| The system prompt that consumes it | **The Visual Brand Profile** (below), last section |
| Why ten images, and what is sourced | ⚠️ **Provenance** (below) |
| The workflow this plugs into | `aca-803-creative-automation` |
| Prompts for a single asset instead | `aca-write-ai-image-prompts` |

---

## The Visual Brand Profile

---

### What ACA says to do

**The instruction from the recording**, which is the prompt he uses:

> "I have a number of images I want to create a visual profile as a guide to create more images in the style
> of a brand."

⭐ **And what that returns:** *"what I'm doing is I'm uploading ten images and saying like, let's go create off
that, right. So we'll go and take those ten images, **create the core identity, composition, subject styling,
imagery, style, signature details**."*

**The instruction from ACA's workflow template**, Step Three, reassembled from its two-column layout:
*"Here are 10 brand images. Create a"* / *"visual profile I can use to generate new"* / *"images in the same
style."*

⭐ **Two sources, ten images, same artifact.**

⚠️ **Do it twice.** *"You can keep adding. You can stop there or just keep adding like here's more like add
to the visual profile. **I think I did it twice**, right? So have a good visual profile to work with."*

⭐ **The second pass is where a profile stops being generic.** First pass gets the obvious; showing it the
images again and asking what is missing gets the signature details, which are the part that makes output
recognisable.

---

### ⭐ The six sections

**Emit all six.** Each holds concrete, generatable attributes.

#### 1. Core identity

**What the brand is, visually, in one or two sentences a generator can use.** Not its values, its look.

- The category it reads as: luxury, clinical, utilitarian, lo-fi, editorial
- The overall finish: polished or raw, warm or cool, dense or minimal
- ⭐ The one thing that would be lost if it were removed

⛔ **Not this:** "premium, trustworthy, aspirational."
⭐ **This:** "cool-toned clinical minimalism, near-white studio space, product isolated and centred, nothing
decorative in frame."

#### 2. Composition

How the frame is built, across the set.

- Where the subject sits: centred, off-centre, rule-of-thirds, edge-cropped
- Crop and aspect ratios the brand actually uses
- Negative space: how much, and where it sits
- Symmetry or asymmetry; leading lines; horizon placement
- ⭐ **Whether space is reserved for copy**, which is the most practically useful thing in this section

#### 3. Subject styling

How people and products are presented.

- Wardrobe: colours, formality, era, whether it is neutral or branded
- Hair, skin, expression register: candid or posed, smiling or neutral
- ⭐ Casting read: age range, energy, whether subjects look professional or real
- How the product is held, worn or placed

#### 4. Imagery

What is depicted, and what never is.

- Recurring settings and environments
- Recurring props and materials
- ⭐ **What is absent.** A brand that never shows faces, never shows outdoors, never shows a second product
  is defined by those absences, and a generator will happily add them

#### 5. Style

The photographic and rendering treatment. ⭐ **The most generator-actionable section.**

- Palette: primary and secondary colours, named
- Lighting: direction, hardness, colour temperature, time of day
- Camera and lens character: focal length feel, depth of field, distortion
- Grain, texture, sharpness, film or digital character
- Grading: contrast curve, saturation, any colour cast

⭐ **Course 802's vocabulary lists belong here** — its lighting terms, film stocks, lenses and composition
terms are exactly this section's raw material. See `aca-write-ai-image-prompts`.

#### 6. Signature details

⭐ **The section that makes output recognisable rather than merely competent.** The small, repeated things.

- A recurring highlight, reflection or shadow shape
- A material that always appears: brushed metal, linen, wet stone, condensation
- A consistent surface the product sits on
- An edge treatment, a border, a consistent vignette
- ⭐ Anything a regular viewer would notice was missing without being able to name it

⚠️ **This is the section a single extraction pass usually leaves thin**, which is why the course runs it
twice.

---

### ⛔ Observed against declared

**Mark every attribute as one or the other.**

| | Where it came from | How it fails |
|---|---|---|
| ⭐ **Observed** | Read off the supplied images | Fails if the image set is unrepresentative |
| **Declared** | Told to you by the brand, or taken from guidelines | Fails if the brand's guidelines and its actual photography disagree, which is common |

⛔ **Never blend them silently.** When generated output looks wrong, the first question is which kind of
attribute misled it, and an unlabelled profile cannot answer that.

---

### What the profile does not hold

⛔ **The product's fine details.** Those are carried by the input image and the keep-this-change-that clause,
not by the profile:

> "keep colon this exact product visible and preserve define details"

⚠️ *"preserve define details"* is the transcript's rendering of *preserve fine details*.

⭐ **Say this explicitly in the emitted profile.** The failure mode is a good profile producing on-brand images
with wrong packaging, and whoever uses it next needs to know the profile was never responsible for that.

---

### ⭐ The system prompt that consumes it

**Emit this alongside the profile**, so it is wired up rather than filed. It is Course 803's six-part
structure with the profile pasted into core focus.

| Part | What to write |
|---|---|
| **Actors** | A visual role generic enough to serve several models. ACA's is *"a visual merchandizer"*, chosen because *"it's generic enough to know that it's going to go to multiple models"* |
| **Goal** | Generate prompts that render this brand's aesthetic from a loose idea |
| **Output** | *"for every user input, image or idea always generate a distinct prompt"* |
| ⭐ **Core focus** | ⭐ **The Visual Brand Profile, pasted in whole.** This is the only part that changes per brand |
| **Format** | The Course 802 slot formula, plus a length target. ACA uses *"Minimum of 250 to 350 words"* for natural-language models |
| ⛔ **Limits** | ⛔ *"do not include any explanation, just provide the"* prompt |

⛔ **Limits is not optional.** In a chained workflow the model's reply becomes the next step's input, so a
conversational answer breaks the chain: *"the back end is like, **do you have any more questions with those
things can screw up the output.**"*

⭐ **To batch it**, change two lines only: ask for ten prompts instead of one, and *"separate each prompt by a
star"*. Then split on that delimiter. Full mechanism in `aca-803-creative-automation`.

---

### ⭐ The swap test

**Close every emitted profile with this**, because it is the claim the artifact is making:

> "Once this thing is built **you're just switching the visual brand profile**. Right. And like this can be
> totally different."

**State plainly:** if this profile were replaced with another brand's, nothing else in the workflow would need
to change. ⭐ **If that is not true, the profile is carrying something that belongs elsewhere** — usually a
product detail that should be in the image input, or a format rule that should be in the system prompt's
format section.

**What ACA's finished generator then accepts** are plain briefs, because the profile is doing the brand work:

> "everything we're doing here is just **built on the brand principles. It's already has, like the brand style
> got attached. It's already going to create ten new prompts for you.**"

⚠️ **And be honest about the output.** *"I would consider all of these **raw assets** that you're going to have
to sort of doctor up in your own way."* The profile makes generations on-brand; it does not make them
finished.

## Provenance

### Source

**Ad Creative Academy** — Course 803: *The Creative Automation Workshop* (800-Level), **Rory Flynn**,
1h 34m 13s. The profile is taught in the course's final module, *Iteration Generator* (5m 49s).

⭐ **Two sources name this artifact independently**, which is unusual in this programme:

| Source | What it contributes |
|---|---|
| **The recorded course** | The extraction prompt, ⭐ **the six section names**, the do-it-twice instruction, the swap claim, and the finished generator it plugs into |
| **ACA's one-page workflow template** | ⭐ **Step Three names the artifact by name**, sets the input at 10 brand images, and gives its own suggested prompt |

⭐ **They agree on the input count (ten images) and on the artifact's purpose.** Neither cites the other.

---

### ⛔ What is ACA's and what is this skill's

**This is the most important distinction in this file**, because the balance here is different from most
skills in the folder.

#### ACA's, quoted directly

- ⭐ **The six section names**, verbatim: *"the core identity, composition, subject styling, imagery, style,
  signature details"*
- The extraction prompt: *"I have a number of images I want to create a visual profile as a guide to create
  more images in the style of a brand."*
- The template's Step Three prompt, reassembled from its two-column layout: *"Here are 10 brand images. Create
  a"* / *"visual profile I can use to generate new"* / *"images in the same style."*
- **Ten images** as the input, from both sources
- ⭐ **Do it twice:** *"I think I did it twice, right? So have a good visual profile to work with."*
- ⭐ **The swap claim:** *"a visual brand profile is the only thing that really needs to change in all of
  this"*
- The invitation to extend: *"You can keep adding. You can stop there or just keep adding like here's more
  like add to the visual profile."*
- **The raw-assets caveat:** *"I would consider all of these raw assets that you're going to have to sort of
  doctor up in your own way."*

#### ⛔ This skill's, and clearly marked as such

⛔ **ACA names the six sections and never says what goes in them.** The course gives the section list in a
single spoken sentence and then moves on to demonstrate the result. **Everything below is this skill's
elaboration**, built from what is visible in the course's own worked examples and from Course 802's
vocabulary:

- ⛔ **The contents of all six sections** — every bullet under every heading. **ACA supplies the headings
  only**
- ⛔ **The observed-versus-declared distinction.** Not in the source at all. Added because the two fail
  differently and a profile that blends them cannot be debugged
- ⛔ **The rule that the profile does not hold product detail.** The course implies it by keeping the *keep:*
  clause separate; it never states it, and it is the failure mode most likely to waste a batch
- ⭐ **The swap test as a closing step.** The claim is ACA's; turning it into a check the emitter must state
  is this skill's
- ⭐ **The reasoning for why the second pass matters**, and that signature details is the section it fixes
- ⭐ **Routing Course 802's lighting, lens, film-stock and composition vocabulary into the style section.**
  Neither course connects them
- ⚠️ **The floor of about five images**, and the instruction to stop and say so below it. ⛔ **ACA states no
  minimum.** The five comes from Course 802's model-training guidance — *"if you have one image, it's not
  really gonna be that great, but if you have at least five and ideally 10"* — which is a **different
  mechanism**, so it is an inference, not a rule
- ⚠️ **The marketing-language prohibition**, and the worked contrast showing what is generatable
- ⚠️ **The rebrand note**

⭐ **Why the elaboration is defensible anyway:** the six names are specific enough to be unambiguous, the
course demonstrates output from a filled profile at length, and Course 802 supplies the vocabulary. **But a
reader must know the section contents are a reconstruction**, not ACA's checklist, because ACA has no
checklist to hand over.

---

### ⚠️ The ten-image figure

**Both sources say ten**, and neither explains why.

⭐ **Weak corroboration from a different mechanism:** Course 802's object-model training band is *"10 to 20
images"*, and its cheat sheet's moodboard ladder puts **10-20 images** at *branded style*. **Three
appearances of the same range, by two mechanisms.** ⚠️ That is agreement, not evidence: none of the three
carries a source.

⚠️ **The template's Step Two adds a split with no rationale:** *"Generate 20 images (10 brand, 10
experimental)"*. ⛔ **Nothing in the recording explains the brand/experimental division**, so this skill does
not build on it.

---

### ⛔ The template's step one cannot be followed

ACA's one-page guide opens by telling the reader to open a hosted workflow template and *"Click Duplicate to
create your own workspace,"* then *"connect your accounts and complete setup."*

⛔ **That hosted template is not held in this library**, and the guide is the only place it is named. ⚠️ **The
recording's build-from-scratch walkthrough is the working fallback** and it is complete, which is why this
skill does not depend on the template existing.

⚠️ **The guide is also named nowhere in the recording.** Measured: the string *"workflow template"* appears
**zero** times in the transcript. It is attached to this course by ACA's curriculum sheet.

---

### ⚠️ Tool dependence

⛔ **The workflow this profile feeds runs inside one third-party node editor**, which was mid-acquisition when
the course was recorded. ⭐ **The profile itself is tool-independent** — it is a text document, and it works
pasted into any system prompt, any custom GPT, or by hand. **That is why this skill emits the profile and the
system prompt rather than a workflow.**

---

### ⚠️ Rights

⛔ **Course 802's disclaimer governs this technique and travels with it:** *"try to only do this on your
brand, don't go do this to other people's brands."*

⚠️ **Course 803 names client brands as examples without stating permission**, unlike Course 802, where Rory
explicitly notes one brand is not a client and that he asked another for permission. ⭐ **Apply 802's standard
here**, since it is the same person and the same technique.

---

### ⚠️ How old this material is

**ACA stamps no recording date.** Received into this library in **2026-W31**, a "no later than".

⭐ **What is durable:** the six sections, the ten-image input, the two-pass extraction, and the swap claim.
None depends on a tool.

⛔ **What dates:** the node editor, the models named around it, and the specific system-prompt length target.

### Scope

⛔ **Not brand guidelines** — no logo rules, typography, tone of voice or legal requirements. ⛔ **Not product
consistency** — that belongs to the input image and the *keep:* clause. ⛔ **Not the workflow** — that is
`aca-803-creative-automation`. ⛔ **And no performance claim**: Course 803 contains no metric, benchmark or
result anywhere, so an emitted profile must never carry a predicted outcome.

### Credit

Ad Creative Academy's curriculum and Rory Flynn's teaching are their own work. The six section names are
theirs; the elaboration of what each section holds is this skill's, marked as such above.
