# The Visual Brand Profile

---

## What ACA says to do

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

## ⭐ The six sections

**Emit all six.** Each holds concrete, generatable attributes.

### 1. Core identity

**What the brand is, visually, in one or two sentences a generator can use.** Not its values, its look.

- The category it reads as: luxury, clinical, utilitarian, lo-fi, editorial
- The overall finish: polished or raw, warm or cool, dense or minimal
- ⭐ The one thing that would be lost if it were removed

⛔ **Not this:** "premium, trustworthy, aspirational."
⭐ **This:** "cool-toned clinical minimalism, near-white studio space, product isolated and centred, nothing
decorative in frame."

### 2. Composition

How the frame is built, across the set.

- Where the subject sits: centred, off-centre, rule-of-thirds, edge-cropped
- Crop and aspect ratios the brand actually uses
- Negative space: how much, and where it sits
- Symmetry or asymmetry; leading lines; horizon placement
- ⭐ **Whether space is reserved for copy**, which is the most practically useful thing in this section

### 3. Subject styling

How people and products are presented.

- Wardrobe: colours, formality, era, whether it is neutral or branded
- Hair, skin, expression register: candid or posed, smiling or neutral
- ⭐ Casting read: age range, energy, whether subjects look professional or real
- How the product is held, worn or placed

### 4. Imagery

What is depicted, and what never is.

- Recurring settings and environments
- Recurring props and materials
- ⭐ **What is absent.** A brand that never shows faces, never shows outdoors, never shows a second product
  is defined by those absences, and a generator will happily add them

### 5. Style

The photographic and rendering treatment. ⭐ **The most generator-actionable section.**

- Palette: primary and secondary colours, named
- Lighting: direction, hardness, colour temperature, time of day
- Camera and lens character: focal length feel, depth of field, distortion
- Grain, texture, sharpness, film or digital character
- Grading: contrast curve, saturation, any colour cast

⭐ **Course 802's vocabulary lists belong here** — its lighting terms, film stocks, lenses and composition
terms are exactly this section's raw material. See `aca-write-ai-image-prompts`.

### 6. Signature details

⭐ **The section that makes output recognisable rather than merely competent.** The small, repeated things.

- A recurring highlight, reflection or shadow shape
- A material that always appears: brushed metal, linen, wet stone, condensation
- A consistent surface the product sits on
- An edge treatment, a border, a consistent vignette
- ⭐ Anything a regular viewer would notice was missing without being able to name it

⚠️ **This is the section a single extraction pass usually leaves thin**, which is why the course runs it
twice.

---

## ⛔ Observed against declared

**Mark every attribute as one or the other.**

| | Where it came from | How it fails |
|---|---|---|
| ⭐ **Observed** | Read off the supplied images | Fails if the image set is unrepresentative |
| **Declared** | Told to you by the brand, or taken from guidelines | Fails if the brand's guidelines and its actual photography disagree, which is common |

⛔ **Never blend them silently.** When generated output looks wrong, the first question is which kind of
attribute misled it, and an unlabelled profile cannot answer that.

---

## What the profile does not hold

⛔ **The product's fine details.** Those are carried by the input image and the keep-this-change-that clause,
not by the profile:

> "keep colon this exact product visible and preserve define details"

⚠️ *"preserve define details"* is the transcript's rendering of *preserve fine details*.

⭐ **Say this explicitly in the emitted profile.** The failure mode is a good profile producing on-brand images
with wrong packaging, and whoever uses it next needs to know the profile was never responsible for that.

---

## ⭐ The system prompt that consumes it

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

## ⭐ The swap test

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
