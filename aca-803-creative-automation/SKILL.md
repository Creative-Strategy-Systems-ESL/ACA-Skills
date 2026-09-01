---
name: aca-803-creative-automation
description: Ad Creative Academy Course 803, Rory Flynn of Systematiq Ai - building an automated AI ad engine instead of prompting one image at a time. Covers the three core AI skills that make you tool-agnostic (deconstruction, system prompts, workflow development), the keep-this-change-that edit formula for in-context image models, the six parts of a system prompt with limits as the load-bearing one, node-based workflow building, batch processing so one input returns twenty outputs, and the reusable image generator whose only per-brand variable is a Visual Brand Profile. Use this when a team is prompting by hand and cannot keep up, when output is inconsistent between people, when the same creative job is being redone every week, or when someone wants to build a tool rather than make an asset. Reach for it whenever AI workflows, automation, batch generation or system prompts come up.
---

# Course 803: The Creative Automation Workshop

**Rory Flynn**, founder of Systematiq Ai, and the same faculty member who teaches Course 802. 1h 34m 13s,
6 modules.

> "We are going to go into a little bonus module on workflow building. Now that we've done a lot of things
> with the images and the videos ... **so we can actually start to build little micro tools**"

⭐ **This is the only course in the programme that builds a tool rather than an asset**, and the only one
that cites another course: it assumes Course 802 and explicitly extends it.

## What this skill needs from you

**Required:**

1. **The repeating job.** ⛔ **This course is for work that happens more than once.** A one-off image is
   faster by hand; the whole argument is *"there's no more single thoughts"*.
2. **The brand, and 10 or so of its images.** The Visual Brand Profile is built from them and it is the
   piece that makes a workflow reusable.
3. **What one run should produce** — 20 static variants, a prompt set, a video, an edited product shot.

**Useful:**

4. Who else will run it. ⭐ **Workflows are shareable and that is half their value**: *"It's something that
   can be shared between you or your team or a friend or whoever."*
5. Whether they already have prompts that work, which become the system prompt
6. Whether the assets ship as-is or get finished by a designer. ⚠️ **They are not finished goods** — see
   the scope note

⛔ **Never present a tool-specific workflow as the skill.** The course's own argument is the opposite:
*"it won't be about the tools, it'll be about what you can do with them."* The three core skills work
anywhere; the node editor is one implementation.

## Where to go

| They are asking | Go to |
|---|---|
| What do I actually need to learn? | **The three core AI skills** (below) |
| How do I write a system prompt? | **The three core AI skills** (below), the six parts |
| How do I edit an image with a prompt? | **The three core AI skills** (below), keep-this-change-that |
| How do I build the workflow? | **Building the workflow, and batching it** (below) |
| How do I get 20 outputs instead of 1? | **Building the workflow, and batching it** (below), batch |
| How do I point it at a different brand? | `aca-build-visual-brand-profile` |
| Where did these claims come from? | ⚠️ **Provenance** (below) |

## The through-line

> "**We don't want single outputs anymore. We have to think in batch.** So like in this case it's how do
> I put this image in, write a prompt and **I get 20 outputs instead of one** and 20 different variations."

⭐ **That is the whole course in one sentence**, and it is a different claim from Course 702's volume
argument. 702 says produce more ads. This says **build the thing that produces them**, so volume stops
being a headcount problem.

## How to run it

⛔ **This is for work that repeats.** A one-off image is faster by hand, and the whole argument is that single
outputs are the thing to stop making.

1. **Confirm the job repeats.** If it does not, route to Course 802 and stop here.
2. **Teach the three core skills** from **The three core AI skills** (below) — deconstruction, system prompts,
   workflow development. ⭐ Someone who learns only the node editor has learned nothing portable.
3. **Give the keep-this-change-that edit formula**, same file, with the keep clause stated explicitly. The
   model will not guess which part is the product.
4. **Write the system prompt** in its six parts, same file. ⛔ Limits is the load-bearing part: without it the
   model answers conversationally and breaks the next node. ⭐ **Its core-focus section is where the Visual
   Brand Profile goes**, so build that first if the output has to be on-brand —
   `aca-build-visual-brand-profile`, if installed. It is the one variable that repoints the whole workflow.
