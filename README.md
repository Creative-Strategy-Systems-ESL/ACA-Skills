# Ad Creative Academy — Claude skills

**The whole ACA course, turned into 44 skills Claude can use.** Every numbered course from the
100-Level to the 800-Level has one, plus one for each worksheet that produces something.

No coding. Nothing to install on your computer. About a minute per skill.

---

## How to add them

### Do this first — once

In Claude, go to **Settings → Capabilities** and turn on **Code execution and file creation.**

Skip this and the skills will upload but never actually run.

### Then, for each skill you want

1. **Download this repo.** Green **Code** button at the top → **Download ZIP.**
2. **Unzip it**, and open the **`Skills`** folder. It holds 44 files, one per skill.
3. **In Claude, go to Settings → Customize → Skills → Add → Upload skill.**
4. **Drag in one file.** Claude runs a security check that takes a minute or two.
5. **Repeat** for the next one.

⛔ **One file at a time.** You cannot upload the folder, and you cannot upload them all at once.
That is Claude's own rule — its uploader accepts exactly one skill per file. Do not try to upload
the ZIP GitHub gives you either; that is the whole repo, and it will be rejected.

---

## Do not add all 44

Pick four or five that match what you actually do. Nothing depends on anything else and there is no
order, so there is no wrong choice. You can always come back for more.

| Start with | What it is for |
|---|---|
| **`aca-welcome`** | **Start here.** What the programme covers, and which skill to open for what |
| `aca-103-creative-fundamentals` | The building blocks every ad is made of |
| `aca-402-key-metrics` | Reading ad numbers without overclaiming |
| `aca-build-angles` | Angles for a real offer, across all ten types |
| `aca-analyze-building-blocks` | Taking one ad apart, piece by piece |

[`SKILLS-README.md`](SKILLS-README.md) describes all forty-four.

---

## Using them

Just describe your problem. Claude picks the right skill.

> *"which part of ACA covers hooks"*
> *"break this ad down into its building blocks"*
> *"give me angles for this offer"*

**They will ask you questions, and that is them working.** The skills that produce a document will
not invent a price, a customer count, a discount, or an ad they cannot see. Anything missing gets a
question rather than a guess, so what comes back is safe to put in front of a client.

### The three kinds

Tell them apart from the name: a **number** after `aca-` follows a course, a **word** means it makes
something.

| Kind | What happens |
|---|---|
| **Teach** · 10 | Ask a question, get an answer. Nothing to fill in first |
| **Teach and do** · 17 | Explains the method, then makes the document with you |
| **Do** · 17 | No lesson. Asks what it needs, hands back the finished worksheet |

---

## If something goes wrong

| What you see | What to do |
|---|---|
| The upload is rejected | You are probably uploading the folder, or the ZIP GitHub gave you. Use the files inside `Skills` exactly as they came |
| The skill is listed but nothing happens | You skipped the setting. Turn on **Code execution and file creation** in Settings → Capabilities |
| Claude does not use the skill | Name it directly — *"use aca-402-key-metrics"* — instead of describing the problem |
| It names a skill you do not have | Expected. `aca-welcome` knows all 44 and points at them whether or not you installed them. Add the one it named, or ignore it |

---

## What is in here

| | |
|---|---|
| `Skills/` | **The 44 files you upload.** One per skill |
| `SKILLS-README.md` | The full index: every skill, what it does, what it needs, what it returns |

Every skill carries a `reference/provenance.md` saying where its material came from and who taught
it. Quotations are word for word from ACA's own recordings and worksheets — including the
transcription slips, which are flagged rather than quietly corrected, so any quote can be checked
against its source.

---

## Credits

All course material is Ad Creative Academy's, taught by their faculty — Mirella Crespi, Seth Godin,
George Mack, Reza Khadjavi, Ashley Vinson, Carlotta Costanzo, Zach Murray, Chloe Rhys, Luke Kostka,
Evan Lee, Udi Avital, Jesse Ketonen and Rory Flynn. Each skill names the faculty member it came
from.
