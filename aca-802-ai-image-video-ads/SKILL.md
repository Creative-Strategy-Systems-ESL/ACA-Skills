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
| Why did my prompt give me something generic? | **How the generators actually work** (below), tokens and weighting |
| How do I write a prompt that works? | **Prompting: the formulas** (below) |
| How do I make AI images that look like *our* brand? | **Asset cloning** (below) |
| How do I get the same product in every shot? | **Training custom models** (below) |
| How do I turn a still into video? | **Prompting: the formulas** (below), image-to-video |
| Which tool should we use? | **How the generators actually work** (below), the trade-off |
| Where did these claims come from? | ⚠️ **Provenance** (below) |
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

1. **Explain diffusion and token weighting** from **How the generators actually work** (below), including the removal
   experiment. ⭐ The lesson is that you choose whether *you* specify a slot or the model invents it.
2. **Give the eight-slot image formula** in **Prompting: the formulas** (below), condensed-first.
3. **Add the six-slot video structure** and the nine camera motions, same file, plus the interaction clause
   that stops output reading as AI.
4. **Teach asset cloning** with **Asset cloning** (below) when the brand has tired photography. ⛔ Carry
   the disclaimer: their own brand only. ⚠️ And step 2 of the five fails on purpose — the LLM pass is the fix,
   not polish.
5. **Only reach for model training** in **Training custom models** (below) when a product must be identical across
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
| **How the generators actually work** (below) | Diffusion, tokens, weighting, the video pipeline, and choosing a tool |
| **Prompting: the formulas** (below) | The rules, both prompt structures, the nine camera motions, the three video modes |
| **Asset cloning** (below) | Reverse-engineering a brand's visual signature into variants |
| **Training custom models** (below) | LoRA training for products, characters and styles |
| **Provenance** (below) | ⚠️ **Read before quoting any number or tool claim.** Includes the course-number conflict |

---

## How the generators actually work

⭐ **Read this before the prompting file.** Rory spends the first third of the course here on purpose:
someone who understands the mechanism debugs their own prompts, and someone who does not just rerolls.

⚠️ **Quotes here are verbatim from a spoken transcript**, so they carry speech as spoken. Where the
recording renders a tool name oddly, **Provenance** (below) lists what the source says against what
the tool is called.

---

### The equation the whole course rests on

> "This is a basic equation that I sort of live my life by now in AI: essentially **a clear and direct
> prompt will equal a clear and direct output**, an ambiguous prompt will equal an ambiguous output, so
> **the more detail you put in a prompt, the better detail you're going to get in an image**"

**His demonstration**, worth reusing because it lands in seconds. First the vague version, *"let's just
picture a woman in the park"*:

> "I can guarantee you that you and I are thinking different things because that statement is ambiguous
> ... we're not talking about ... time of day it is what park it is what she's wearing what else is
> going on"

Then the specific version, *"a woman sitting in a New York City park during a cold winter night wearing
cozy clothes and a single spotlight shines on her"*:

> "I feel like we're probably **much closer to the same idea** than we were just woman in a park right
> so **this is how these image generators work as well**"

⭐ **Run this on anyone who says AI images are unpredictable.** The prompt was unpredictable first.

⚠️ **He shows the same thing on real output**: the vague prompt returned four wildly different women,
*"all varying different perspectives shots things of that nature"*, because *"what we said was ambiguous
in the same way each one of you were probably thinking something different than me"*.

---

### Diffusion, in his terms

> "how it works is **they upload images into the machine learning brain**. All those images get turned
> into **a jumbled mess of noise**. And then when you prompt it, **the image is recalled**. So, it takes
> all those ideas and all those training images and **diffuses them together**. That's a diffusion
> model, right?"

**Tokens are the unit:**

> "Basically through tokens. **They're the building blocks** the entire process. They can be **text,
> words, or images**, and they have **a huge influence on the output** of the image."

⚠️ *"the building blocks the entire process"* is what the recording says; the missing word is the
transcript's, not an edit.

---

### ⭐ The token-weight law

The single most useful mechanical idea in the course.

| Prompt length | Emphasis per token | Style | Control |
|---|---|---|---|
| **Shorter** | ⭐ **More** per token | Stronger style for each | ⛔ **Less** control of output |
| **Longer** | Less per token | Moderate style for each | ⭐ **Stronger** control |

In his words: *"when you use a shorter prompt, what's happening here is **you have more emphasis per
token**. You're gonna have a stronger style for each token, but you're gonna have a little bit less
control on what's outputted."* And going longer: *"there's gonna be **less emphasis per token** ...
You'll have a little bit stronger control on the image output, but **everything's gonna be represented
a little less**."*

**His worked example.** Four tokens: *"orange Jeep, snowy environment, 35 millimeter film"*

> "When we look at how that might break down, **it might be 25% for each**. So, you might have 25%
> orange, 25% Jeep, 25% snowy environment, 25%, 35 millimeter film aesthetic."

Then he adds *New York City, snowman, icicles, spotlight*:

> "So, instead of being 25% of the image, **they might be 12.5%**, right? Again, **not an exact
> science**, but we'll see how this looks."

**And the result is visible:** everything asked for is present, but *"the icicles are very small, they're
there, the spotlight on top of the Jeep"*.

⚠️ **He flags his own analogy as an analogy**, twice: *"you don't have to take the 25% analogy, verbatim,
just a good representation of how it works"*. Carry it the same way.

#### ⭐ The removal experiment, which is the real lesson

He then deletes *snowman* and *New York City*, removing the environment entirely:

> "Number one, **it creates an environment, because we didn't add it, we can't just have it in the black
> void of space**, right? If we said things like icicles, it'd be very weird if there was just icicles
> just floating in space with a car. So, **it's gonna create an environment that fits that**."

And the remaining tokens gain weight:

> "you see the icicles that immediately jumps out, because now there's less tokens, **meaning it has
> more weight on it, it's much bigger in the image**"

⛔ **This is the structural fact behind everything else in the course.** You never choose whether the
image has lighting, an environment or a composition. You only choose **whether you specify them or the
model invents them.**

---

### How video generation differs

> "video generation really similar to image generation, **but more complex. There's more variables**.
> There's a lot more things going on in a video than there is in an image. **There's a lot more things
> they can screw it up to.**"

**The pipeline:**

| Stage | What happens |
|---|---|
| 1. Training data | *"you have your training data, which is your video set"*, uploaded into the model |
| 2. Prompt | ⭐ *"when you prompt what's being recalled is **the motion**"* |
| 3. Frame generation | *"it's going to generate most of the time **24 frames a second**. So if you have 10 second generations, **about 240 frames**"* |
| 4. Interpolation | *"we just take all those random frames and sort of **combine them together**"* |
| 5. Output | |

**Training works by tagging:**

> "when videos are uploaded, **they're basically tagged and that's how the machine learn**. So when I
> put this video in, I might use like, what is the action? It's, you know, an arcing shot. What is the
> environment? It's outdoors. It's on mountains. **So all these little tags get applied to the videos.**"

#### ⭐ The X factor is motion

> "Really **the X factor in all this is the motion recall. That's what makes everything generate.** So
> what does that tell us? That tells us that when we're prompting, basically **everything is gonna be
> focused around the motion** because that's the thing that it is all working around."

**How it learns motion:** *"if a character is walking, basically what it's going to do, it's going to
strip that aesthetic away, just the baseline functionality of the walking."* Camera motion is learned
the same way, and *"it'll track the camera motion, we'll sort of understand the depth and perception of
the subject"*.

⭐ **This is why a video prompt that only describes a scene produces a still that drifts.** The model is
looking for motion to recall and you gave it none.

---

### ⭐ The creativity-control trade-off

> "**what you gain in creativity, you lose in control. And when you gain control, you lose a little
> creativity.** So there's a balancing act. And this is the way it is with the image generators with the
> video generators."

**How he splits the two image tools:**

| | Midjourney | Flux, inside Krea |
|---|---|---|
| **Best at** | ⭐ *"visual firepower"*, *"lifestyle currently"*, storyboarding, *"a lot of internal usage, because it's quick and good"* | ⭐ **Consistency.** *"we use this a lot for consistency, because you can train models and replicate characters or styles"* |
| **Why** | *"it's the ultimate sandbox"*, and *"they have so many creative controls"* | *"if we have things that need to be replicated exactly ... it gives us that precise control"* |
| **Trade** | Less precise control | *"you lose a little bit of the visual firepower of mid-journey"* |
| **Reach for it when** | Expressing an idea, exploring, static that must pop | ⭐ **A product must look identical every time** |

⚠️ **Midjourney cannot train custom models**, which is the whole reason the course moves to Flux for
product work: *"that's something that mid-journey does not have the capabilities to do yet, probably will
come, keep an eye on that."*

