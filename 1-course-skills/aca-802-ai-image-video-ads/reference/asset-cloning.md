# Asset cloning

⭐ **The most transferable idea in the 800-Level.** Course 803 generalises it into a named skill,
"deconstruction", and calls it one of three core AI skills. This is where it is taught concretely.

⚠️ **Quotes are verbatim from a spoken transcript.** The recording renders Midjourney as *"mid-journey"*
and ChatGPT as *"chatgbt"* or *"chat GBT"*; see `reference/provenance.md`.

---

## The problem it solves

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

## ⛔ The disclaimer is part of the method

> "I put this in here as a disclaimer, **try to only do this on your brand, don't go do this to other
> people's brands**, but again, this is all what's possible and how you can think about it."

**Carry this every time the technique is used.** It is Rory's own line, it is unambiguous, and the
technique works just as well on a competitor's imagery, which is exactly why he says it.

---

## What it is

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

## ⭐ The five steps

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

## ⛔ Step 2 fails on its own, and he shows it

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

## ⭐ Step 3: the ChatGPT instruction

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

## Step 4: style reference

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

## ⭐ What you keep is the prompt

The most important sentence in the module, and the one that stops this being image theft:

> "again, the idea isn't to get this image. **We don't wanna copy this image. We just need the prompt. The
> prompt is the piece** because then we can go and iterate on it, right?"

---

## ⭐ The visual signature, and the three slots you flip

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

## ⭐ The mindset, which is why 803 builds on this

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

## What else the technique unlocks

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
