# The formulas, filled

---

## ⭐ Both sources agree on the structure

The recording and the course's cheat sheet were made separately and **state the same three things**, which
is the strongest corroboration in the 800-Level:

| | The recording says | The cheat sheet says |
|---|---|---|
| **The rules** | Don't use full sentences · strong keywords · powerful language · one subject · tell it a story | *"01. Don't use full sentences · 02. use strong keywords · 03. separate key elements with commas · 04. use powerful language · 05. Focus on one subject · 06. Tell midjourney a story"* |
| **The slots** | Photo type · shot type · subject and action · environment · colour scheme · camera details · lighting · composition · additional | *"Photo Type Shot Type Subject Environment Tech Details Lighting Modifiers"* |
| ⭐ **What to hold and flip** | *"all we have to do is flip the photo type, the subject and the action and the environment"* | *"**keep:** Color scheme, technical details, composition, lighting, modifiers / **Change:** Shot type, Subject + Action,"* Environment |

⛔ **They disagree about nothing except the parameters**, which appear only on the sheet. See
`reference/provenance.md`.

---

## The image prompt, eight slots

**Emit in this order, comma-separated, no full sentences.**

| # | Slot | ⭐ Signature or variable | What goes in it |
|---|---|---|---|
| 1 | **Photo type** | 🔁 Variable | cinematic still · editorial photo · product shot · flat lay · closeup |
| 2 | **Shot type / composition** | 🔁 Variable | closeup · wide · drone · front view · side · rear · diagonal · overhead |
| 3 | **Subject and action** | 🔁 Variable | who or what, and what it is doing |
| 4 | **Environment** | 🔁 Variable | the location or context |
| 5 | **Colour scheme** | 🔒 **Hold** | the brand palette, named as colours not hex |
| 6 | **Camera and technical details** | 🔒 **Hold** | camera body · lens · film stock · settings |
| 7 | **Lighting** | 🔒 **Hold** | see the lighting list below |
| 8 | **Composition and modifiers** | 🔒 **Hold** | balance, lines, plus *"sharp crisp detail"* |

⭐ **Slot 4, environment, sits on the boundary.** The recording flips it; the cheat sheet's "change" list
ends mid-phrase but the diagram places Environment with the changeable group. **Treat it as variable, and
say so**, because moving a product from studio to outdoors is usually the point.

**ACA's worked example**, which is the shape to match:

> "cinematic still of a Haggard man sitting in a grungy East Village dye bar, brown and burgundy colors,
> 35 millimeter film, backlight, off-balance composition, and loneliness is our emotion"

⚠️ *"dye bar"* is the transcript's rendering of *dive bar*.

### The order matters, and the source contradicts itself about how

The cheat sheet states a token-position rule the recording never mentions:

> "Beginning of prompt: Midjourney places the most focus on these tokens. end of prompt: Midjourney places
> the least focus on these tokens."

⛔ **Then its own diagram labels read the other way**: *"End of Prompt More Importance / Beginning of
Prompt Less Importance"*. **The sheet contradicts itself, or the two labels are axis captions that cannot
be resolved from the artifact.** Either way it is unresolved in the source.

⭐ **What to do about it:** put the load-bearing tokens **early**, which is what the sheet's prose says and
what the recording's token-weight demonstration implies, and **do not present the rule as settled.** If
output emphasis looks wrong, reordering the prompt is a legitimate thing to try.

---

## ⭐ The iteration plan

**This is the deliverable.** One prompt plus a plan is a library; one prompt alone is one image.

**Emit it as a table**: the five held slots written out once, then five to ten variants that change only
the four variable slots.

> "**we're isolating the variable within the prompt** ... you can keep everything else the same if you
> want to ... **you can then go and do this into infinity**"

⭐ **Rory's worked variant set off a single reference image** shows the pattern: same signature, swap the
subject and action each time — a racing car on a hill becomes a skier, a motorcyclist, a dune buggy.

⚠️ **And name the debugging move**, because it is the reason the slots are named at all: *"if I know I
listed out my lighting as mid-day lighting, but it's way too bright, maybe I can just go back in for the
iteration process and switch that."*

---

## The video prompt, six slots