**And on prompt style, the two differ:** Midjourney takes broad-concept token prompting; Flux *"likes ...
more natural language prompting"*, so *"the writing prompts gets a little bit longer"*. ⭐ **Same building
blocks either way** — *"It's essentially the same thing. You're just adding more words."*

---

### The video tool stack, with his strengths and weaknesses

⚠️ **Every name and version here dates fast.** Carry the reasoning, check the tool. Names appear as the
transcript renders them, with the real product name alongside.

| Tool | What he says it wins on |
|---|---|
| **Kling** (*"Cling"*) | ⭐ *"which I use probably the most often because it's predictable"* — *"the coherence is very strong on the prompting and the control is very good"*, and the only one with a negative prompt |
| **Veo 2** (*"Veyo 2"*) | ⭐ *"ultra realistic. It's super, super indistinguishable in certain cases from real life."* |
| **Runway** | *"a production sort of masterpiece"* — aspect-ratio expansion, and *"an Act 1, which is an advanced motion capture"* |
| **Minimax** | *"super creative and it has like a nice little streak to it"* |
| **Sora** | ⚠️ *"complex and complicated, but it's super powerful"* — *"flopped a little bit on release"* |
| **Luma Labs** | *"radically updating consistently"* |

> "**there's not one that head and shoulders above another.** They all have their different uses and
> most of them are multi purpose."

⭐ **The tool-agnostic argument he makes for skills over tools:**

> "**you really only need baseline skills. You need fundamentals, not just tools.** Right. Like if you
> understand the process of how these things work, how you can leverage them, **the tools are
> interchangeable.**"

**The three he says you need:** an **LLM** (*"chat, G.P.T., Claude, Lama"*) · an **image generator**
(*"Mid-Journey, Flux, Leonardo"*) · a **video generator** (*"Cling, Runway, Sora, Minimax"*) · plus niche
tools for sound and music, which *"become way less of a lift"*.

⭐ **And on the video generators specifically:** *"if you have skills with one, you can basically use them
all."*

---

### ⚠️ The cons, in his words

He returns to these repeatedly, and a skill that drops them misrepresents the course.

- **Video is glitchy.** *"still glitchy"*, and *"You're going to have to do multiple generations."*
- ⛔ **It gets expensive.** *"they cost more than the image generators. You get less value out of them
  from a ... generation standpoint."*
- ⛔ **Resolution is the real ceiling.** *"Majority of it comes out at 720p right now. 1080p you'll get
  out of some of the models, but they really still need upscaling to get them to a higher resolution,
  higher clarity."*
- ⭐ **The missing tool in the entire stack:** *"a video upscaler that can not just only increase the
  resolution, but do a creative upscaling as well. So really add fine grain detail. So we get rid of
  that sort of AI plasticness or AI fuzz."*
- **Sports is the hardest thing in AI.** *"there's no replicable motion because everything is so
  different"*, and ⭐ *"I promise you I've tried to get a basketball going into a hoop maybe 800 times
  over the last two years. This is about as close as I get"*.

**His workaround, which is a real strategy:**

> "We use it in a smaller format, right? Also in a shorter format so you don't have these long
> generations with opportunities for morphing or things to go wrong."

And: *"the quicker the cut, the less scrutiny there is"*, because *"the smaller it is ... you're just
going to have less details people see, it's going to be less scrutiny"*.

⭐ **Hybrid is explicitly allowed:** *"It doesn't have to be, again, all AI ... You can use real footage
with AI footage, make it a hybrid approach, something that we can do just to amplify what we're doing
already, not reinventing the entire wheel."*

---

### The adoption ladder

Useful for diagnosing whether a team's problem is a prompt or an operating procedure.

| Stage | What it looks like |
|---|---|
| 1. **Discovery** | *"You find tools, start using them, get excited, really start to push the envelope on it a little bit."* |
| 2. **Adopt** | *"We start to use this in our daily workflow, solving certain problems"* — ⚠️ *"But mostly, you're doing it on an individual level."* |
| 3. **Operationalised** | ⚠️ *"They're all using the tools, but they're all using it in their own way. They're all using it in a very siloed approach. **There's no organization around it.**"* |
| 4. **Systematised** | *"we start to build SOPs around it to make it more systematized so **the outcomes are more predictable**"* |
| 5. **Automated** | *"If you've heard the term automated agents, that's what's coming ... it's taking those SOPs and those workflows and then automating it."* |

> "I would say **majority of people are at stage two or three.** Again, I might be overselling there"

⭐ **Stage 3 is the trap and it is where most teams are.** Everyone using AI, nobody using it the same
way, so nothing compounds. The fix is not a better tool.

⭐ **And the goal he attaches to stage 5 is worth keeping**, because it is the opposite of removing
people: *"the idea is to get from point A to point B in a quicker fashion ... **so that you can then put
your own human creative at the end of it**."*

## Prompting: the formulas

⚠️ **Quotes are verbatim from a spoken transcript.** Where a word looks wrong it is the recording's;
**Provenance** (below) lists the tool names and the one number that are transcription artifacts.

---

### The five rules

⚠️ **He frames these as loose, and means it:** *"these are some loose guidelines, right? Take this for
what it is, you do not have to use this step by step, you don't have to use this verbatim, this is just
like the way that I like to do it."*

| # | Rule | In his words |
|---|---|---|
| 1 | ⭐ **Don't start with full sentences** | *"start with what I like to call **broad concepts, prompting**, meaning put a number of tokens in there, see how it comes out, iterate along the way"* |
| 2 | **Use strong keywords** | *"you can separate those by commas or periods, it doesn't really make a difference, **just a way to separate ideas**"* |
| 3 | ⭐ **Use powerful language** | *"**big versus enormous, enormous sounds better**, like colorful versus vibrant, vibrant sounds better, but **they also produce better imagery within the tool**"* |
| 4 | **Focus on one subject to start** | *"don't go in there and try to add a bunch of different people and a bunch of different props and things of that nature, **add those as you go along**, because you don't want it to be too much too soon"* |
| 5 | ⭐ **Tell it a story** | *"just like you talk to your friends, like you're living a memory, **how does it look, how does it feel, what was going on, who was around, what is the mood like, what is the atmosphere like**"* |

⭐ **The concentrated-juice method**, which is rule 1 made concrete:

> "if you're familiar with what cranberry juice concentrate is or orange juice concentrate, just like
> the really distilled form of it, but you add water to it to create the juice. So **I like to create
> that very condensed form first, and then I'll add water and add details to it as I go along**."

> "basically **a prompt is a story**. So if you think about it that way, you can start to create much
> easier."

---

### ⭐ The photographic elements

For photorealism, which is what advertising usually needs: *"a lot of times, especially in the
advertising space, we need things to look real"*, and *"mid-journey responds to photography terminology
very well"*.

⛔ **The rule that makes this list matter, quoted in full:**

> "essentially, **every one of these elements, they have to be in an image**. So if we look at all of
> these, **if you take one out, the image doesn't really exist** or mid-journey is not gonna know what
> to do, so **it's gonna add it in there**. The same with any other image generator."

| Element | What it decides |
|---|---|
| **Subject and action** | *"Who's in it, what they're doing"* |
| **Environment** | *"where it takes place"* |
| **Composition or shot type** | ⭐ *"there's a big difference in storytelling from a close-up shot versus a drone shot"* |
| **Mood and emotion** | *"fairly good use of your prompting here, because **it tells the story better**. It sort of molds the scene"* |
| **Camera and lens** | ⚠️ *"there's a lot of debate online here between whether specific cameras and lenses work in a prompt. Personally, I like to use them"* |
| **Film stock** | *"to craft a specific look"* |
| **Lighting** | ⭐ *"super essential. There's lighting in every single image. **If there was no lighting, you just have a black image**"* |
| **Colours** | *"What are the colors looking like?"* |
| **Details and modifiers** | |

**On cameras and lenses, why they work:** *"naturally there's a different visual signature from something
like an iPhone photo to a Polaroid image, right, they have two very specific looks."* And on lenses,
*"there's something different between ... eight millimeter super wide lens and then a 200 millimeter long
distance lens, right? They produce a different visual signature."*

⭐ **If you don't know the terminology, he says to outsource it:** *"That's something you can use other
LLMs for, like Chat GPT, help me come up with some specific cameras, or help me find some really high
quality lenses that would work with this image."*

---

### ⭐ The image prompt formula, eight slots

> "we do here to basically create a simple prompt formula, is **we take those photographic elements, and
> we structure them into a prompt**. So **this is how we can do this at scale and do it often**."

| # | Slot | Example value |
|---|---|---|
| 1 | **Photo type** | cinematic still |
| 2 | **Shot type or composition** | *"Is it a closeup? Is it far away?"* |
| 3 | **Subject and action** | a haggard man sitting |
| 4 | **Environment** | a grungy East Village dive bar |
| 5 | **Colour scheme** | brown and burgundy colors |
| 6 | **Camera details** | 35 millimeter film |
| 7 | **Lighting** | backlight |
| 8 | **Composition, and anything additional** | off-balance composition, loneliness |

