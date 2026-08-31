# Training custom models

⭐ **The largest block in the course**: modules 5 and 6, 39 minutes of the 2h 18m. This is where the course
moves from Midjourney to Flux inside Krea, because Midjourney cannot do it.

⚠️ **Quotes are verbatim from a spoken transcript.** It renders Krea as *"Kria"* or *"Korea"*, LoRA as
*"Lora"* or *"Laura"*, and jeans as *"genes"*. See `reference/provenance.md`.

---

## Why a custom model, and what it changes

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

## ⛔ The training-data guidelines

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

## ⭐ The data-volume trade-off

> "the more images you have, the more varied your results can be, the less images you have, the tighter the
> results are gonna be. **So the more data, more varied results. Less data, tighter results.**"

⭐ **This is a dial, not a best practice.** Tight is right for a product that must be identical. Varied is
right for a style you want to explore.

---

## The four model types

| Type | Images | What it is for | His notes |
|---|---|---|---|
| **Style** | **10 to 50** | *"think brand aesthetic, a lot of lifestyle images"*, and B-roll source imagery | ⭐ *"I would look to have broader situations here, so not every person is the same or they're doing the same thing ... **because you're looking for the overall style, so style's more general than a product**"* |
| **Object** | **10 to 20** | One product, replicated | ⛔ *"I wouldn't use a pair of red sneakers and white sneakers in a training dataset **because they're just gonna mash it together**"* |
| **Character** | **5 to 20** | *"characters or subjects that can be a person, that can be a dog"*, or a brand mascot | *"you're gonna wanna have the same person in that"* |
| ⭐ **Default** | **5 to 100** | *"the default, which is where I like to live in Korea, because it's pretty versatile"* | *"It can be multiple people. It can be a mix of lifestyle and product, multiple environments."* |

### ⛔ Before training a character model on a person

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

### ⭐ Two failure modes he demonstrates on himself

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

## ⛔ Fashion needs one model per colourway

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

## The Krea training settings

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

## ⭐ Whether a brand is even trainable

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

## Prompting a trained model

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

## ⭐ What to iterate, once one prompt works

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

## ⚠️ Post-processing is not optional

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

## Krea's editor, and swapping a trained object in

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