| # | Slot | What goes in it |
|---|---|---|
| 1 | **Shot type** | handheld · cinematic · dynamic · fast action |
| 2 | **Subject and their details** | including what they are wearing, even if the image shows it |
| 3 | ⭐ **Camera motion** | one of the nine below |
| 4 | ⭐ **Direction** | which way. ⛔ *"if I just said the camera tracks, it could track forwards, it could track anyway"* |
| 5 | **Mood and atmosphere** | |
| 6 | **Captured in a style** | *"reminiscent of a professional fashion photo shoot shot in cinematic 4K"* |

**ACA's worked example:**

> "a handheld shot of a man modeling khaki pants in a studio environment ... Then the camera follows the
> man as he moves, as he models the pants in various poses. The camera stays fixed on his pants as he does
> a full 360 degree turn. The scene is playful, reminiscent of a professional fashion photo shoot shot in
> cinematic 4K."

⛔ **Write video prompts in natural language, not tokens**, and be more detailed than for images: *"it can
take your words and interpret them very wrong if you're not doing it that way."*

⛔ **Motion is the load-bearing slot.** *"Camera and subject motion are the most important. That's how the
whole scene is developed ... **But if you don't have the motion, obviously it doesn't look like a
video.**"*

### The nine camera motions

**static** · **panning** (left to right on an arc) · **tilting** (up or down) · **tracking** (following a
moving subject) · **trucking** (parallel, alongside) · **arcing** (around, ~180°) · **pedestal or crane**
(changing level) · **dolly push in / pull out** · **orbit** (360°)

⭐ **The cheat sheet carries the same vocabulary**, listing tracking, trucking and arcing among its camera
movements, so the two sources agree here too.

### ⛔ Add an interaction clause

The highest-value line in a video prompt, and the one most often missing. Every one of these is ACA's own
example of a fix:

| If the scene has | Add |
|---|---|
| Someone running | *"his hair is flowing in the wind"* |
| Someone in water | *"the water drips from his body"* |
| Someone holding something against force | *"holding poles that are anchoring him in a raging river"* |
| Steam, smoke or liquid near a body | *"flows **around** his body"*, never through |
| A current or flow | *"the stream is flowing **towards us**"* |
| Drinking from a straw or cup | *"as she tilts her head down to sip from a straw"* |

> "this is a way that you can quickly tell that things are AI is when things just **unnaturally interact
> with each other**"

---

## ⭐ If the still becomes video, change the still

**Ask this before writing the image prompt.** Motion tokens go in the *image* prompt.

| Add to the image prompt | Because |
|---|---|
| **motion blur** | a static subject has to be animated from nothing |
| **spinning wheels** | otherwise *"the car just sort of glides across the sand, doesn't drive"* |
| **freeze motion** | ⭐ a subject caught mid-action continues naturally |
| A subject already mid-stride | *"a natural progression is for it to just go down and to keep"* walking |
| **cheering**, a blurred crowd | gives a background implied life instead of frozen extras |

⛔ **And the debugging rule:** *"if you just can't get something you've run it through all those features
**the image is usually the problem**"*.

---

## The parameter block

⛔ **Source boundary: every parameter below comes from the course's Midjourney cheat sheet. None of them
is mentioned anywhere in the recording.** Emit them as a separate labelled block so they can be dropped
whole for a non-Midjourney tool.

