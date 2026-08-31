# Prompting: the formulas

⚠️ **Quotes are verbatim from a spoken transcript.** Where a word looks wrong it is the recording's;
`reference/provenance.md` lists the tool names and the one number that are transcription artifacts.

---

## The five rules

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

## ⭐ The photographic elements

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

## ⭐ The image prompt formula, eight slots

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

## ⭐ The video prompt structure, six slots

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

### Two extra rules for video

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

## ⭐ Interaction: the thing that gives AI away

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

## The nine camera motions

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

## The three video modes

| Mode | How it works | ⛔ Where it fails |
|---|---|---|
| **Text-to-video** | *"you write a text prompt, generates a video"* | *"there's no image reference. So you have to control all the things"* — ⛔ *"consistent characters and styles can be very hard"* |
| **Image-to-video** | *"we create an image, we write a prompt, and then we generate a video"* | ⭐ *"you're basically giving it a halfway mark"*, so prompts run shorter — ⛔ *"a lot of times where it lacks is on extreme motion"* |
| **Video-to-video** | *"a video with a text prompt that you generate a video from"* | *"there's less you can do because the structure of the video is already defined"* — ⛔ *"this video of me walking and then changing to me doing jumping jacks, video to video is not the way to do"* it |

### ⭐ Image-to-video is where the work happens, and the still decides it

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

### ⭐ Bake motion into the still

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

## Adding text to an image

> "you can add that very simply by just **putting the words you want in quotation marks**"

His example: *"let's just say we wanted the black crew neck sweater with the words USA on the, in
collegiate bold font. If you put quotation marks or open quote unquote around USA, it will read that as
I need to add text."*

⚠️ **One or a few words only.** *"you're not gonna be able to add a paragraph in there if you wanna add
one word or a couple words here and there. That can be really executed well. When you wanna add a full
paragraph of text ... it's probably not gonna look good."*

---

## ⭐ Using ambiguity deliberately

The one place the course inverts its own opening rule, and it is a real technique:

> "When you have this super detailed prompt on the left, **we're trying to get something exact. When you
> don't know what you want, you can use a little bit more ambiguous of a prompt to vary the outcomes**"

His example of a deliberately loose prompt: *"a man is posing with a dramatic thoughtful expression"*.

> "That could go from an image generation standpoint, 50 million different ways, **but that can also be
> good, so we can use ambiguity to our advantage.**"

⭐ **The distinction: precision for replication, ambiguity for exploration.** Both are prompt-craft;
neither is a mistake.

---

## Happy accidents

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

## Negative prompting

⭐ **Kling's differentiator, per Rory:** *"that's the one that's a very big differentiator that clean has.
The other ones don't is this negative prompt feature."*

> "If you're not familiar with negative prompting, **it's basically just what you don't want in the in
> the output.** So I'll typically put in there if I'm doing something that's photorealistic. Like I
> don't want animation. I don't want blur. I don't want distortion. I don't want X."

⭐ *"if you don't want people with tattoos, just put tattoos in the negative prompt. It'll take that. It'll
take it out. It won't generate those."*

---

## The motion brush

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

## Keyframes

> "basically, it is **you give it a first frame and a last frame, or a first frame only. Or a last frame
> only. It generates before after in the middle.**"

**His examples of what this is for:** *"you go from a blank apartment to an apartment that's filled. Like
that is a great way to sort of show development."* And ⭐ *"We have a first frame of an egg. Second frame is
an egg sandwich, right? Like we're showing basically the origin story of this egg sandwich."*

⭐ **Which makes keyframes the native tool for before-and-afters and transformations**, the two most common
ad structures this technique fits.