**His worked prompt, assembled:**

> "cinematic still of a Haggard man sitting in a grungy East Village dye bar, brown and burgundy colors,
> 35 millimeter film, backlight, off-balance composition, and loneliness is our emotion"

⚠️ *"dye bar"* is the transcript's rendering of *dive bar*, and he confirms the meaning in the next
breath: *"If you're not familiar with the East Village in New York City, this is what a dye bar looks
like. You see the paint chips on the right side of the wall."*

⚠️ **He undersells it deliberately:** *"Pretty simple, seems like a lot of random ideas put together. But
when we run it, we get something that is exactly what we asked for."* Then he audits the output element
by element against the prompt, which is the habit worth copying: *"everything that we listed is available
within the image."*

⭐ **Why eight slots beats a paragraph:** *"So it becomes easy to iterate and play **because you're
controlling majority of the aspects**."* His example: *"I know I listed out my lighting as mid-day
lighting, but it's way too bright, maybe I can just go back in for the iteration process and switch
that."*

---

### ⭐ The video prompt structure, six slots

> "So what does that look like for video here? **It's going to look very similar to what you saw in the
> image ones.**"

| # | Slot |
|---|---|
| 1 | **Shot type** |
| 2 | **Subject and their details** |
| 3 | **Camera motion** |
| 4 | **Direction** |
| 5 | **Mood and atmosphere** |
| 6 | ⭐ **Captured in a style** |

**On slot 6:** *"I like to use a style because a lot of different filmmaking type styles that you can
utilize here and **tailor it to your brand** or the brands that you're working on."*

**His worked prompt:**

> "a handheld shot of a man modeling khaki pants in a studio environment ... Then the camera follows the
> man as he moves, as he models the pants in various poses. The camera stays fixed on his pants as he
> does a full 360 degree turn. The scene is playful, reminiscent of a professional fashion photo shoot
> shot in cinematic 4K."

⭐ **Why he claims it ports across tools:** *"this kind of problem structure is going to work in just
about every video generator **because you're covering all your bases**."*

⚠️ *"problem structure"* is the transcript's rendering of *prompt structure*; he uses both in the same
passage.

#### Two extra rules for video

**Write in natural language**, and be more detailed than for images: *"You need to be a little bit more
detailed because **it can take your words and interpret them very wrong** if you're not doing it that
way."*

⛔ **Camera and subject motion are the load-bearing parts.** *"Camera and subject motion are the most
important. That's how the whole scene is developed. Outside of that, you can really start to nitpick on
the lighting and the composition and things like that. **But if you don't have the motion, obviously it
doesn't look like a video.**"*

⭐ **Direction is a separate slot for a reason:**

> "If I don't say the camera's tracking backwards, **if I just said the camera tracks, it could track
> forwards, it could track anyway. We're not really giving it much direction.**"

---

### ⭐ Interaction: the thing that gives AI away

The most distinctive teaching in the course, and the part most likely to be skipped.

> "this is where a lot of times people miss and **I think is probably one of the most overlooked aspects
> of it, is environment and interaction**. When there's video, there's a lot more going on. The way the
> light interacts with everything, the way that the environment interacts with the subjects, like
> **there's a lot of detailed interactions that can make things look real or fake**."

> "this is a way that you can quickly tell that things are AI is when things just **unnaturally interact
> with each other. We don't even subconsciously notice it most of the time, but it's there.**"

**His framing for how to think about it:** *"you're essentially explaining this to a blind person, to
someone who's never seen before. **You really have to take the interaction into account.** What is the
human doing? What is the environment doing?"*

| Miss | The fix in the prompt |
|---|---|
| Running with static hair | *"his hair is flowing in the wind"* — ⚠️ *"It wouldn't just be like static hair that doesn't move."* |
| A person sitting in a river, dry | *"the water drips from his body"* |
| Arms out for no reason | *"holding poles that are anchoring him in a raging river"* — ⭐ *"that's going to describe **the physics of the moment**"* |
| Steam passing through a body | *"as the steam bubbles and flows **around** his body"* — *"We don't want it flowing through his body."* |
| Water flowing the wrong way | *"the stream is flowing towards us"* — *"Because if I don't tell it that, it could just flow the other way, which doesn't make any sense."* |
| Sipping a straw head-upright | ⭐ *"as she tilts her head down to sip from a straw"* — *"you don't have your head, it's totally upright, sipping a straw. It's very odd."* |

> "These little things will make you feel a lot better when you actually get to execute them. I think
> it's very easy to overlook them, but also **this is what makes the difference, these interaction
> pieces, in generating one video or generating 50 to get the one you want.**"

⚠️ **He names his own hardest case:** *"Skateboarding is super hard for AI because there is so much
human-object-environment interaction. The human's connected to the board. The board's connected to the
environment. **But sometimes that board leaves the human and leaves the environment at the same time.**"*

---

### The nine camera motions

> "if you learn the camera motions, **you basically have the tool set that you need to tell the tools what
> they need to do**"

And: *"these nine terms here can save you a lot of stress."*

| Motion | What it does |
|---|---|
| **Static** | *"exactly how it sounds. It's still"* |
| **Panning** | *"moving left to right on a slight bit of an arc"* |
| **Tilting** | *"tilting upwards or tilting downwards"* |
| **Tracking** | *"someone's in motion. You're following them"* |
| **Trucking** | *"you might be walking in parallel and horizontal, going next to someone"* |
| **Arcing** | *"you're coming around in about 180 degree fashion"* — ⭐ *"good for fashion or any sort of modeling type work where you want to get more of the body and more of the face"* |
| **Pedestal or crane** | *"means you're going up or down changing levels"* |
| **Dolly push in / pull out** | *"You're zooming and pulling out the frame so you can see a wider field of depth"* |
| **Orbit** | *"we're going around 360"* |

⭐ **Why they earn their place:** *"you don't have to describe too much of the camera movement. You can
give it those terms and it'll work."*

⭐ **And why motion vocabulary specifically:** *"if we're going back to our X Factor of video, it's
motion. And these are the terms that are really help you get that camera motion to **make it not look so
stale and static**."*

---

### The three video modes

| Mode | How it works | ⛔ Where it fails |
|---|---|---|
| **Text-to-video** | *"you write a text prompt, generates a video"* | *"there's no image reference. So you have to control all the things"* — ⛔ *"consistent characters and styles can be very hard"* |
| **Image-to-video** | *"we create an image, we write a prompt, and then we generate a video"* | ⭐ *"you're basically giving it a halfway mark"*, so prompts run shorter — ⛔ *"a lot of times where it lacks is on extreme motion"* |
| **Video-to-video** | *"a video with a text prompt that you generate a video from"* | *"there's less you can do because the structure of the video is already defined"* — ⛔ *"this video of me walking and then changing to me doing jumping jacks, video to video is not the way to do"* it |

#### ⭐ Image-to-video is where the work happens, and the still decides it

> "**understanding the base image is really the most important piece of this. Probably I'd say 70 80
> percent of doing image to video.**"

**What that means in practice:**

> "if you have a little person standing on top of a mountain and they look like they're a mile away and
> you say like pushing close up on that person's face, like **that's not going to happen. That's way too
> much distance for a camera to travel in AI to get there.** So **you're kind of restricted by your
> image.**"

⭐ **The prompt gets shorter, because the image already carries half the slots:** *"oftentimes when you
create an image, a lot of these things are accounted for like color scheme, lighting style. It's already
accounted for. It's in your image."* What is left is *"shot type, camera, motion, direction, subject,
action and then environment"*.

⚠️ **Unless you are adding something not in the frame.** Then you must describe it, and its colours: *"we
added a little bit more environment description and we added the colors. **Because if I didn't add the
colors, it might not get it.**"* His checklist for that case: *"What is different than the original
setting? What do I have to add? Do the colors change? Does the lighting change?"*

#### ⭐ Bake motion into the still

The best cross-module idea in the course: **prompt the image differently when you know it becomes video.**

> "if there's already motion in the image, **you're giving the video generator about a 50% leg up**"

| Problem | Cause | Fix at image stage |
|---|---|---|
| ⛔ A car that glides instead of driving | Static wheels in the still | *"using things like spinning wheels or motion blur"* |
| ⛔ Boots that refuse to walk | Feet flat on the ground | ⭐ Generate the boot already mid-stride — *"a natural progression is for it to just go down and to keep"* walking |
| A crowd standing frozen | No implied action | *"freeze motion"*, *"cheering"*, and *"this vibacious crowd blurred in the background"* |

> "So I like to **bake in motion** in a certain way. You can basically start the start the process
> halfway, simple tokens like motion blur, freeze motion"

