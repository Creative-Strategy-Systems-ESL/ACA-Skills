# How the generators actually work

⭐ **Read this before the prompting file.** Rory spends the first third of the course here on purpose:
someone who understands the mechanism debugs their own prompts, and someone who does not just rerolls.

⚠️ **Quotes here are verbatim from a spoken transcript**, so they carry speech as spoken. Where the
recording renders a tool name oddly, `reference/provenance.md` lists what the source says against what
the tool is called.

---

## The equation the whole course rests on

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

## Diffusion, in his terms

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

## ⭐ The token-weight law

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

### ⭐ The removal experiment, which is the real lesson

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

## How video generation differs

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

### ⭐ The X factor is motion

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

## ⭐ The creativity-control trade-off

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

## The video tool stack, with his strengths and weaknesses

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

## ⚠️ The cons, in his words

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

## The adoption ladder

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
