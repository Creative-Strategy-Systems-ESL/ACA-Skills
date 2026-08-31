# Provenance

## Source

**Ad Creative Academy** — Course 803: *The Creative Automation Workshop: How to Build Your Own AI Ad Engine*
(800-Level). 1h 34m 13s, 6 modules. **Rory Flynn**, founder of Systematiq Ai, and **the same faculty member
who teaches Course 802**.

**Its worksheet:** a one-page setup guide for the workflow template, listed by ACA as this course's
downloadable asset.

**The six modules, with ACA's own durations, and how they map onto the recording:**

| ACA's module | The recording's section |
|---|---|
| 1. Introduction to AI Design Workflows (24m 26s) | Video 1, Workflow Intro |
| 2. Building Your First Workflow Part 1 (21m 15s) | Video 2, Basics |
| 3. Building Your First Workflow Part 2 (16m 14s) | Video 3, Workflow Ext |
| 4. System Prompting (7m 50s) | Video 4 |
| 5. Batch Processing (18m 39s) | Video 5 |
| 6. Iteration Generator (5m 49s) | Video 6 |

⭐ **A clean one-to-one mapping**, which is unusual in this programme: most courses' published module lists do
not match their recordings.

---

## ⛔ ACA's own file contains the transcript twice

**Measured, not assumed.** The file ACA sent carries its entire content **two times over**:

| | |
|---|---|
| First copy | **19,709 words** |
| Second copy | **19,736 words** |
| Shingle overlap | ⛔ **99.7%** |
| Fragments unique to the second copy | **40, every one of them an artifact of a doubled heading line** |

⛔ **Not one word of content exists only in the second copy.** The six video headings appear twice at the
start of the second block, which is what creates the 27-word difference and all 40 "unique" fragments.

⚠️ **The duplication is ACA's, not an extraction error.** Their re-sent file carries it identically, at the
same overlap, with the same 40 heading artifacts.

⛔ **So the real length of this course is about 19,700 words, not the ~39,150 a naive word count returns.**
Any claim that this is the longest input in the programme is wrong: **Course 802, at 29,461 words, is.**

---

## ⚠️ The course number

**Older material in this library files this course under a 502 code.** ACA publishes it as **803**, and three
things confirm that: ACA's live course listing, the filename ACA itself sent (*803 - Rory Flynn - The
Creative Automation Workshop*), and arithmetic — the 800-Level's stated total of 04:23:51 equals
31:06 + 2:18:32 + 1:34:13 exactly, and its stated 19 lessons equals 4 + 9 + 6 exactly.

⚠️ **Course 802 has the same problem** and worse: Rory says *"welcome to course 502"* out loud on that
recording. The 502 codes are a superseded numbering.

⚠️ **The recording also calls itself a bonus module**, not a course: *"We are going to go into **a little
bonus module** on workflow building"*, and the material was filed here as a bonus to Course 502 before ACA's
listing settled it as a numbered course. ⭐ **It is a course.**

---

## ⭐ How this course sits against Course 802

**Same teacher, and this is the only place in the programme where one course explicitly cites another:**

> "So think about **the image deconstruction model that we did** in terms of taking an image, turning it into
> its requisite parts, and then rebuilding it."

⛔ **But it also partly supersedes 802**, and that matters more than the citation:

> "We did we went through a little bit of the Laura training stuff, which is how do I take one singular
> product and do sort of train a model on that ... **these image models make it a lot easier** ... And it's
> **actually relatively easy in comparison to what we did with the Laura training stuff.**"

⭐ **Read plainly: the 39 minutes Course 802 spends on LoRA training is, by its own teacher's later account,
the hard way to get consistency.** In-context editing models do much of it in natural language.

⚠️ **This is not a reason to skip 802.** Training still wins where a product must be pixel-identical across a
catalogue, and 802's prompt formula, asset cloning and camera vocabulary are all still load-bearing here.
**But if someone has one week, this course's method reaches a usable result faster.** ⛔ **Neither ACA's
curriculum nor either course says this**, and a reader taking the courses in order will spend the week
before finding out.

### ⚠️ And the two courses appear to contradict each other on prompt length

| Course 802 | Course 803 |
|---|---|
| ⛔ *"don't start with full sentences"*, *"use stronger keywords or phrases"* | ⭐ *"Each prompt should aim to be highly descriptive. **Minimum of 250 to 350 words**"* |

