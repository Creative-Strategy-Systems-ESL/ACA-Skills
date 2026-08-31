# The three core AI skills

⚠️ **Quotes are verbatim from a spoken transcript**, which renders the tool as *"YV"*, *"CV"*, *"weave"* and
*"weaving"*, and LLM as *"LM"* or *"LMS"*. See `reference/provenance.md`.

---

## Why skills rather than tools

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

## ⭐ Skill 1: Deconstruction

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

### ⭐ The edit formula: keep this, change that

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

### ⚠️ In-context editing models, and what they replace

> "the biggest sort of shift in AI is what's called these **In-Context models.** We did we went through a
> little bit of the Laura training stuff, which is how do I take one singular product and do sort of train
> a model on that ... **these image models make it a lot easier.**"

> "these editing image models, right, where you can **just take anything and just say, put this here or
> make this, do this, or change this character's clothes.** It's really easy. **It's natural language, it's
> super simple, it's intuitive now** ... And it's **actually relatively easy in comparison to what we did
> with the Laura training stuff.**"

⛔ **Read that carefully: the same teacher is saying his own Course 802 module on LoRA training is now
largely unnecessary for consistency.** That is not a contradiction to hide — it is the most useful thing in
the course for anyone deciding where to spend a week. See `reference/provenance.md` for how the two courses
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

## ⭐ Skill 2: System prompts

> "Second one is system prompts. System prompts are essentially like **how we tell the LMS what to do and
> how we tell them what to do every time.** So if you're familiar with building like custom GPT, you know,
> again, like you build a custom GPT to just like do this single task every single time."

⭐ **The line that explains why this is a core skill and not a trick:**

> "**So also system prompts are like the precursor to agent.** So it's **how we move things from process to
> process without having to have a human in the loop** with a lot of it. So it just becomes really
> important."

And: *"what they do is they just **guide the output.** You're telling the LM what to do. Every single time.
So it's becomes **controllable and predictable**."*

### The six parts

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

### ⭐ His worked system prompt, a prompt generator

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
802's "do not use full sentences"** — see `reference/provenance.md`, which reconciles them.

⚠️ **He notes this used to be manual work:** *"if you've been in ChatGPT for a long time ... **you used to
have to prompt like this to get a good answer.** Now it's sort of like built as a system."*

---

## ⭐ Skill 3: Workflow development

> "workflow development really is just like, **how do I get from point A to point B? And in what sequence do
> I do it and what tools do I need?**"

⚠️ **He flags this as the least stable of the three:** *"This portion will change. Often it's really about
understanding again **what the tools can do, what their capabilities are.** And then we can start to sort of
like build around it."*

And: *"this is the skill that will be **the most fluid moving forward**."*

**Why he thinks it is where everything is heading:**

> "You're seeing all the tools start to roll out some sort of, you know, **node based system where you can
> use multiple tools in one space** to do certain tasks, and **it's all going to be customizable.**"

### What it buys

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

## ⭐ The end state he is building toward

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