5. **Build the workflow** with **Building the workflow, and batching it** (below). ⛔ Everything must be connected — the most
   common silent failure is a workflow that runs and quietly ignores your product.
6. ⛔ **Test before batching.** Batching a broken system prompt costs twenty generations to discover.
7. **Batch it**: ask for ten prompts, separate them with a delimiter the content cannot contain, split, run.
8. ⭐ **Hide the system prompt in app mode.** It is the tool's logic, not its input.
9. ⭐ **Swap the profile to point it at another brand.** Nothing else in the workflow changes, and that is
   the test that a tool was built rather than one job done.
10. **Check the output is treated as raw.** These are assets to finish, not finished assets.

## Answering well

**Lead with the three core skills, not the tool.** Deconstruction, system prompts, workflow development.
*"These are three tools that are three skills that can be used anywhere in any time, in any medium. And
basically this will make you sort of tool agnostic."* ⭐ **Someone who learns only the node editor has
learned nothing portable**, which is the argument the course makes about itself.

**Deconstruction is Course 802's asset cloning, generalised.** Rory says so: *"think about the image
deconstruction model that we did"*. ⭐ **And he extends it past images** — *"that same process of
deconstruction can work for video. It'll work for sound, it'll work for music, it'll work for ... add
scripts or, you know, copy."*

**The edit formula is two words.** *"what is editing. Essentially it's if you break it down to its core
component components, **keep this change that**."* ⛔ **Then say what to keep explicitly**, because the
model will not guess which part is the product.

**In system prompts, limits do the work.** Six parts: actors, goal, output, core focus, format, limits.
⭐ *"limits probably the most important thing"* — and his worked example shows why: without *"do not
include any explanation, just provide the prompt"*, the model returns conversation that breaks the next
node in the chain.

⚠️ **Be honest about what comes out.** *"I would consider all of these **raw assets** that you're going to
have to sort of doctor up in your own way."* The workflow removes the repetition, not the craft.

## ⚠️ Scope

Building the machine. ⛔ **No metric, benchmark or performance claim appears anywhere in this course** —
what to test is Course 602, what the numbers mean is Courses 402 and 701, and what the ad should say is
Course 401. ⚠️ **It also does not decide creative volume**: Course 703's five variables and Course 601's
spend ladder do that.

⛔ **And it is the most tool-dependent course in the programme.** Every walkthrough runs inside one
third-party node editor. Carry the three core skills as the durable part and treat the tool as one
example, which is what the course itself asks for.

## Reference files

| File | Read it when |
|---|---|
| **The three core AI skills** (below) | Deconstruction, the edit formula, and the six parts of a system prompt |
| **Building the workflow, and batching it** (below) | Node basics, building the generator, app mode, and batch processing |
| **Provenance** (below) | ⚠️ **Read before quoting any tool claim.** Includes the duplicated-source note and the conflict with Course 802 |

---

## The three core AI skills

⚠️ **Quotes are verbatim from a spoken transcript**, which renders the tool as *"YV"*, *"CV"*, *"weave"* and
*"weaving"*, and LLM as *"LM"* or *"LMS"*. See **Provenance** (below).

---

### Why skills rather than tools

> "as you know, with the AI world, everything moves really quick. And these tools change all the time. But
> **a lot of times with the workflows they don't change that much.** So. And one of the same process is
> going to be employed. And I think this is **how we get ourselves to be sort of tool agnostic**"

> "It's more so like **I already have a process in place. Let me just swap the newest and the best**, you
> know the best for what comes next."

> "first I think we have to talk about the core AI skills, right? **These are three tools that are three
> skills that can be used anywhere in any time, in any medium.** And basically this will make you sort of
> tool agnostic. Like I said, **it won't be about the tools, it'll be about what you can do with them.**"

⭐ **This is the strongest claim in the 800-Level and the easiest to lose.** A reader who takes away only
the node editor has taken the perishable half.

---

### ⭐ Skill 1: Deconstruction

> "first one is deconstruction, where basically it's like, **how do we take something, break it down into
> its core components and then build out from it?** So think about **the image deconstruction model that we
> did** in terms of taking an image, turning it into its requisite parts, and then rebuilding it."