⭐ **They are reconcilable and the reader needs to be told how**: 802's token style is written for Midjourney,
which weights tokens; 803's word count is written for natural-language models, and Course 802 itself says Flux wants
natural-language prompting with longer prompts. **The rule is the target model, not a
change of mind.** ⚠️ **Neither course states this**, so a reader who takes both at face value will conclude
one is wrong.

---

## ⚠️ The worksheet, and what it is not

ACA's listed asset for this course is a **one-page, 131-word setup guide**, not a fillable worksheet. It
gives three steps:

| Step | What it says |
|---|---|
| **One: Set Up** | Open the template, then *"Click Duplicate to create your own workspace,"* and *"connect your accounts and complete setup."* ⚠️ (two fragments: the guide is a two-column layout and its sentences interleave) |
| **Two: Product Image Generator** | Upload your product image, add a prompt or style direction, and ⭐ *"Generate 20 images (10 brand, 10 experimental)"* |
| ⭐ **Three: Create a Visual Brand Profile** | Open ChatGPT, upload 10 brand images, ask it to create a visual brand profile. Suggested prompt, reassembled from the interleaved columns: *"Here are 10 brand images. Create a"* / *"visual profile I can use to generate new"* / *"images in the same style."* |

⭐ **Step Three is the one that matters**, and it is corroborated by the recording, which calls the profile
*"the only thing that really needs to change"* to point the workflow at a new brand. **Two sources, same
artifact.** That is why it has its own skill: `aca-build-visual-brand-profile`.

⭐ **The counts line up too:** the guide says generate 20 images from 10 brand references; the recording's
batch system generates ten prompts per run and says *"It's already going to create ten new prompts for you."*

⚠️ **The guide is named in ACA's curriculum sheet but nowhere in the recording.** Measured: the string
*"workflow template"* appears **zero** times in the transcript. ⛔ **And the guide's first instruction is to
open a hosted template that this library does not hold** — so step one cannot be followed from the shipped
material alone. The recording's build-it-from-scratch walkthrough is the fallback, and it is complete.

---

## ⚠️ Transcription artifacts

The recording is a machine transcript and it mishears the tool's name constantly. **This skill quotes the
source verbatim and flags each one in place.**

| Real name | What the transcript says |
|---|---|
| **Weavy** | ⛔ *"YV"* · *"CV"* · *"weave"* · *"weaving"* · *"we've"* · ⭐ *"Wi-Fi"* — **never spelled correctly** |
| **LLM / LLMs** | *"LM"* · *"LMS"* · ⭐ *"The line"* |
| Reve | *"Rev"* · *"Reeve"* |
| Seedream | *"sea dream"* · *"seed see dream"* |
| Higgsfield | *"Higgs field"* |
| Recraft | *"re Craft"* |
| Runway Gen-4 | *"runway gen for"* |

**Other artifacts quoted and flagged in place:** *"provide the problem"* for *provide the prompt* ·
*"preserve define details"* for *preserve fine details* · *"thrusted the camera"* for *thrust toward the
camera* · *"created art director"* for *creative art director* · *"3040 of these"* for *30 or 40 of these* ·
*"precursor to agent"* for *agents* · *"a less prompt"* for *a list: prompt*.

⚠️ **Nano Banana is the exception:** it is rendered correctly and is a real product name, however unlikely it
reads.

---

## The numbers, and what each is worth

| Claim | Status |
|---|---|
| **Generate ten prompts per run**, split on an asterisk | ⭐ Mechanism, not a benchmark. It works because the delimiter cannot occur in the content |
| **20 images: 10 brand, 10 experimental** | The worksheet's instruction. ⚠️ No rationale given for the split |
| **10 brand images** to build a profile | ⭐ Stated in both sources. ⚠️ It matches Course 802's 10-to-20 band for object-model training, which is weak corroboration from a different mechanism |
| **250 to 350 words** per prompt | ⚠️ *"typically like a good range for all of the image generators"* — his practice, no source |
| ⭐ *"3040 of these at a time"*, up to 100 | ⚠️ Illustrative, not a recommendation. The transcript renders *30 or 40* as *"3040"* |
| *"maybe five minutes"* for a full run | ⚠️ Tool-state, and the fastest-dating claim in the course |
| **"all of 30s"** for a single edit | ⚠️ Tool-state |

⛔ **There is no performance claim anywhere in this course.** No CPA, ROAS, CTR, hook rate, or win rate. It
never says the assets perform; it says they exist faster. ⭐ **That is a more honest position than most of the
programme takes**, and it should not be quietly upgraded.