⭐ **And it is a deliberate decision at the image stage:** *"So it is all conscious what we're doing here.
When we know we're going from image to video, this might be different if it was a still, but **I know I
wanted a video out of this. So I have to add the tokens.**"*

⛔ **The debugging rule that follows from all of it:**

> "a lot of times we're talking about sort of troubleshooting in the video space **the images the
> problem** a lot of times if you just can't get something you've run it through all those features **the
> image is usually the problem** so keep testing keep playing keep learning"

---

### Adding text to an image

> "you can add that very simply by just **putting the words you want in quotation marks**"

His example: *"let's just say we wanted the black crew neck sweater with the words USA on the, in
collegiate bold font. If you put quotation marks or open quote unquote around USA, it will read that as
I need to add text."*

⚠️ **One or a few words only.** *"you're not gonna be able to add a paragraph in there if you wanna add
one word or a couple words here and there. That can be really executed well. When you wanna add a full
paragraph of text ... it's probably not gonna look good."*

---

### ⭐ Using ambiguity deliberately

The one place the course inverts its own opening rule, and it is a real technique:

> "When you have this super detailed prompt on the left, **we're trying to get something exact. When you
> don't know what you want, you can use a little bit more ambiguous of a prompt to vary the outcomes**"

His example of a deliberately loose prompt: *"a man is posing with a dramatic thoughtful expression"*.

> "That could go from an image generation standpoint, 50 million different ways, **but that can also be
> good, so we can use ambiguity to our advantage.**"

⭐ **The distinction: precision for replication, ambiguity for exploration.** Both are prompt-craft;
neither is a mistake.

---

### Happy accidents

> "Right at the end, **I did not ask for him to stretch his shirt or stretch his pants, but it's actually
> a nice touch.** So sometimes they'll throw in these little additional accent pieces in the videos that
> can be usable."

> "You have to put on your artist hat, right? When you start to paint a picture, you don't necessarily,
> **if you miss a brush stroke, you don't just scrap the whole painting, you work around it.**"

⭐ **And the setting that controls how often this happens**, in Kling: creativity against relevance. *"The
more creative you're going to let cling take over a little bit on the relevant side. That means you're
going to have more coherence to your prompt. So sometimes **a nice balance in the middle is good. Those
happy accidents happen. We love them.**"*

---

### Negative prompting

⭐ **Kling's differentiator, per Rory:** *"that's the one that's a very big differentiator that clean has.
The other ones don't is this negative prompt feature."*

> "If you're not familiar with negative prompting, **it's basically just what you don't want in the in
> the output.** So I'll typically put in there if I'm doing something that's photorealistic. Like I
> don't want animation. I don't want blur. I don't want distortion. I don't want X."

⭐ *"if you don't want people with tattoos, just put tattoos in the negative prompt. It'll take that. It'll
take it out. It won't generate those."*

---

### The motion brush

For when text prompting cannot get the motion you need.

> "Really what you do is **you highlight something.** The more that be a subject anything **and then you
> select the path.** So as you can see these cars were using them to demo how you can drive through a S
> turn, **which basically impossible in every other. Video generator unless you have motion** brush."

⭐ **Its real use:** *"If you want someone to raise their hand or you want someone to do something very
specific. This is a way to do it. If it's not coming out, you're not getting it via text prompt. You can
go this route."*

⚠️ **And it is the partial answer to the sports problem:** *"Motion brush can help with something like
that. This is about as good as it gets."*

---

### Keyframes

> "basically, it is **you give it a first frame and a last frame, or a first frame only. Or a last frame
> only. It generates before after in the middle.**"

**His examples of what this is for:** *"you go from a blank apartment to an apartment that's filled. Like
that is a great way to sort of show development."* And ⭐ *"We have a first frame of an egg. Second frame is
an egg sandwich, right? Like we're showing basically the origin story of this egg sandwich."*

⭐ **Which makes keyframes the native tool for before-and-afters and transformations**, the two most common
ad structures this technique fits.

## Asset cloning

⭐ **The most transferable idea in the 800-Level.** Course 803 generalises it into a named skill,
"deconstruction", and calls it one of three core AI skills. This is where it is taught concretely.

⚠️ **Quotes are verbatim from a spoken transcript.** The recording renders Midjourney as *"mid-journey"*
and ChatGPT as *"chatgbt"* or *"chat GBT"*; see **Provenance** (below).

---

### The problem it solves

> "You're always gonna need multiple ad angles, fresh creative, and of course, subtle variants, right?
> Now, the average media buyer, unfortunately, a lot of times **working with fatigued assets**, stuff you
> used a million times, just a small variety of them, and then the static can tend to be subpar. **A lot
> of brand photography is recycled, it's not the best, it doesn't turn over that often.**"

⛔ **The arithmetic that makes this urgent**, and it is the closest thing to a volume argument in the
course:

> "you have to hire the photographer, you have to do the photo shoot. From there, then it's not even
> about that, you have to go through revisions, and you have to select the winners, and **you might end
> up with 100, 200 great images**, but if you're in a certain space that we are, performance marketing,
> **you might blow through those in a month**, and then it's like back to the drawing board, but **you
> might not have that accessibility** depending on the brand"

⭐ **Cross-reference worth making:** Course 601's spend ladder and Course 703's five variables both put
required creative volume well above what one shoot produces. This is the supply-side answer to the
number those courses generate.

---

### ⛔ The disclaimer is part of the method

> "I put this in here as a disclaimer, **try to only do this on your brand, don't go do this to other
> people's brands**, but again, this is all what's possible and how you can think about it."

**Carry this every time the technique is used.** It is Rory's own line, it is unambiguous, and the
technique works just as well on a competitor's imagery, which is exactly why he says it.

---

### What it is

> "Fun name, just made it up, don't even, there's probably a lot better words for it, but essentially
> what we're doing here is **we're reverse engineering images so that we can have consistent imagery that
> are brand relevant, and then we can replicate them into infinity**, right?"

And the goal: *"the goal of doing this process is to really **break down an image into its DNA
components**."*

**His analogy:**

> "if you had a pizza, what makes up pizza? What are the ingredients? You have your dough, you have your
> mozzarella cheese, and you have some sort of tomato sauce, marinara sauce, whatever you might be
> putting on it, right? You have these three ingredients. So **once you've broken them down, you can
> rebuild that, and that can be a calzone, that can be something else. But once you have the
> ingredients, you can make whatever you need.**"

> "we'll take something like a brand asset, which is our initial image, we'll turn that into these
> **visual building blocks**, so we'll extract it and **turn it into text**, so we can then **rebuild it
> out into a million other images**"

---

### ⭐ The five steps

| # | Step | Tool |
|---|---|---|
| 1 | **Collect our brand assets** | — |
| 2 | **Run them through the `describe` feature** | Midjourney, website or Discord |
| 3 | ⭐ **Fine-tune those prompts** | ChatGPT |
| 4 | **Attach an image to make the prompt stronger** | Style reference |
| 5 | **Iterate the images** | — |

In his words: *"First, we'll collect our brand assets. Two, we'll go into mid-journey, we'll run them
through the describe feature. Three, we'll go and sort of fine-tune those prompts in chat.jpt, and then
four, we'll basically attach an image to it to make this prompt a little bit more strong, and then five,
we'll iterate the images."*

---

### ⛔ Step 2 fails on its own, and he shows it

This is the part most write-ups of this technique omit, and it is the reason step 3 exists.

**What `describe` does:** *"describe does is it turns your image into text. So I would paste my image into
mid-journey website or Discord and run the describe function, and basically it would turn that image into
a text prompt. So what it does is **it provides four prompts, they're all uniquely different**."*

**What happened when he ran them:**

> "these are sort of the results that we get, right? We have these four different sets images, I would
> say, you know, **these look like crap.** Maybe some people out there are like, "Oh, that's cool," but
> personally, I think this **looks like video games or like fine arts, doesn't look anything like what we
> need it to be. So we have to go a little bit deeper.**"

⭐ **He says outright he is showing the failures on purpose:** *"I wanna show you the failures of this stuff
too."* A skill that presents `describe` as sufficient misrepresents the course.

---

### ⭐ Step 3: the ChatGPT instruction

The load-bearing prompt in the whole technique.

> "take this image of the F1 card, we're gonna paste it into chatgbt, and then we're gonna ask it to
> **analyze the image. We want to create a prompt for an AI image generator**, right? We want it to
> **describe it like an award-winning professional photographer in extreme technical details.**"

Then, and this is the join between the two halves of the course:

> "**use this formula to structure the prompt.** We can insert our prompt formula from a couple slides ago
> to help us structure a prompt, and then **include specific camera lens, camera settings, et cetera, be
> very technically specific, use short and powerful keywords and phrases, do not use** full sentences"

⭐ **Why a machine does this better than a person, in his words:**

> "That's the goal, is to take out that detail that **maybe your eye or someone on your team's eye can't
> see** or doesn't have the baseline skills to understand how to describe it."