⭐ **That back-reference is to Course 802's asset cloning.** It is the only place in the entire programme
where one course cites another, and it is the same faculty member doing it.

**And he immediately widens it past images:**

> "that same process of deconstruction **can work for video. It'll work for sound, it'll work for music,
> it'll work for, you know, add scripts or, you know, copy** anything like that. Right. So deconstruction is
> just **a main point in terms of being able to maneuver with AI.**"

⭐ **Worth naming:** that generalisation is also Course 301's argument about ad scripts and Course 103's
about ad structure, reached from a third direction. Neither of those courses is cited here.

#### ⭐ The edit formula: keep this, change that

The concrete form deconstruction takes once image-editing models exist.

> "we have to think about like **what is an edit**. Like it's **same theory of deconstruction**. Like what
> is editing. Essentially it's if you break it down to its core component components, **keep this change
> that.** Right. Pretty simple. **It doesn't have to be any harder than that.**"

**The structure he gives:**

> "I would structure this as like **keep colon details** you want to keep **change colon details you want
> to change or add or remove** or you know, anything of the sort."

| Slot | What goes in it |
|---|---|
| ⭐ **keep:** | The part that must survive — the product, the fine details, the branding |
| **change:** | Everything else: the scene, the position, the framing, the mood, what else is happening |

**His worked prompt**, on a supplement brand:

> "**keep colon this exact product visible and preserve define details** right change might be **cyclist mid
> training ag1 bottle thrusted the camera with a wide angle vertical crop, powerful sweat soak expression,
> blurred background, dramatic mountain the horizon glowing behind**"

⚠️ *"preserve define details"* and *"thrusted the camera"* are the transcript's renderings of *preserve fine
details* and *thrust toward the camera*.

⭐ **How fast this is, and why it changes the economics:** *"once we run it, we get stuff that is
relatively usable right out the gate ... **this is like took all of 30s.**"*

⛔ **But the value is not the one image**, and he says so in the next breath:

> "**where it gets really cool is when we can start to scale this**, when we can say, okay, I have this
> image, but **I want to make 30 images at a time, 40 images at a time, 100 images at a time**, instead of
> just doing one."

> "That's how we can start to change our thought process ... We can start to run. Like I said, **3040 of
> these at a time and then pick the winners**, right? That's when it gets cool."

⭐ **"Pick the winners" is Course 702's argument arriving through a different door** — you cannot predict
which one works, so generate the set and select. Neither course cites the other.

#### ⚠️ In-context editing models, and what they replace

> "the biggest sort of shift in AI is what's called these **In-Context models.** We did we went through a
> little bit of the Laura training stuff, which is how do I take one singular product and do sort of train
> a model on that ... **these image models make it a lot easier.**"

> "these editing image models, right, where you can **just take anything and just say, put this here or
> make this, do this, or change this character's clothes.** It's really easy. **It's natural language, it's
> super simple, it's intuitive now** ... And it's **actually relatively easy in comparison to what we did
> with the Laura training stuff.**"

⛔ **Read that carefully: the same teacher is saying his own Course 802 module on LoRA training is now
largely unnecessary for consistency.** That is not a contradiction to hide — it is the most useful thing in
the course for anyone deciding where to spend a week. See **Provenance** (below) for how the two courses
sit together.

> "**This is the thing that I would say to keep your eye on the most.** And it's a way to just really, you
> know, **take consistency and take that problem out of the mix**"

**Models he names for it:** *"Nano bananas, Google products Gemini 2.5. Incredible. Really good"* ·
*"Cadence has an editing function as well"* · *"ChatGPT, image flux, context runway references"* · *"Rev
right now is, is coming up"*.

⚠️ **He expects the field to level:** *"everyone is going to have this type of model very soon."*

⭐ **And the method for when a new one lands**, which is the tool-agnostic claim made operational:

> "Basically, once something like this comes out, **we have to understand what the model does and how it
> functions.**"

---

### ⭐ Skill 2: System prompts

> "Second one is system prompts. System prompts are essentially like **how we tell the LMS what to do and
> how we tell them what to do every time.** So if you're familiar with building like custom GPT, you know,
> again, like you build a custom GPT to just like do this single task every single time."