---

## ⚠️ Named brands and tools

**Brands used as examples:** Athletic Greens · a card issuer · a menswear denim brand · Red Bull · C4 ·
Barkbox · a skincare brand. ⚠️ **No permission or client relationship is stated for any of them in this
course**, unlike Course 802 where he is careful about it. ⭐ **Course 802's disclaimer still applies** — *"try
to only do this on your brand"* — and this course's technique is the same technique.

**Tools named:** Weavy · Flora / Fauna · ComfyUI · Figma · Photoshop · Nano Banana / Gemini 2.5 · ChatGPT ·
Flux · Flux Context · Reve · Seedream · Higgsfield · Recraft · Mystic · Runway · Runway Gen-4 · Kling.

⛔ **Rule 9 applies with unusual force here.** This is the most tool-dependent course in the programme: every
walkthrough runs inside one third-party node editor, which was mid-acquisition at recording. ⭐ **The manual
fallback is the course's own argument** — the three core skills are explicitly tool-independent, and the
build can be reproduced by hand in any node editor or by chaining an LLM and an image model directly.

⚠️ **No commercial relationship is disclosed**, and he is a vendor of AI services.

---

## What is quoted and what is organised

**Everything substantive is Rory's, quoted directly** — the three core skills, the keep-this-change-that
formula, all six parts of a system prompt, both worked system prompts, the array and delimiter mechanism,
app mode, and the visual-brand-profile swap.

⭐ **Every quotation has been checked character by character against the transcript**, with compressions
marked by an ellipsis. Where the recording mishears a name, the mishearing is preserved and flagged.

**This skill's organisation, not ACA's:**

- Splitting the course into the three skills and then the build, rather than following its six videos
- Rendering the six system-prompt parts as a table with his worked example beside each. ⚠️ **He lists them in
  speech and never numbers them**
- The two-way comparison of text iterator against list selector
- The expose-versus-hide table for app mode
- Collecting the tool-name artifacts into one place

**This skill's additions, drawn from the material rather than stated by it:**

- ⛔ **The measurement that ACA's file duplicates itself**, and the corrected word count
- ⛔ **Naming the 802 supersession plainly**, and saying what it means for someone with one week
- ⛔ **Reconciling the token-prompt and 250-350-word instructions** across the two courses. Neither course
  attempts this
- ⭐ **The point that the delimiter must be a character the content cannot contain**, which is why an asterisk
  works where a comma would not. He changes the setting and never says why
- ⭐ **Naming "hide the system prompt" as an engineering instinct**, not a UI preference: the system prompt is
  the tool's logic, and exposing it undoes the course's whole purpose
- ⭐ **The observation that "pick the winners" is Course 702's unpredictability argument** arriving through a
  different door
- ⭐ **The note that the worksheet's step one cannot be followed from the shipped material**, and that the
  recording is the working fallback
- ⚠️ **Promoting "these are raw assets" from a passing remark to a scope statement**, since it is the only
  place the course bounds its own claim
- ⚠️ **Flagging that this course names client brands without the care Course 802 takes**

---

## ⚠️ How old this material is

**ACA stamps no recording date.** Received into this library in **2026-W31**, a "no later than".

⭐ **Internal evidence dates it after Course 802**: it treats in-context editing models as the current shift,
names Gemini 2.5, and describes the node tool as *"joining Figma"* but not yet integrated.

⛔ **What dates fastest:** every tool name, the node editor's UI, every model in the picker, the *"five
minutes"* and *"30s"* timings, and the claim that in-context models are new.

⭐ **What is durable:** the three core skills, keep-this-change-that, the six parts of a system prompt with
limits as the critical one, everything-must-be-connected, test-before-batch, the delimiter mechanism,
hide-the-logic, and *"we have to think in batch"*. ⚠️ **None of these depends on a tool**, which is the
argument the course makes for itself.

## Scope

Building the machine. ⛔ **No metric, benchmark or performance claim appears anywhere.** What to test is
Course 602; what the numbers mean is Courses 402 and 701; what the ad should say is Course 401; how much
creative an account needs is Courses 601 and 703. ⚠️ **And what comes out is raw** — *"all of these raw assets
that you're going to have to sort of doctor up in your own way."*

## Credit

Ad Creative Academy's curriculum and Rory Flynn's teaching are their own work. This skill organises that
material for reference; it does not originate it.