And on the result: *"That second half of the prompt, **I'm probably never gonna be able to describe it that
way.** It's just great to have Chatgbt as a partner there."*

**What came back on his Red Bull example:**

> "panning shot, Red Bull racing car, indigo and amber, hillside, Canon EOS 1D X Mark II ... 35 millimeter
> style, dappled sunlight, bold contrast with delicate precision, high speed capture, low ISO value wide
> aperture"

⚠️ **And it still was not right:** *"when we run this, we get something better, not great. Like it's still,
it got way more photorealistic, but **that perspective is way off.** Like that's not what we're looking
for. We need something a little bit closer, not aerial."* Hence step 4.

⚠️ *"F1 card"* is the transcript's rendering of *F1 car*.

---

### Step 4: style reference

> "you give mid-journey a reference image and **it'll take that visual signature and apply it to another
> image. So it transfers the aesthetic from one image to the next**"

**What transfers, from his walkthrough:** the lighting (*"you have this backlight, which is essentially a
nice golden hour, sun peeking over a cliff"*), the colour scheme, and the consistency: *"The color scheme
comes in, the lighting comes in. It's very consistent."*

⭐ **And it survives a subject swap:** *"we could take this pistachio gelato and turn it into strawberry or
turn it into a mocha gelato and **keep the same look and texture and feel with a style reference**."*

**The combination is the clone:** *"we take that style reference, we take that image that we first used as a
style reference, we attach it to the new prompt that we had from Chad GBT and then we run it together. So
when we do that, we get this, which is what we call **that asset clone**."*

⚠️ **He is honest that the tool is inconsistent:** *"And again, using style reference can be way easier than
this. **A lot of times it's way harder.**"*

---

### ⭐ What you keep is the prompt

The most important sentence in the module, and the one that stops this being image theft:

> "again, the idea isn't to get this image. **We don't wanna copy this image. We just need the prompt. The
> prompt is the piece** because then we can go and iterate on it, right?"

---

### ⭐ The visual signature, and the three slots you flip

Once the prompt is decomposed into the building blocks, the slots split into two groups.

| Group | Slots | What to do with them |
|---|---|---|
| ⭐ **The visual signature** | Colour scheme · camera details · lighting · composition · modifiers | ⛔ **Hold constant.** *"That's the brand of the image"* |
| **The variables** | ⭐ **Photo type · subject and action · environment** | **Flip these** |

> "that's your visual signature. That's the brand of the image. So **if that stays consistent, all we have
> to do is flip the photo type, the subject and the action and the environment and we can basically create
> anything in that brand style.**"

**His worked variants off one Red Bull image:** *"instead of it being Red Bull Racing Car on a hill, maybe
it's Red Bull Ski-er, maybe it's Red Bull Motorcyclist, maybe it's Red Bull Dune Buggy"*.

⭐ **This is the whole trick.** One asset yields a style, because the brand lives in five slots and the
subject lives in three.

⚠️ **On how close the clones get:** *"these have been produced in Mid-Journey 5.2. So they're older and
it's gotten way better in terms of clarity, in terms of sharpness ... So a lot of times this can be
basically **indistinguishable**."*

---

### ⭐ The mindset, which is why 803 builds on this

> "Why does any of that matter? It's just that **it's a mindset**, right? **Everything is translatable,
> everything is data.** And like, **if you can dissect anything, you can rebuild it.**"

> "It's the same thing with maybe an LLM or chat GBT. **If you see how someone writes a post on social
> media, or if you see ad copy that you like, you can break that down into a structure, repurpose it, and
> then also put your own spin on it.** Right, it's the same thing people do with hooks."

⭐ **Cross-course note, and it is a real convergence:** that is Course 301's reverse-engineering argument
arrived at from a completely different direction, by a different faculty member, about images rather than
scripts. Neither course cites the other. ⚠️ **Course 301 makes the stronger version of the claim** (nothing
is original, so remix deliberately); this one makes it mechanical.

---

### What else the technique unlocks

Rory lists these as downstream uses, all of which reuse the same decomposition:

| Use | How |
|---|---|
| **Mood boards in one prompt** | ⭐ *"can I build a mood board with one prompt? Yes, I just have to go and look up what elements are constituted in a mood board, structured into a prompt"* |
| **Consistent styling across shots** | *"the same image of a drone, of a drone shot of a pickup truck driving on a dirt road. It can be the same as a closeup of a man hugging a dog, right? **It's the same prompt, just little subtle changes**"* |
| ⭐ **Rapid storyboarding** | *"where that leads to is rapid storyboarding, to where you can get from **idea to full concept very quick**"* |
| **Asset expansion** | *"If we were able to take certain images and then reverse engineer how those images looked and then build other images from those images"* — taking a local shoot global |

⭐ **Why the mood board mattered first**, in his own adoption story:

> "it started to bleed into problem solving for us, it was things like **mood boards because we were able
> to save time significantly.** If you've ever done a mood board before, you know, **it takes forever
> sourcing images**, making everything look consistent."

And on why it did not need to be perfect: *"It wasn't didn't have to be production ready. It was just an
idea that we could translate from one person to the next. **Something as simple as a mood board can really
save a lot of time within a business.**"*

**Rapid concepting:** *"If you're ever familiar with the hackathon type environment, **we can take a brief
and go to concept in less than three hours.**"*

⭐ **The underrated benefit he names:** *"Sometimes we've never been able to **fail quicker**, in a sense,
where we can create something, have feedback on that very quickly and then iterate so that we can get to
this end result **without having to go through days and weeks and months of revisions, which we know can
be the death of any agency, any client relationship.**"*

## Training custom models

⭐ **The largest block in the course**: modules 5 and 6, 39 minutes of the 2h 18m. This is where the course
moves from Midjourney to Flux inside Krea, because Midjourney cannot do it.

⚠️ **Quotes are verbatim from a spoken transcript.** It renders Krea as *"Kria"* or *"Korea"*, LoRA as
*"Lora"* or *"Laura"*, and jeans as *"genes"*. See **Provenance** (below).

---

### Why a custom model, and what it changes

> "If you're not familiar with custom models, essentially what they do is **they limit the data set.** So,
> you can create precise images, **they can be trained on your own assets**, and essentially **you can
> generate into infinity.**"

**The contrast he draws:**

| | Large model, e.g. Midjourney | ⭐ Smaller tailored model |
|---|---|---|
| Prompt a specific vehicle | *"they're gonna have a lot of varying outcomes because **it's taking a really big data set of all the images that it has in its mind**"* — a white car, a green car, a black car, *"all in varying environments, different lighting schemes"* | *"I might use **10 to 20 pictures of a very specific** green"* one *"and then it'll produce that car, specifically **the tires, the bumper, the brake caliper, the logo**"* |

> "So, **it's a way to just trim everything down, so it's only working off a limited amount of data, so it
> can replicate that.**"

**What a LoRA is, deliberately demystified:**

> "if you're not familiar with what a LoRa model is, **it sounds more intimidating than it is** low-rank
> adaption model. Basically, **you input your images into the training, it learns your images, and then it
> generates and replicates your images consistently.**"

⭐ **Not only for products:** *"you can also, it doesn't have to be just a car, **you can do this with
people, you can do this with products, you can do this with a style.**"*

---

### ⛔ The training-data guidelines

⚠️ **He hedges the word "rules" himself:** *"There's a couple, I don't wanna say rules, but there's some
hard, fast sort of guidelines that you should know."*

| Guideline | What he says |
|---|---|
| **Image count** | **5 to 100.** ⛔ *"if you have one image, it's not really gonna be that great, but **if you have at least five and ideally 10**, then we're gonna keep moving in the right way"* |
| **Resolution** | ⚠️ *"Typically, you need high res photography, so I wouldn't use anything that's under 124 pixels resolution here at a minimum"* — see the note below |
| **Aspect ratio** | ⭐ *"the best way to add the data into the data set is in a square format. **That's the default for majority of the image generators**, so a one by one format"* |
| **Angles** | ⭐ *"if you have a picture of my face, I don't just want a front picture of my face. I want the side or like a slightly angled, a side profile, maybe me turning my head all the way to the back **because we're trying to create essentially a 3D model of my face with still images**"* |
| **Logos and copy** | ⛔ *"if you can **avoid small logos and small copy**, that's gonna be the hardest thing for any model to replicate"* |

⚠️ **On the resolution figure.** *"124 pixels"* is what the recording says and it is quoted here unchanged.
**It is almost certainly a transcription artifact** — 124 pixels is a thumbnail, and it contradicts the same
sentence's demand for high-resolution photography and the reasoning immediately after it: *"The lower the
resolution you get, the more fuzzy your outputs become, so you wanna use things that are **as large and as
clear as possible** here."* ⛔ **Do not hand the number on as a threshold.** Give the rule it sits inside.

**If images are not square:** *"Photoshop has a **generative fill** feature, which is great. You can put an
image in and put it into a square and generate sort of a rounded or out-painted, so it can be a square."*
Krea and Midjourney both have equivalents.

---

### ⭐ The data-volume trade-off

> "the more images you have, the more varied your results can be, the less images you have, the tighter the
> results are gonna be. **So the more data, more varied results. Less data, tighter results.**"

⭐ **This is a dial, not a best practice.** Tight is right for a product that must be identical. Varied is
right for a style you want to explore.

---

### The four model types

| Type | Images | What it is for | His notes |
|---|---|---|---|
| **Style** | **10 to 50** | *"think brand aesthetic, a lot of lifestyle images"*, and B-roll source imagery | ⭐ *"I would look to have broader situations here, so not every person is the same or they're doing the same thing ... **because you're looking for the overall style, so style's more general than a product**"* |
| **Object** | **10 to 20** | One product, replicated | ⛔ *"I wouldn't use a pair of red sneakers and white sneakers in a training dataset **because they're just gonna mash it together**"* |
| **Character** | **5 to 20** | *"characters or subjects that can be a person, that can be a dog"*, or a brand mascot | *"you're gonna wanna have the same person in that"* |
| ⭐ **Default** | **5 to 100** | *"the default, which is where I like to live in Korea, because it's pretty versatile"* | *"It can be multiple people. It can be a mix of lifestyle and product, multiple environments."* |

#### ⛔ Before training a character model on a person

⛔ **Get their written permission, and say what the model will be used for.** The course does not ask for
this. It demonstrates character training on the faculty member's own face, where consent is implicit, and
then generalises to *"a character or a brand mascot or someone along those lines"* without ever raising
the question.

⭐ **Course 801 supplies the missing rule**, and it is the only place in the programme that does:

- ⛔ *"do not copy a person's appearance or voice without their permission"*
- Document the permission: *"we always make sure that we have the creator's permission to use the
  likeness in AI enhanced production"*
- ⛔ Check disclosure rules: *"Some platforms force their users to label AI-generated content, so make
  sure you have read the guidelines before you start advertising with AI-generated content"*

⚠️ **A trained model is not one image.** It is a reusable likeness that can be prompted into any scene,
shared as a code with a team, and used after the shoot is forgotten. **Scope the permission to that**,
not to a single asset.

#### ⭐ Two failure modes he demonstrates on himself

**Non-neutral clothing bakes in.** *"Better if you have neutral clothes, not a hard and fast rule. **Neutral
clothes allows you to change more.** Like in this dataset, for example, I wanted to show something that's
potentially problematic, so you're aware of it. **I'm wearing a green tuxedo and a bow tie** ... So, a lot
of times when I use this model, **I'm gonna end up in a tuxedo whether I asked for it or not.**"*

**Missing scale reference produces nonsense.** ⭐ *"I'll add like a picture of someone wearing the shoes,
because again, **if you don't give it any sort of depth or size perspective, they might end up looking like
clown shoes on really skinny legs.** They need to be, **it needs to be trained how to think these shoes fit
on feet**, right?"*

⭐ **The general rule behind both:** *"basically **anything with a hand is gonna be great** because it gives
the model an idea of how big something is."*

---

### ⛔ Fashion needs one model per colourway

> "when we start with training fashion, the thing to know is **this can be tricky**. And the reason is
> because **each product is going to require a new model. That means like each color needs a new model
> also.**"

**His arithmetic**, in the transcript's rendering of *jeans*: *"if you have genes in five colorways and you
have khaki pants and five colorways, **you need to train 10 models.** Because if not, you train genes and
khakis together, **you're gonna get a mashup of genes and khakis.** And that's not what we're looking for."*

> "**The idea is precision**, right? So we need to be very precise in the data that we curate. Sometimes it
> takes a couple extra models to do that, but the results, basically **you put the taxon up front, the
> results come after.**"

⭐ **Plan around this before promising a client a fashion library.** A ten-item catalogue in three colours is
thirty models.

---

### The Krea training settings

| Setting | What he says | His value |
|---|---|---|
| **Model type** | Style, product, character, or default | *"for this one, I'm gonna select default"* |
| **Training steps** | ⚠️ *"typically the more steps you have, **there's more detail, there is a risk of overfitting** there, meaning some things are gonna be off-sized"* | *"Between three or 400 is pretty good ... **I usually typically start as 350** as my setting"* |
| **Batch size** | *"**the bigger the batch, the more smooth the results.** Honestly, if you have more images, you're gonna wanna go with a bigger batch size **because it's gonna need to homogenize them into one look**"* | *"you can either go two or four. **I went four** for this one"* |
| ⭐ **Trigger word** | *"Basically, **it's how Flux recalls your model.** That's like **your trigger word is like your own little special token**"* | *"this was for the denim khaki. So I made the trigger word dank, D-E-N-K"* |
| **Use with** | *"the option to use with Flux real time or WAN"* | ⛔ *"You're gonna wanna use Flux for this."* |

**How long:** *"It doesn't take that long. Should only take about **five to 10 minutes**."*

⭐ **After training you get two things and you need both:** *"**you need a trigger word and a style code** to
generate in that sense or in that aesthetic."*

⭐ **And they are shareable, which makes this an organisational asset rather than a personal one:**

> "basically **you can share that too.** So if you're on a team and you trained a model, someone gets a
> really good model, **you can share this code with someone else. You can give them the trigger word.** They
> can start to do this on the same thing. So **not everyone has to do this individually. This can be way
> more organizational**, right?"

⚠️ **If a setting is unclear, he outsources it:** *"If you don't know, you can always look up, **I ask chat
GBT stuff all the time**, Claude stuff all the time for this and what it thinks should, what it would do
with this dataset, how we should adjust things."*

---

### ⭐ Whether a brand is even trainable

The most commercially useful section in the course, and the one worth showing to a brand owner.

| Trainable | ⛔ Hard to train |
|---|---|
| ⭐ *"a simple logo, the text is larger, it's placed right in the center"* | *"super small text. That is again, an issue"* |
| *"the branding is very minimalist and clean"* | *"a small logo ... everything is connected. So it's fluid. And that's also gonna be a problem **because there's not a lot of defined edge to it**"* |
| *"it's got a matte color to it, so it doesn't have that reflection"* | ⛔ **Reflective materials.** *"every lighting situation is different ... **there's shadow streaks that are going right down the center of the can. That's gonna be present in every one of your images regardless of the lighting**"* |
| ⭐ *"the super high contrast, so you have that yellow against the black ... **it pops, it's easy to recognize**"* | ⛔ *"when you have a green can with green letters, with green designs and everything's sort of intersecting and jumbled together, **this is not gonna be the best**"* |
| Defined shape, few features: *"the sunglasses, they just translate well. **The shape is very defined. There's not a lot of features to it**"* | *"The intricate branding can get hard"* — layered elements on top of each other |

⭐ **The advice he gives brand owners, which nobody else in the programme makes:**

> "**any brand owners out there**, if it's something that you're considering, might wanna consider looking at
> your branding as **can this be replicable by AI at some point because everyone's gonna be using it.**"

⚠️ **And the honest ceiling:** *"**your product can be great for Lora model training, your product can be
awful for Lora model training, it all kind of depends.** ... **You're still gonna need some post-processing
skills.** AI is not gonna be your best friend in every single situation. But **it's good to know how to get
you 95% of the way there** most of the time."*

---

### Prompting a trained model

> "Now prompting Flux is **different, but the same.** It still works off those same visual building blocks
> theory. **We need all of those pieces of the image to be present to control it.**"

**What changes:** Flux wants *"more natural language prompting"*, so *"the writing prompts gets a little bit
longer"* — closer to a paragraph than a token list.

⭐ **The decomposition is identical:** *"if we were to separate into categories like how we had it in
mid-journey, you can see just this has the photo type. It has the subject. It has what the subject is
wearing, the action, the lighting, the mood, the atmosphere, the environment, the colors, and then like the
modifiers. So **it's essentially the same thing. You're just adding more words**, right?"*

**The prompt ends with the trigger word and the style code.**

⭐ **His product-shot structure**, the slots minus a human subject: *"we'll use this prom structure where it's
editorial, perspective, photo of a black credit card, we'll describe the environment a little bit, go with
the color scheme, go with the emotion and the mood and the lighting"*, then *"at the end we'll add **sharp
crisp detail. I just like to add that a lot of times, it does help.**"*

⭐ **And he ships a prompt generator so nobody starts cold:** *"All you do is you can either upload a picture
into this custom GPT and say, help me create some prompts in this style. You can give it an idea via text
prompt ... So it'll give you typically around five prompts."*

---

### ⭐ What to iterate, once one prompt works

The payoff of the whole module: with a trained model and one working prompt, single-variable changes generate
a library.

| Change only this | And you get |
|---|---|
| **Perspective** | ⭐ *"it can be front view, it can be side view, it can be rear view, diagonal ... close up"* — *"you can then create five different assets from that same prompt"* |
| **Environment** | *"now we can go from a studio to a guy that's standing outside next to a car. Right now we bring it from inside to outside"* |
| **Clothing or top layer** | *"we changed the sweater, we changed it to a t-shirt, we changed it to a button down. Again, **the variability here is insane**"* |
| **Background details** | *"If I don't like the purple clouds, maybe I make them blue"* |

> "**we're isolating the variable within the prompt**, which is the environment, you can keep everything else
> the same if you want to ... **you can then go and do this into infinity.**"

⛔ **The mindset instruction, which is the point:**

> "**Don't get in the habit of generating one image and thinking that image is static and that's it. Every
> image is a little piece of a hole, it's a building block**, you can do a lot with it. It doesn't have to be
> very one shot, one deal."

⚠️ *"a little piece of a hole"* is the transcript's rendering of *a piece of a whole*.

⭐ **And the counterintuitive tip that closes the module:** *"I think it's really important that you keep
things simple because **simple is versatile.** This might look like the most boring image ever on the right,
but **one image equals multiple**."*

His example is a flat lay of shorts on a slate table, which he then points out can be re-backgrounded
endlessly, expanded for ad copy, or animated: *"This was stain resistant. We could splash a glass of wine on
it. If it's a Black Friday sale, we can have it get swiped out of the image. So if you think about the
versatility of one single thing of what that can be, **you're really only limited by your imagination.**"*

---

### ⚠️ Post-processing is not optional

> "So **nothing in AI is 100%** up personally, I think. So always gonna have a little bit of eye for detail
> here."

**What goes wrong, in his own examples:** a brand mark rendered as *"master C-A-A-A-A-A instead of master
card"*; on the credit card, *"the N26, which should be clear present branding is screwed up"*; and legs
visibly thinner in one colourway than another — *"his legs are skinnier than his legs are with the tan
pants."*

> "**That's kind of embarrassing, I've all been there.** But again, when you're looking at this, **Photoshop
> generative fill is a nice piece.** If you're not familiar with it, you can go in there and edit certain
> pieces of it to make it fit the aesthetic. Kria can do it within the editor."

⭐ **The one place the bar legitimately drops:** *"Solid little tip here. **Doesn't have to be immaculate if
you're using it for video** because it's gonna move and **the video generator will pick it up and sort of
like mesh it together.** So, I mean, obviously don't make it look pixelated and jacked up, take a little
time, polish it out."*

⚠️ **And when one tool cannot do it, he switches tools rather than rerolling.** A table looked *"super
polished and way too clean, like that looks AI to me"*, and Flux could not roughen it: *"It's not gonna be
able to really take that wood and turn it into something gnarly or matted. **It's very polished, it's a very
clean model, and especially the images that I've trained it on are super clean**, so that's not gonna be the
way that it outputs, so **I might take it into mid-journey**"* and ask for *"a gnarly wooden table"*.

---

### Krea's editor, and swapping a trained object in

⭐ **The feature that makes the models compose:** *"the other thing that Kria is exceptional at is it has an
editor feature. But its editor feature means **you can attach one of your models into the edit.**"*

**The sequence:** select the region (*"we select the pants. We don't just trace the region of the pants"*),
add the trigger word, then add the style code. *"So now it's telling the editor, **I wanna put these pants on
this guy.**"*

⭐ **And multiple models at once:** *"**you can attach multiple models**, you can describe it. Here we have the
tobacco, the olive, and you're the warm sand color khakis **so that we can have some different variants in
the colors**"* — three colourways in one image.

**Aspect-ratio expansion for ad layout:** *"The original might be in one by one, which is how I like to
generate a lot of product shots, it just tends to come out a lot better. But then also when you take this
into Create Editor, **I can turn that into 2-3 aspect ratio or 1920 by 1080, so that we can give it a little
bit more room to breathe on top so we can add copy in there.**"*

⭐ *"That's one of the best things that I think's ever happened with AI, is just simple things like that, like
**being able to give me space** so I don't have to go and do my whole Photoshop rigmarole to get to just a
blank space on top of my products."*

## Provenance

### Source

**Ad Creative Academy** — Course 802: *Prompt to Production: Crafting AI-Generated Image & Video Ads*
(800-Level). 2h 18m 32s, 9 modules. **Rory Flynn**, founder of Systematiq Ai, later working with a
design-as-a-service agency he describes as having *"an 800 person team"*.

⭐ **29,461 words. The longest single input in the entire programme.**

**Its worksheet:** a Midjourney V7 cheat sheet, listed by ACA as the course's downloadable asset. See the
warning about it below.

**ACA's stated learning objectives for the course:** Full Generative AI Workflow · AI Generated Image Ads ·
Prompt Engineering · AI Generated Video Ads.

**The nine modules, with ACA's own durations:** The Current State of AI (13m 30s) · Image Gen Basics: Intro
to Midjourney (10m 20s) · Mastering the Prompt (7m 28s) · Asset Cloning for Static Ads (12m 00s) · Creating
Custom AI Image Models Part 1 (28m 38s) · Part 2 (10m 28s) · Current State of AI Video (14m 14s) ·
Text-to-Video (26m 00s) · Image-to-Video (15m 54s).

⚠️ **The recording's internal section markers do not match those nine.** They read as the four learning
objectives instead, so module boundaries inside the transcript are approximate. Durations and titles above
are ACA's; the content mapping is this skill's reading.

---

### ⛔ The course number is contested, by the course itself

**Rory says the wrong number, twice, on the recording:**

> "So everyone, **welcome to course 502** crafting AI generated image and video ads."

⛔ **ACA publishes this as Course 802**, and three independent things confirm 802: ACA's live course listing,
the filename ACA itself sent (*802 - Rory Flynn - Prompt to Production*), and arithmetic — the 800-Level's
stated total of 04:23:51 equals 31:06 + 2:18:32 + 1:34:13 exactly, and its stated 19 lessons equals
4 + 9 + 6 exactly.

⚠️ **A second course in the programme is also numbered 502**, taught by a different faculty member on a
completely different subject (UGC talent). **The spoken "502" here is stale**, almost certainly from an
earlier numbering, and it is the reason older material in this library carries a 502 code for this course.

⭐ **Use 802.** If someone quotes "course 502" from the recording, they are quoting accurately and citing a
superseded number.

---

### ⚠️ The worksheet documents parameters the course never teaches

⛔ **Measured, not assumed.** The cheat sheet carries a twenty-parameter reference: `--sref` `--ar`
`--profile` `--p` `--s` `--q` `--c` `--exp` `--sw` `--ow` `--weird` `--r` `--iw` `--stop` `--v` `--oref`
`--sv` `--no` `--style` `--tile`.

**In the 29,461-word transcript, the literal string `--` appears exactly twice, and not one of those
parameters is named.** `--sref` appears zero times. `stylize` appears zero times.

**What the course actually teaches** is the prompt formula, the `describe` feature, and style reference as a
*concept* (*"style reference"* appears 7 times) — never as a flag.

⭐ **But the sheet is not off-message.** It independently prints the same six prompting rules, the same
prompt slots, and the same keep-versus-change split as the recording. **The gap is syntax, not method** —
which is what makes the parameters safe to use and still worth labelling.

⛔ **And the sheet contradicts itself once.** Its prose says Midjourney *"places the most focus"* on tokens
at the **beginning** of a prompt; its diagram labels say *"End of Prompt More Importance"*. Nothing in the
artifact resolves it and the recording never mentions token position, so there is no tiebreak.

⛔ **So when a prompt carries parameters, say where they came from.** The formula is taught on the recording;
the parameters are from a reference sheet, at whatever version it documents. Do not present them as Rory's
instruction.

⚠️ **The sheet is also third-party material**: no ACA branding and no course code appear on it, and it is
attributed to Rory personally. ACA's own curriculum sheet names it as this course's worksheet, which is why
it belongs here, but it is his artifact distributed through the course rather than ACA's.

⚠️ **And it is a wall-sized board, not a document** — a single page measuring roughly 296 × 352 inches.
Anything read from it comes from a spatial reconstruction of that canvas, not a normal page.

---

### ⚠️ Transcription artifacts, measured

The recording is a machine transcript and it renders tool names inconsistently. **Counts are exact.** This
skill quotes the source verbatim and names the real product alongside.

| Real name | What the transcript says | Count |
|---|---|---|
| Midjourney | *"mid-journey"* · *"mid journey"* | 26 · 5 |
| **Krea** | ⛔ *"Kria"* · *"Korea"* — **never spelled correctly** | 6 · 6 |
| **Kling** | ⛔ *"Cling"* — **never spelled correctly**, and *"clean elements"* for Kling Elements | 10 · 2 |
| **Veo 2** | *"Veyo 2"* | 1 |
| **LoRA** | *"LoRa"* · *"Laura"* | 1 · 1 |
| ChatGPT | *"chatgbt"* · *"chat GBT"* · *"chat.jpt"* · *"Chad GBT"* · *"chat GPT"* | 2 · 3 · 1 · 1 · 1 |
| Systematiq Ai | *"Systematic AI"* | 3 |
| jeans | *"genes"* | 4 |

⚠️ **ACA's own course description repeats two of these errors**, writing *"Flux/Kria"* and *"Cling"*. So the
misspellings are not only the transcript's.

⚠️ **His own name appears both ways in the material:** *"Rory Flynn"* and *"Rory Flinn"*, twice each. ACA's
curriculum sheet says **Flynn**, which is what this skill uses.

**Other artifacts quoted and flagged in place:** *"dye bar"* for dive bar · *"124 pixels"* for a resolution
floor · *"F1 card"* for F1 car · *"a little piece of a hole"* for a piece of a whole · *"problem structure"*
for prompt structure · *"the taxon up front"* for the tax on up front · *"vibacious"* for vivacious.

---

### The numbers, and what each is worth

| Claim | Status |
|---|---|
| ⭐ **65% reduction in cost, 65% reduction in hours**, on a run of **500 fully polished ads** | ⭐ **The only measured claim in the course, and it has a method.** *"we wanted to track this meticulously because if it wasn't saving time, or it wasn't saving money, then what's really the point"* |
| **5 to 100 training images**, 10 to 50 for style, 10 to 20 for object, 5 to 20 for character | Practitioner guidance, hedged by him as *"I don't wanna say rules"* |
| **350 training steps, batch size 4** | ⚠️ His own defaults for one tool at one version |
| ⛔ **"under 124 pixels resolution"** | ⛔ **Almost certainly a transcription error.** Contradicted by the same sentence. Never pass it on as a threshold |
| **720p / 1080p video output ceiling** | ⚠️ A tool-state claim, and the fastest-dating thing in the course |
| **24 frames a second, ~240 frames per 10 seconds** | Arithmetic, and consistent |
| **"about five to 10 minutes"** to train | ⚠️ Tool-state |
| **The 25% and 12.5% per-token split** | ⚠️ ⭐ **He labels this an analogy himself**, twice. Not a measurement |

⛔ **The 65% figure is the one most likely to be misquoted.** What it measures is **the cost and hours of
producing 500 ads**, on one project, for one client, in 2023, with a localisation problem. **It is not an ad
performance result.** No CPA, ROAS, CTR or hook rate appears anywhere in this course.

⚠️ **The client is deliberately unnamed** and Rory says why: *"my client does not allow us to talk about
this. Then they don't want to be known for using AI. So we are basically using a mock up here"* from a
comparable company. ⭐ **Worth noting as a fact about the industry**, not just a caveat: a brand that used AI
across a 500-ad campaign did not want that known.

---

### Named brands and tools

**Brands used as examples:** Red Bull (⚠️ explicitly *"not a client of mine"*) · Suitsupply · a fashion
apparel brand · a card issuer · a beverage brand named as the hardest model he has trained · another named
as easy · a friend's brand, used with permission — *"asked him if I could use it for the demonstration
purposes in here. He allowed me to do so"*.

⭐ **He is careful about attribution throughout**, which is unusual in this programme and worth preserving:
the disclaimer on asset cloning, the note that Red Bull is not a client, the mocked-up client, and the
explicit permission for the friend's brand.

**Tools named:** Midjourney · Flux · Krea · Leonardo · ChatGPT · Claude · Llama · Kling · Runway · Minimax ·
Sora · Luma Labs · Veo 2 · Photoshop · Figma · Canva.

⚠️ **No commercial relationship is disclosed for any of them**, and he is a vendor of AI services. That is
not an accusation; it is context for weighing a tool recommendation.

⛔ **Rule 9 applies to all of them.** Every tool here is an optional adapter, and the course's own
tool-agnostic argument is the manual fallback: *"the tools are interchangeable."*

---

### ⭐ Where this course quietly agrees with others

- ⭐ **Asset cloning is Course 301's reverse-engineering argument**, applied to images instead of scripts, by
  a different faculty member. *"Everything is translatable, everything is data. And ... if you can dissect
  anything, you can rebuild it."* **Neither course cites the other.**
- ⭐ **The static-supply problem answers Course 601 and Course 703's volume demands.** *"you might end up with
  100, 200 great images, but ... you might blow through those in a month."* This is the only supply-side
  answer in the programme to the volume those two courses require.
- ⭐ **The eight building blocks are Course 103's building-blocks framework** for a different medium: same
  claim that an ad decomposes into interchangeable parts.
- ⚠️ **Course 803 is the same faculty member and does cite this one**, which makes it the only genuine
  faculty-authored cross-reference in the programme. Everything else agrees by accident.

⚠️ **And one place it collides.** Course 105 teaches AI adoption as *process first, then automate*; this
course teaches a five-stage ladder where SOPs arrive at stage 4, after everyone is already using the tools
in their own way. ⭐ **They are compatible if read as description versus prescription** — Rory is describing
what happens, Course 105 is prescribing what should. Worth naming rather than blending.

---

### What is quoted and what is organised

**Everything substantive is Rory's, quoted directly** — the equation, the diffusion explanation, the token
demonstrations, both prompt structures, all five asset-cloning steps, every training guideline, the nine
camera motions, and every worked prompt.

⭐ **Every quotation in this skill has been checked character by character against the transcript**, and
compressions are marked with an ellipsis. Where the recording says something odd, the oddity is preserved
and flagged rather than corrected.

**This skill's organisation, not ACA's:**

- Splitting the course into mechanism, prompting, cloning and training, which is not its module order
- Rendering the eight- and six-slot formulas as numbered tables. ⚠️ **He never numbers them**; he lists them
  in speech, and the slot count is this skill's reading
- The two-group split of the eight slots into visual signature and variables, rendered as a table. ⭐ **The
  rule itself is stated in BOTH sources** — the recording says *"flip the photo type, the subject and the
  action and the environment"*, and the cheat sheet prints *"keep: Color scheme, technical details,
  composition, lighting, modifiers"*. **Two independent statements of the same rule**, which makes it the
  most reliable thing in the 800-Level
- The trainable-versus-untrainable comparison table
- Collecting the cons into one place, since he scatters them across four modules

**This skill's additions, drawn from the material rather than stated by it:**

- ⛔ **The measurement that the worksheet's parameters are never taught in the course.** ACA does not note
  this and neither does Rory
- ⭐ **Naming the removal experiment as the structural lesson** of the whole course, rather than one
  demonstration among several
- ⭐ **The observation that step 2 of asset cloning fails by design**, and that step 3 exists to fix it. He
  shows this; he never says it
- ⭐ **The point that "bake motion into the still" is a cross-module instruction** — it changes how you prompt
  images, and it appears in the video module where an image-stage reader will not find it
- ⚠️ **The distinction between the 65% figure as a production saving and as a performance claim**
- ⭐ **The note that stage 3 of the adoption ladder is the trap**, because that is where he says most people
  are and it is the stage with no organisation
- ⚠️ **The fashion arithmetic extended** to a ten-item, three-colour catalogue equalling thirty models
- ⚠️ **The observation that he is unusually careful about attribution**, and that his client's wish to hide
  AI use is itself a finding
- ⚠️ **The Course 105 collision**, and the reading that reconciles it

---

### ⚠️ How old this material is

**ACA stamps no recording date.** Received into this library in **2026-W31**, which is a "no later than",
not a date of recording.

⭐ **Internal evidence dates it more precisely than ACA does.** Rory references Midjourney 5.2 as *"almost a
year and a half removed now, we're at mid-journey 6.1"*, describes a 2023 client project, and calls Veo 2
something he is *"lucky to be in their beta program"* for. **The material is meaningfully older than its
receipt date.**

⛔ **What dates fastest:** every tool name, every version, every UI walkthrough, the 720p ceiling, the
missing-upscaler claim, and the training settings.

⭐ **What is durable:** the prompt-equals-output equation, the token-weight law, the removal experiment, the
building-blocks decomposition, asset cloning as a method, the interaction principle, the nine camera
motions, and the creativity-control trade-off. ⚠️ **None of these depends on a tool**, which is exactly the
argument Rory makes for teaching them.

⭐ **He dates his own material inside the course**, which is the right way to read all of it: *"I could be
talking to you right now, and five new models have already released. So the pace of development here is
insane."*

### Scope

Production craft for generative image and video assets. ⛔ **No performance metric, benchmark or threshold
appears anywhere in this course.** What to say belongs to Courses 102, 103 and 401; what the numbers mean
belongs to Courses 402 and 701.

### Credit

Ad Creative Academy's curriculum and Rory Flynn's teaching are their own work; the cheat sheet is his. This
skill organises that material for reference; it does not originate it.