⭐ **The line that explains why this is a core skill and not a trick:**

> "**So also system prompts are like the precursor to agent.** So it's **how we move things from process to
> process without having to have a human in the loop** with a lot of it. So it just becomes really
> important."

And: *"what they do is they just **guide the output.** You're telling the LM what to do. Every single time.
So it's becomes **controllable and predictable**."*

#### The six parts

⚠️ **He hedges them:** *"these are not 100% why you have to use this every single time. This is just as if
we condensed it down to what's the most usable."*

| # | Part | What it sets | His framing |
|---|---|---|---|
| 1 | **Actors** | Who the model is acting as | *"whose is GPT acting as. How do we want it to respond ... **each one is going to sort of alter the output**"* |
| 2 | **Goal** | The end state | *"what exactly we're trying to do. So it knows every time. So it has like **an end goal**"* |
| 3 | **Output** | What to do with each input type | *"depending on whether I give it a, you know, a piece of text, if I give it an image, if I give it a video, **it's like, what are you supposed to do with those**"* |
| 4 | **Core focus** | The default subject matter | *"what you specifically want it to focus on. **Should this be realistic? Should this be a video**"* |
| 5 | **Format** | The shape of the answer | *"Do we want it to be in a list? Do we want to be in a prompt? Do we want it to be in a script?"* |
| 6 | ⛔ **Limits** | What it must not do | ⭐ *"**limits probably the most important thing**, which is like just don't do this"* |

⚠️ **Why part 3 needs to be explicit:** *"a lot of times you have to be **very specific and practical** with
these tools because **they'll just take whatever you say and sort of add context to it without you giving it
to it.**"*

#### ⭐ His worked system prompt, a prompt generator

Reconstructed from the six parts as he reads them out.

| Part | What he writes |
|---|---|
| **Actor** | *"act as a visual merchandizer"* — ⭐ *"it's a good holding category for, generating prompts tailored to AI generation models"* |
| **Goal** | *"to help users generate really solid prompts, especially in **photorealism and human anatomy**"* |
| **Output** | *"for every user input, image or idea **always generate a distinct prompt**"* |
| **Core focus** | *"while **photorealism and cinematic realism are your focuses**, you should also support other styles when requested"* |
| **Format** | *"All prompt should be expressive and suited to intended style"*, using the Course 802 prompt formula, and ⭐ *"**Minimum of 250 to 350 words**"* |
| ⛔ **Limits** | *"**do not include any explanation, just provide the** problem."* ⚠️ The transcript says *"problem"*; he means **prompt**, and says so in the next sentence |

⭐ **Why "visual merchandiser" and not "photographer":** it is *"generic enough to know that it's going to go
to multiple models is not just Midjourney, it's not just flux, it's not just runway."* **The actor is chosen
to keep the prompt portable.**

⭐ **Why core focus has an escape hatch:** *"if I give you like a 3D render, basically just adapt the process
to it. **Don't just be so rigid and say, I can't do this because it's not in my training.**"*

⛔ **And why limits is the load-bearing part.** Without it the model answers conversationally, and in a
chained workflow that answer becomes the next node's input:

> "I don't want it to be like, **here's the prompt that I created for you.** And I wanted to just do what I
> ask and just give me the prompt"

> "the back end is like, **do you have any more questions with those things can screw up the output.** So we
> don't want it to be that way."

⭐ **That is the difference between a prompt for a person and a prompt for a pipeline**, and it is the single
most practical thing in the course.

⚠️ **On the 250-350 word figure:** it is *"typically like a good range for all of the image generators.
Where you know you're going to get a good enough amount of detail."* ⛔ **It appears to contradict Course
802's "do not use full sentences"** — see **Provenance** (below), which reconciles them.

⚠️ **He notes this used to be manual work:** *"if you've been in ChatGPT for a long time ... **you used to
have to prompt like this to get a good answer.** Now it's sort of like built as a system."*

---

### ⭐ Skill 3: Workflow development

> "workflow development really is just like, **how do I get from point A to point B? And in what sequence do
> I do it and what tools do I need?**"

