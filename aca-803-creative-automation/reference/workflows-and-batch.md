# Building the workflow, and batching it

⚠️ **The tool is one implementation.** The three core skills are the portable part; this file is how the
course wires them together in a node editor. ⚠️ **The transcript renders the tool's name as *"YV"*, *"CV"*,
*"weave"*, *"weaving"* and *"Wi-Fi"***, and the models by ear. See `reference/provenance.md`.

---

## Where the tool sits

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

## The node vocabulary

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

## ⛔ The failure mode, which he demonstrates on purpose

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

## The simple version first

**Three nodes:** a product image, a prompt, and an image-editing model.

> "if we wanted to just do this in the basic way, let's just do a prompt right. We'll have our prompts here,
> and then we'll use something like **nano banana** ... This is the simple way we attach our prompt. We
> attach our image."

**And the prompt is the keep-this-change-that formula:** *"keep this exact product and preserve the fine
details change. Put this bottle on a countertop in a high end luxury apartments."*

⚠️ **On aspect ratio:** *"you can also change the aspect ratio. **Most of the time it will just want to use
default. It will default to whatever aspect ratio this is.**"*

---

## ⭐ Adding the system prompt: the auto-prompt tool

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

### His system prompt for it, part by part

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

### ⛔ Test before you batch

> "this is again **the base of where we're going to do this at batch. Like we have to know that this works
> first. We can get good outputs with this system prompt. Then we can go and start doing other things.**"

⭐ **Do not skip this.** Batching a broken system prompt produces twenty broken outputs and costs twenty
generations to find out.

### ⭐ Then it generalises for free

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

## ⭐ Batch processing: two lines in the system prompt

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

### Splitting them: the array node

> "when we want to split these into individual prompts. So we can run them at the, you know, the same time
> we're going to have to go and add **what's called an array**. Now, what an array is, is basically **it's
> going to take these prompts and split them out** ... as you can see up here **it's a split by comma. But
> we don't want it to be split by comma. We want it to be split by a star.**"

⛔ **Change the delimiter to match the system prompt.** *"that asterisk is what's going to once we put it in
here, **that's going to make it split**."*

⭐ **Why an asterisk and not a comma:** prompts are full of commas. **The delimiter has to be a character
the content will never contain**, which he does not say outright but is the reason his choice works.

### Running all ten

| Way | How | His verdict |
|---|---|---|
| ⭐ **Text iterator** | *"you just have to pull into here. It'll show you all your prompts"*, attach the image model, run | ⭐ *"**this is the easy way to do it**"* — *"all ten have just showed up in here"*, *"all going to be generated in one shot"* |
| **List selector** | *"you can basically select one of each ten prompts. If I wanted to see all of these at once ... **I just duplicate this ten times**"*, then *"run them each two individual"* model nodes | *"the hard way"* — ⚠️ ten nodes to maintain instead of one |

⛔ **And the connection warning applies here too:** *"we have to make sure of course that **we attach our
image.**"*

---

## ⭐ App mode, and hiding the logic

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

## ⭐ Pointing the finished tool at a new brand

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

## ⚠️ What comes out is raw

⛔ **The most important caveat in the course, and it is easy to miss because it arrives late:**

> "I would consider **all of these raw assets that you're going to have to sort of doctor up in your own
> way.**"

⭐ **So the workflow removes the repetition, not the craft.** It replaces the tab-switching and the
one-at-a-time prompting; it does not replace the designer, and the course never claims it does.

⚠️ **Judge output by the batch, not the item:** the argument for generating thirty is that you *"pick the
winners"*, which means most of any run is discarded by design.