| Parameter | Use, in the sheet's words | Range | Default | Format |
|---|---|---|---|---|
| `--ar` | Aspect Ratio | | | `--ar 5:6` |
| `--s` / `--stylize` | *"Changes how "artistic" this image is."* | 0-1000 | 100 | `--s 750` |
| `--q` / `--quality` | *"Changes time spent rendering the image."* | 1, 2, 4 | 1 | `--q 4` |
| `--c` / `--chaos` | *"Changes how varied the image grids are."* | 0-100 | 0 | `--c 50` |
| `--exp` | *"Gives images dynamic aesthetics."* | 0-100 | 0 | `--exp 50` |
| ⭐ `--sref` | *"Transfer aesthetics between prompts."* | up to 3 image links | N/A | `--sref [url 1] [url 2]` |
| `--sw` | *"Changes sref effect on the prompt."* | 0-1000 | 100 | `--sw 500` |
| ⭐ `--oref` | *"Transfer character/object between imgs."* | image link | N/A | `--oref [url 1]` |
| `--ow` | *"More/less object influence on prompt ."* | 0-1000 | 100 | `--ow 50` |
| `--iw` | *"Adjust weight of the image vs. text prompt."* | 0-3 | 1 | `--iw 2` |
| `--no` | *"Removes unwanted elements."* | any word | N/A | `--no words` |
| `--r` / `--repeat` | *"Create multiple jobs for one prompt."* | 2-40 | 0 | `--r 4` |
| `--tile` | *"Images that can be used as patterns."* | N/A | N/A | `--tile` |
| `--stop` | *"Finish a job partway through the process."* | 10-99 | 100 | `--stop 50` |
| `--v` | *"Changes the MJ Version used to generate."* | 1-6 | 6 | `--v 2` |
| `--seed` | *"starting point to generate the initial image"* | 0-4294967295 | N/A | |
| `--style raw` | *"Makes images look more natural."* | | | `--style raw` |
| `--weird` | *"Gives images experimental looks."* | | | `--weird <value>` |
| `--sv` | *"Changes the SREF version."* | | | |
| `--sref random` | *"Produces a unique style code."* | | | |
| `--p` / `--profile` | Personalize | | | |
| `--draft` | *"Faster generations + lower cost"* | | | `--draft` |

⭐ **The three that actually matter for brand consistency:** `--sref` to carry an aesthetic across prompts,
`--sw` to dial how hard it lands, and `--oref` to carry a specific object or character. Those three do in
one flag what asset cloning does in five steps, when you have a usable reference image.

⭐ **The sheet's own iteration tip:** `--r 40` to fan out wide, `--r 2` to narrow; `--iw 0` for *"Close to
Text"* and `--iw 3` for *"Close to Image"*.

---

## ACA's vocabulary lists

⭐ **Use these rather than inventing descriptors.** They are the course's own, and slots 6, 7 and 8 are
where prompts usually go vague.

**Lighting and mood:** Soft Light *(diffused, low shadows)* · Hard Light *(harsh, strong shadows)* ·
Natural Light · Ambient Light *(broad, no-source glow)* · Backlit *(halo from behind)* · Sidelit *(adds
depth)* · Frontlit *(low shadows)* · Toplit *(downward shadows)* · Underlit *(eerie light from below)* ·
Golden Hour

**Composition:** Leading Lines *(guides focus)* · Horizontal Lines *(calm)* · Vertical Lines *(strength,
elevation)* · Symmetrical · Asymmetrical *(equal weight, different elements)* · Balance · Colour Balance ·
Tonal Balance · Colour Blocking *(bold contrasts)* · Selective Colour *(one colour pops, rest
grayscale)* · Colour Harmony

**Motion, for stills that become video:** Freeze Motion *(sharp moving shots)* · Motion Blur *(intentional
blur)* · Panning *(camera moves, subject stays sharp)* · Light Trails *(low-light streaks)* · Ghosting ·
Bokeh Motion *(blurry lights in motion)*

**Photography style:** Editorial/Magazine *(stylish, polished, high-end)* · Documentary *(real-life,
storytelling)* · Street Style *(urban)*

**Colour film stocks**, each with the look it produces: Kodak Ektachrome *(lifelike, rich colours)* ·
Fujifilm Provia *(balanced, natural)* · Fuji Velvia 50 *(vivid, high-contrast landscapes)* · Cinestill
800T *(low-light, cinematic tungsten)* · Kodak Aerochrome *(false-colour infrared)* · Polaroid SX-70
*(old-school Polaroid artistry)* · Lomography LomoChrome Purple *(surreal purple shift)* · Lomography
Redscale XR *(red cast, surreal)* · Rollei Infrared 400 *(ethereal, dreamlike)* · Yodica Antares 200
*(saturated, golden hour)* · Adox Color Mission 200 *(muted, vintage)* · AgfaPhoto CT *(crisp, vivid
pop)* · Instax Square SQ6 *(square, bold colours)* · Revolog Texture *(pre-exposed patterns)*

**Black and white stocks:** Foma Fomapan R 100 *(fine-grained, rich)* · Foma Fomapan *(deep blacks, bright
whites)* · JCH Streetpan 120 *(high-contrast, fine-grained)* · Film Washi S *(delicate, dreamy)* ·
Lomography Berlin 400 *(high-contrast)*