⚠️ **He flags this as the least stable of the three:** *"This portion will change. Often it's really about
understanding again **what the tools can do, what their capabilities are.** And then we can start to sort of
like build around it."*

And: *"this is the skill that will be **the most fluid moving forward**."*

**Why he thinks it is where everything is heading:**

> "You're seeing all the tools start to roll out some sort of, you know, **node based system where you can
> use multiple tools in one space** to do certain tasks, and **it's all going to be customizable.**"

#### What it buys

| Benefit | In his words |
|---|---|
| **Scalable** | *"What's good about this is it's scalable"* |
| ⭐ **Shareable** | *"It's something that can be **shared between you or your team or a friend** or whoever"* |
| ⭐ **No more tabs** | *"**I don't have to go and write a prompt in GPT, copy it, go to Midjourney, create an image, download that**, go to ... clang or runway"* |
| **Traceable** | *"it's a way for us to like sort of **track our progress in each step**"* |
| **Reusable** | *"really like **build things that we can use over and over again**"* |

⭐ **And the mental shift, which is the course's thesis:**

> "we want to start thinking about it as **there's no more single thoughts**, right? Like it's not single
> prompts, not how do I just do one thing to one thing? **We don't want single outputs anymore. We have to
> think in batch.** So like in this case it's **how do I put this image in, write a prompt and I get 20
> outputs instead of one** and 20 different variations."

---

### ⭐ The end state he is building toward

The reason the three skills combine rather than stack:

> "this next slide, which is basically **where we want to end up**, which is **I want to provide the idea**,
> I want the system prompt that says, I do this every time ... **The line will go and generate the prompt
> itself. And then I can send to the image model so that I don't have to do that in multiple steps. I can
> just describe my idea, hit enter**, and then we get different iterations of this from the image model"

⚠️ *"The line"* is the transcript's rendering of *the LLM*, which it also writes as *"LM"* and *"LMS"*
elsewhere.

⭐ **Read the chain:** an idea in plain words → a system prompt that turns it into a proper prompt → an image
model that renders it → twenty variants back. **Deconstruction supplies the formula, the system prompt
enforces it, the workflow connects it, and batch multiplies it.** That is why all three are called core.

## Building the workflow, and batching it

⚠️ **The tool is one implementation.** The three core skills are the portable part; this file is how the
course wires them together in a node editor. ⚠️ **The transcript renders the tool's name as *"YV"*, *"CV"*,
*"weave"*, *"weaving"* and *"Wi-Fi"***, and the models by ear. See **Provenance** (below).

---

### Where the tool sits

> "They call it **an artistic intelligence platform** ... you can use all of these models, have a lot of big
> partners that's really built as **like a professional tool.** So it's **a little bit more complex than
> some of the other options** out there."

**His placement of it against the alternatives:**

| Tier | Tool | His words |
|---|---|---|
| Lite | Flora / Fauna | *"they're sort of like **the lite version**"* |
| ⭐ Middle | This one | *"**it sits right in the middle, which is why I like it a lot**"* |
| Extreme | ComfyUI | *"that's like **the extreme version**"* |

⭐ **Who it will feel familiar to:** *"if you're familiar with utilizing **node based tools**, if you've ever
worked in post-production or you've worked in, you know, Photoshop, **it's kind of how I wish Photoshop
would work.**"*

⚠️ **And it was mid-acquisition when he recorded:** *"as you can see up here is joining Figma. **By the time
you watch this. Don't know if it'll be integrated into Figma just yet.**"* ⛔ **Assume the UI has moved.**

---

### The node vocabulary

⭐ **The one hard part, in his words:** *"the hardest part of learning" the tool "is just learning the
functionality in these node based tools, or like **how this whole thing connects together. Once you have
that down, it's the same thing you've always been doing.**"*

| Node group | What is in it |
|---|---|
| **Text tools** | ⭐ *"We're going to use these a lot"* — the prompt box, prompt enhancer, image describer |
| **Toolbox** | *"traditional editing tools like you'll have your levels compositor or painter, you know, resizing things, extracting video frames"* |
| **Production** | *"mask extractor ... merge alphas"* |
| **Image models** | *"Reve, Higgs field, GPT image", flux, "re Craft", "Mystic"* |
| **Image editors** | *"nano banana", "sea dream", "runway gen for", "flux context"* |
| **Helpers** | *"import, export, preview"*, model upload, routers, ⭐ **sticky notes** |
| **Data types** | *"list selectors ... toggles"* |

