# Ad Creative Academy — Claude skills

**Forty-four Claude skills built from the Ad Creative Academy curriculum.** Every numbered course
from the 100-Level to the 800-Level has one, plus one for each worksheet that produces something.

Install them and Claude can teach the courses, run the worksheets, and produce ACA's documents for a
real brand.

**Pick your setup:** [Claude Code](#installing-to-claude-code) · [the Claude app](#installing-to-the-claude-app)

---

## Installing to Claude Code

**All forty-four in one command.** From the project you want them in:

```bash
npx skills add Creative-Strategy-Systems-ESL/ACA-Skills
```

That copies every skill into `.claude/skills/`. Start a session and ask *"which ACA skills do I
have?"* — you should get **44**.

### Or by hand

Download the repo (green **Code** button → **Download ZIP**), unzip it, and copy the `aca-*` folders
into `.claude/skills/` — either inside a project, or into `~/.claude/skills/` to have them
everywhere:

```
your-project/
└── .claude/
    └── skills/
        ├── aca-100-course-outline/
        ├── aca-101-tribe-building/
        └── … 42 more
```

⚠️ **Copy the `aca-*` folders themselves.** Skills are found at exactly
`.claude/skills/<skill-name>/SKILL.md`. Nested one level too deep — as
`.claude/skills/ACA-Skills-main/aca-101-tribe-building/` — they load silently as nothing, with no
error message.

---

## Installing to the Claude app

**One skill per upload.** That is the app's rule, not a quirk of this repo: its uploader accepts a
zip containing *exactly one* top-level folder and *exactly one* `SKILL.md`. No archive of several
skills will ever go in, however it is packaged.

So the skills come pre-zipped, one file each. Nothing to compress yourself.

**First, once:** open **Settings → Capabilities** and turn on **Code execution and file creation.**
Skills do not run without it.

Then, for each skill you want:

1. **Download the repo** — green **Code** button → **Download ZIP** — and unzip it.
2. Open the **`install`** folder. It holds 44 zips, one per skill.
3. In Claude, go to **Settings → Customize → Skills → Add → Upload skill.**
4. Drag in one zip. Wait a minute or two for the security scan.
5. Repeat for the next one.

⛔ **Do not upload `ACA-Skills-main.zip`**, the file GitHub hands you. It holds the whole repo, so it
fails the one-folder rule. Unzip it first and use the files in `install`.

⭐ **You almost certainly do not want all forty-four.** Start with four or five that match what you
actually do. Every skill works on its own, so there is no wrong subset —
[`SKILLS-README.md`](SKILLS-README.md) describes each one.

**A good first five:**

| Skill | For |
|---|---|
| `aca-100-course-outline` | The map. Which course covers what |
| `aca-103-creative-fundamentals` | The building blocks every ad is made of |
| `aca-402-key-metrics` | Reading the numbers without overclaiming |
| `aca-build-angles` | Angles for a real offer, across all ten types |
| `aca-analyze-building-blocks` | Taking one ad apart |

---

## Every skill works on its own

- **No dependencies.** No skill needs another skill installed.
- **No order.** There is nothing to run first.
- **Nothing else to upload.** Everything a skill needs travels inside its own folder.

Skills do mention each other — *"for that job, use `aca-402-key-metrics`"* — but only as a signpost.
If you do not have the one it names, nothing breaks; you just do not have that one.

Where two skills carry the same material that is deliberate. `aca-103-creative-fundamentals` and
`aca-build-angles` both hold the ten angle types **precisely so** neither depends on the other.

⚠️ **One exception.** `aca-100-course-outline` is the front door: its job is pointing you at the
right course, so on its own it will name skills you have not installed. Install it alongside others.

---

## The three kinds of skill

Tell them apart by name: a **number** after `aca-` means it follows a course, a **verb** means it
produces something.

| Kind | What it is for | What happens when it runs |
|---|---|---|
| **Teach** · 10 | Learning, and answering questions | Ask in plain words, get an answer. It never makes you fill in a form first |
| **Teach and do** · 17 | Learning by making the thing | Explains the method, asks what the document needs, then produces it |
| **Do** · 17 | Getting the document made | No lesson. Tells you what it needs, asks for anything missing, hands back the finished worksheet |

⭐ **The ones that produce documents ask questions first**, and they are built to refuse to invent:
they will not make up a price, a customer count, a discount, or an ad they cannot see. A missing
input gets a question, not a guess.

---

## Using them

Skills load themselves when they are relevant, so mostly you just describe the problem:

> *"which part of ACA covers hooks"*
> *"break this ad down into its building blocks"*
> *"give me angles for this offer"*

Claude picks the matching skill. You can also name one directly.

---

## What is in here

| | |
|---|---|
| `aca-*/` | The 44 skills. Each is a `SKILL.md` plus a `reference/` folder |
| `install/` | The same 44, pre-zipped one per file, for the Claude app |
| `SKILLS-README.md` | The full index: every skill, what it does, what it needs, what it returns |

Every skill carries a `reference/provenance.md` saying where its material came from and who taught
it. Quotations are verbatim from ACA's own recordings and worksheets — including the transcription
slips, which are flagged rather than silently corrected, so any quote can be checked against its
source.

---

## Credits

All course material is Ad Creative Academy's, taught by their faculty — Mirella Crespi, Seth Godin,
George Mack, Reza Khadjavi, Ashley Vinson, Carlotta Costanzo, Zach Murray, Chloe Rhys, Luke Kostka,
Evan Lee, Udi Avital, Jesse Ketonen and Rory Flynn. Each skill names the faculty member it came
from.