**Stills cameras:** Canon 1D X *(fast, rugged DSLR)* · Nikon D850 *(detail beast)* · Sony A7R IV ·
Fujifilm GFX 100 *(ultra-res medium format)* · Leica M10-R *(iconic)* · Hasselblad H6D *(elite medium
format)* · GoPro HERO *(extreme angles)* · Infrared cameras *(spooky, surreal)*

**Cinema cameras:** ARRI Alexa Mini *(compact, large format)* · RED Monstro 8K · Sony Venice *(full-frame,
colour)* · Panavision DXL2 *(big-budget)* · Canon C500 *(full-frame, 5.9K)* · Kodak Super 8 *(modern
nostalgia)* · Krasnogorsk-3 *(16mm, classic)* · Aaton Penelope *(35mm)* · Bell & Howell *(16mm)*

**Lenses:** Canon 24-70mm *(pro zoom, crisp)* · Nikon 70-200mm *(fast telephoto)* · Sony 16-35mm *(wide)* ·
Fujifilm 110mm *(portrait)* · Leica 50mm *(sharp, dreamy prime)* · Lensbaby 56mm *(ethereal glow)*

⚠️ **The named products date.** The *look* each one names is durable; the body or stock may not be current.

---

## The moodboard ladder

⚠️ **Read, not quoted.** This panel of the sheet has a doubled text layer, so the wording below is
de-duplicated rather than quotable. See `reference/provenance.md`.

The sheet ties **how many images you feed a moodboard** to **what kind of style you get back**:

| Images | What you get |
|---|---|
| **1** | An SREF style — one reference's aesthetic |
| **2-10** | A token style |
| **10-20** | ⭐ A branded style |
| **20-50** | An SREF code style |
| **50+** | A compilation style |

⭐ **And the governing rule, which matches the recording exactly:** more images means less consistency;
fewer images means a more defined style. The recording's version: *"more data, more varied results. Less
data, tighter results."*

⭐ **So 10-20 images is the band for brand work**, which is the same range Course 802 gives for training an
object model. Two different mechanisms, same answer.

**The sheet's key moodboard elements:** colour palette (primary/secondary) · imagery
(images/illustrations/renders) · texture (depth/visual direction) · material references (sensory texture and
realism) · lighting and mood (emotional and scene context) · motion.

---

## ⭐ The asset-cloning run sheet

**Emit this instead of guessing a signature, whenever brand images are supplied.**

⛔ **First, the gate.** *"try to only do this on your brand, **don't go do this to other people's
brands**"*. If the images are not theirs, stop and offer the alternative.

| Step | Do | ⚠️ Expect |
|---|---|---|
| **1** | Collect the brand assets and pick the one to build from | Organise first: *"see sort of which one we wanna utilize to build all these other images off of"* |
| **2** | Run it through Midjourney's `describe`. Returns four different prompts | ⛔ **This step fails on its own.** ACA's own verdict on the raw output: *"these look like crap ... looks like video games or like fine arts"*. Do not stop here |
| **3** | ⭐ **Fine-tune in an LLM.** The fix, not polish | Use the instruction below verbatim |
| **4** | Attach the original as a style reference (`--sref`) to the refined prompt | *"using style reference can be way easier than this. **A lot of times it's way harder**"* |
| **5** | Iterate: hold the signature, flip the three variable slots | ⭐ **The prompt is the deliverable**, not the cloned image |

**Step 3's instruction, as ACA gives it:**

> "**analyze the image. We want to create a prompt for an AI image generator** ... We want it to
> **describe it like an award-winning professional photographer in extreme technical details.**"

> "**use this formula to structure the prompt** ... and then **include specific camera lens, camera
> settings, et cetera, be very technically specific, use short and powerful keywords and phrases, do not
> use** full sentences"

⭐ **Why step 3 is worth the extra pass**, in ACA's words: *"That second half of the prompt, **I'm probably
never gonna be able to describe it that way.**"* The technical detail is precisely what a human eye cannot
name and what the signature depends on.

⛔ **And what the output must make explicit:** the prompt is what gets kept.

> "again, the idea isn't to get this image. **We don't wanna copy this image. We just need the prompt. The
> prompt is the piece** because then we can go and iterate on it"