⭐ **Use the sticky notes.** *"If I wanted to be like, okay, this is my, you know, image generation tool,
just so you can label stuff. So it's simple."* A workflow nobody can read is not shareable, and shareable
was half the point.

⚠️ **And name the file first.** *"oftentimes like you'll just start building workflows and **you just forget
to name them.** So just I always just name this right away."*

⭐ **Its own library is a reading exercise:** *"you can see **how these workflows are built, how each one of
these nodes are getting prompted**, sort of where they go, how they're iterating things like text, how
they're building different variations of these product shots ... **it is just a good area to go find some
inspiration.**"*

---

### ⛔ The failure mode, which he demonstrates on purpose

> "It didn't actually do this **because I made a mistake**, right? **I did not attach the image here. I did
> that on purpose.** So one of these things you have to realize with Wi-Fi is that **everything has to be
> connected.**"

⚠️ *"Wi-Fi"* is the transcript mishearing the tool's name, which it also renders as *"YV"*, *"CV"* and
*"weaving"*.

> "because there's no image attached here, **this product is not going to go right into the image.** It's
> just going to take this idea."

⭐ **The debugging rule to memorise:**

> "That's just something to always note. If it's like why and why didn't this work? **Probably because
> something's not connected.** That's where this stuff gets a little bit difficult."

⚠️ **This is the single most common way a node workflow silently produces plausible garbage** — it runs, it
returns an image, and the image simply ignores your product.

---

### The simple version first

**Three nodes:** a product image, a prompt, and an image-editing model.

> "if we wanted to just do this in the basic way, let's just do a prompt right. We'll have our prompts here,
> and then we'll use something like **nano banana** ... This is the simple way we attach our prompt. We
> attach our image."

**And the prompt is the keep-this-change-that formula:** *"keep this exact product and preserve the fine
details change. Put this bottle on a countertop in a high end luxury apartments."*

⚠️ **On aspect ratio:** *"you can also change the aspect ratio. **Most of the time it will just want to use
default. It will default to whatever aspect ratio this is.**"*

---

### ⭐ Adding the system prompt: the auto-prompt tool

The build that turns three nodes into a tool.

**The wiring**, in his order:

1. Add a second text node. **Rename one `User prompt`, the other `System prompt`.** ⭐ *"So now we have both
   of these in here."*
2. Add the LLM node.
3. ⭐ **Attach the image to the LLM** *"so it knows the context ... of what it's going to generate"*.
4. Attach the user prompt.
5. Attach the system prompt.
6. Send the LLM's output to the image model.

⭐ **The division of labour, which is the whole idea:** *"we wanted to make this lifestyle photo really we're
going to **give very loose instruction. But we want the system prompt to do most of the work here.**"*

And: *"we're just **feeding it a loose idea, having the system prompt to actually do the heavy lifting.**"*

#### His system prompt for it, part by part

| Part | What he writes |
|---|---|
| **Actor** | *"professional magazine photographer specialty and created art director prompts for image generators"* |
| **Provided** | *"We provide an idea for a prompt and an image of a product"*, and *"We're going to take that prompt into account when creating new prompts"* |
| **Task** | *"generate one new prompt for image generation"* |
| ⛔ **Format** | *"we want **no additional context commentary or thoughts or analysis, just the raw prompt**"* |
| ⭐ **Rules** | *"follow the exact format below to craft each prompt, so **always start the prompt with keep this exact product visible.** Change" whatever you want to change* |
| **Example** | *"keep the exact product visible ... we have changed the model. Hold a product smiling dynamic studio angle"* |

⚠️ *"created art director"* is the transcript's rendering of *creative art director*.

⭐ **Note what the rules section does:** it hard-codes the keep-this-change-that formula into the tool, so
every prompt the LLM writes preserves the product whether the user remembers to ask or not. **That is the
system prompt earning its place** rather than being a politeness wrapper.

