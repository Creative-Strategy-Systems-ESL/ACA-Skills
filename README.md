# Ad Creative Academy — Claude skills

**Forty-four Claude skills built from the Ad Creative Academy curriculum.** Every numbered course
from the 100-Level to the 800-Level has one, plus one for each worksheet that produces something.

Download this repo, install the skills, and Claude can teach the courses, run the worksheets, and
produce ACA's documents for a real brand.

---

## ⛔ Read this before you install

**Do not upload this repo's ZIP to Claude.** GitHub's green *Code → Download ZIP* button gives you
a file whose contents are a folder, and Claude's skill upload needs a zip whose contents are a
**skill**. It will be rejected, and it looks like the skills are broken when they are not.

Use one of the two paths below instead. Both take the same download.

---

## Install in Claude (the web and desktop app)

Claude's skill uploader takes **one skill at a time**, so this repo ships every skill pre-zipped
and ready. No zipping, no renaming.

1. **Download this repo.** Green **Code** button → **Download ZIP** → unzip it.
2. In Claude, open **Settings → Capabilities** and turn on **Code execution and file creation.**
   Skills do not run without it.
3. Go to **Settings → Customize → Skills** and click **Add → Upload skill.**
4. Open the **`install/`** folder from your download and pick a `.zip`. That is one skill installed.
5. Repeat for each skill you want. Each takes a moment to pass a security scan before it is live.

⭐ **You do not need all forty-four.** Each one works on its own — see below. Start with four or
five that match what you actually do, and add more later.

### On a Team or Enterprise plan

An owner can upload each skill once under **Organization settings → Skills** and it becomes
available to everyone, so nobody else has to install anything.

---

## Install in Claude Code

Faster, because all forty-four go in at once.

Copy the `aca-*` folders from this repo into `.claude/skills/` — either in a project, or in
`~/.claude/skills/` to have them everywhere:

```
your-project/
└── .claude/
    └── skills/
        ├── aca-100-course-outline/
        ├── aca-101-tribe-building/
        └── … 42 more
```

⚠️ **Copy the `aca-*` folders themselves, not this whole repo folder.** Skills are found at exactly
`.claude/skills/<skill-name>/SKILL.md`. Nested one level too deep, they load silently as nothing.

Start a session and ask *"which ACA skills do I have?"* — you should get **44**.

---

## ⭐ Every skill works on its own

This is the part people expect to be complicated, and it is not.

- **No dependencies.** No skill needs another skill installed to work.
- **No order.** There is nothing to run first.
- **No separate document to upload.** Everything a skill needs is inside its own folder.

Skills do mention each other — *"for that job, use `aca-402-key-metrics`"* — but only as a
signpost. If you do not have the one it names, nothing breaks; you just do not have that one.

Where two skills cover the same material, that is deliberate. `aca-103-creative-fundamentals` and
`aca-build-angles` both carry the ten angle types **precisely so** neither has to depend on the
other.

⚠️ **One exception.** `aca-100-course-outline` is the front door: its whole job is pointing you at
the right course. On its own it will name skills you have not installed. Install it alongside
others, not by itself.

---

## The three kinds of skill

You can tell which is which from the name: a **number** after `aca-` means it follows a course, and
a **verb** means it produces something.

| Kind | What it is for | What happens |
|---|---|---|
| **Teach** · 10 | Learning, and answering questions | Ask in plain words, get an answer straight away. It never makes you fill in a form first |
| **Teach and do** · 17 | Learning by making the thing | Explains the method, asks what the document needs, then produces it |
| **Do** · 17 | Getting the document made | No lesson. Tells you what it needs, asks for anything missing, hands back the finished worksheet |

**`SKILLS-README.md`** in this repo lists all forty-four with what each one does, what it needs from
you, and what it hands back.

---

## How to use them

Skills load themselves when they are relevant, so mostly you just describe the problem:

> *"which part of ACA covers hooks"*
> *"break this ad down into its building blocks"*
> *"give me angles for this offer"*

Claude picks the matching skill. You can also name one directly.

⭐ **The ones that produce documents will ask you questions first**, and they are built to refuse to
invent: they will not make up a price, a customer count, a discount, or an ad they cannot actually
see. A missing input gets a question, not a guess.

---

## What is in here

| | |
|---|---|
| `aca-*/` | The 44 skills. Each is a `SKILL.md` plus a `reference/` folder |
| `install/` | The same 44, pre-zipped one per file, for the Claude app uploader |
| `SKILLS-README.md` | The full index: every skill, what it does, what it needs |

Every skill carries a `reference/provenance.md` saying where its material came from and who taught
it. Quotations are verbatim from ACA's own recordings and worksheets — including the transcription
slips, which are flagged rather than silently corrected, so a quote can always be checked against
the source.

---

## Credits

All course material is Ad Creative Academy's, taught by their faculty — Mirella Crespi, Seth Godin,
George Mack, Reza Khadjavi, Ashley Vinson, Carlotta Costanzo, Zach Murray, Chloe Rhys, Luke Kostka,
Evan Lee, Udi Avital, Jesse Ketonen and Rory Flynn. Each skill names the faculty member it came
from.