#### ⛔ Test before you batch

> "this is again **the base of where we're going to do this at batch. Like we have to know that this works
> first. We can get good outputs with this system prompt. Then we can go and start doing other things.**"

⭐ **Do not skip this.** Batching a broken system prompt produces twenty broken outputs and costs twenty
generations to find out.

#### ⭐ Then it generalises for free

He swaps the product and it keeps working, which is the proof that a tool was built rather than an image
made:

> "**the goal here again is that we've built like this little tool. This should now work in general.** Right.
> Let's run this. It should take this idea this card, and then put it into a prompt ... **and then this thing
> can be used all the time.**"

> "This is how we start to really **build again the infrastructure of these tools.** And we can see that
> **this isn't just for one thing, it can be for many.**"

⚠️ **What it holds across a swap**, on a clothing example: *"Typically this should keep **this character,
this shirt, these sort of tattoos, these pants, these shoes.**"*

---

### ⭐ Batch processing: two lines in the system prompt

**The whole batching lesson.** To go from one output to ten, change **only two things**:

| # | Change | The line |
|---|---|---|
| 1 | **Ask for ten instead of one** | *"instead of one prompt we're going to ask it to generate ten"* |
| 2 | ⭐ **Add a delimiter to the format** | *"**separate each prompt by a star** ... formatted as a" list, *"prompt one star prompt two star"* |

> "And **that's really all we changed. Everything else is exactly the same.** You're a professional magazine
> photographer. You provide prompt, take in an account, generate ten prompts, format it like this. These are
> the exact rules. Do it like this every time. And here's an example that is going to stay the same."

⭐ **The delimiter is the mechanism.** It is what lets a single text output be cut into ten independent jobs:

> "when we run this, we should get ten prompts instead of one. **And this is how the batch starts** ... you
> can see ten prompts in here. And **they're all separated by this little star.**"

#### Splitting them: the array node

> "when we want to split these into individual prompts. So we can run them at the, you know, the same time
> we're going to have to go and add **what's called an array**. Now, what an array is, is basically **it's
> going to take these prompts and split them out** ... as you can see up here **it's a split by comma. But
> we don't want it to be split by comma. We want it to be split by a star.**"

⛔ **Change the delimiter to match the system prompt.** *"that asterisk is what's going to once we put it in
here, **that's going to make it split**."*

⭐ **Why an asterisk and not a comma:** prompts are full of commas. **The delimiter has to be a character
the content will never contain**, which he does not say outright but is the reason his choice works.

#### Running all ten

| Way | How | His verdict |
|---|---|---|
| ⭐ **Text iterator** | *"you just have to pull into here. It'll show you all your prompts"*, attach the image model, run | ⭐ *"**this is the easy way to do it**"* — *"all ten have just showed up in here"*, *"all going to be generated in one shot"* |
| **List selector** | *"you can basically select one of each ten prompts. If I wanted to see all of these at once ... **I just duplicate this ten times**"*, then *"run them each two individual"* model nodes | *"the hard way"* — ⚠️ ten nodes to maintain instead of one |

⛔ **And the connection warning applies here too:** *"we have to make sure of course that **we attach our
image.**"*

---

### ⭐ App mode, and hiding the logic

The step that makes a workflow usable by someone who did not build it.

> "what's called **app mode.** So **you don't have to look at all of these spaghetti strings** like you're
> seeing here. We can make this pretty simple so that **you'll see it'll only show you what you can input**,
> which is I can only input this, which is the product photo. And this is my prompt."

> "That's basically it. **You hit rerun 20 new images come up because you've already built the system. Now
> you just need to go and watch it work.**"

⭐ **What to expose and what to hide:**

| Expose | Hide |
|---|---|
| The **user prompt** | ⛔ The **system prompt** |
| The **product image** | The node graph |

> "A lot of times **if you're sending this to your team**, you're doing this yourself, **you don't want to
> have the system prompt.** That's just working here. **That's something you don't want it to be edited.**"

⭐ **That is a real engineering instinct and worth naming as one:** the system prompt is the tool's logic, not
its input. Exposing it turns a reliable tool back into a prompt box, which is what the whole course is trying
to escape.

---

### ⭐ Pointing the finished tool at a new brand

Once the workflow exists, **one variable changes** and everything else stays put.

> "The best thing about this tools that **we've built this thing now and it's going to work the same way
> every time.** Because again, as we showed in the last example, we just have to upload an image. We have to
> create a prompt. This will have our custom instructions, which has great prompts like this. And **a visual
> brand profile is the only thing that really needs to change in all of this**, right?"

> "So if we want to do this for a different brand, **we just have to change the visual brand profile** ...
> Totally different visual profile. **This is as simple as it gets.**"

⭐ **Building that profile is its own skill**: `aca-build-visual-brand-profile`.

**Once it is swapped, the tool takes plain-language briefs:**

> "we can go and just prompt for whatever we're looking for. Right. Whether that's something maybe that's a
> little bit more fun, maybe something is a little bit more luxury, something that's a little bit more
> textured like this. **There's no end to this.**"

⭐ **And the output stays on-brand without being told to**, because the profile is doing that work:

> "everything we're doing here is just **built on the brand principles. It's already has, like the brand
> style got attached. It's already going to create ten new prompts for you. It's already going to keep the
> product pretty much consistent.**"

⚠️ **How fast:** *"this is all happening within **maybe five minutes**"*.

---

### ⚠️ What comes out is raw

⛔ **The most important caveat in the course, and it is easy to miss because it arrives late:**

> "I would consider **all of these raw assets that you're going to have to sort of doctor up in your own
> way.**"

⭐ **So the workflow removes the repetition, not the craft.** It replaces the tab-switching and the
one-at-a-time prompting; it does not replace the designer, and the course never claims it does.

⚠️ **Judge output by the batch, not the item:** the argument for generating thirty is that you *"pick the
winners"*, which means most of any run is discarded by design.

## Provenance

### Source

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

### ⛔ ACA's own file contains the transcript twice

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

### ⚠️ The course number

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

### ⭐ How this course sits against Course 802

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

#### ⚠️ And the two courses appear to contradict each other on prompt length

| Course 802 | Course 803 |
|---|---|
| ⛔ *"don't start with full sentences"*, *"use stronger keywords or phrases"* | ⭐ *"Each prompt should aim to be highly descriptive. **Minimum of 250 to 350 words**"* |

⭐ **They are reconcilable and the reader needs to be told how**: 802's token style is written for Midjourney,
which weights tokens; 803's word count is written for natural-language models, and Course 802 itself says Flux wants
natural-language prompting with longer prompts. **The rule is the target model, not a
change of mind.** ⚠️ **Neither course states this**, so a reader who takes both at face value will conclude
one is wrong.

---

### ⚠️ The worksheet, and what it is not

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

### ⚠️ Transcription artifacts

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

### The numbers, and what each is worth

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

### ⚠️ Named brands and tools

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

### What is quoted and what is organised

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

### ⚠️ How old this material is

**ACA stamps no recording date.** Received into this library in **2026-W31**, a "no later than".

⭐ **Internal evidence dates it after Course 802**: it treats in-context editing models as the current shift,
names Gemini 2.5, and describes the node tool as *"joining Figma"* but not yet integrated.

⛔ **What dates fastest:** every tool name, the node editor's UI, every model in the picker, the *"five
minutes"* and *"30s"* timings, and the claim that in-context models are new.

⭐ **What is durable:** the three core skills, keep-this-change-that, the six parts of a system prompt with
limits as the critical one, everything-must-be-connected, test-before-batch, the delimiter mechanism,
hide-the-logic, and *"we have to think in batch"*. ⚠️ **None of these depends on a tool**, which is the
argument the course makes for itself.

### Scope

Building the machine. ⛔ **No metric, benchmark or performance claim appears anywhere.** What to test is
Course 602; what the numbers mean is Courses 402 and 701; what the ad should say is Course 401; how much
creative an account needs is Courses 601 and 703. ⚠️ **And what comes out is raw** — *"all of these raw assets
that you're going to have to sort of doctor up in your own way."*

### Credit

Ad Creative Academy's curriculum and Rory Flynn's teaching are their own work. This skill organises that
material for reference; it does not originate it.
