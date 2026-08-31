# Ad Creative Academy skills

Claude skills built from the Ad Creative Academy curriculum. Each one carries a course's method so
Claude can teach it, run it, or both, without anyone having to re-read the source material.

**Forty-four skills.** Twenty-seven course skills and seventeen worksheet skills. ⭐ **Every course in the
programme now has a skill: the 100- through 800-Levels are complete.** Only the 900-Level certification
has nothing, because no material for it exists. The coverage table below says what each level holds.

Everything here is derived from ACA's own courses, worksheets and prompt packs, credited to the
faculty who taught them. Each skill carries a `reference/provenance.md` naming its source.

⭐ **Every skill also carries a numbered sequence** — a `## How to run it` or `## How to work through
it` section giving the order to take someone through the material, with the artifact produced at a
numbered step where the skill produces one.

## Installing

Skills are picked up from a `.claude/skills/` directory. Two ways to use these:

**Per project.** Copy the skill folders into `.claude/skills/` at the root of the project you are
working in. They become available in that project only.

```
your-project/
└── .claude/
    └── skills/
        ├── aca-100-course-outline/
        └── ...
```

**For every project.** Copy them into `~/.claude/skills/` instead, and they are available
everywhere.

Copy whole folders. A skill is its `SKILL.md` plus its `reference/` directory, and it needs both.

⚠️ **Copy the skill folders, not a whole `.claude/` directory.** A `.claude/` folder can also hold
`settings.json`, hooks and other project configuration that has nothing to do with these skills, and
copying it wholesale would overwrite yours. The forty-four `aca-*` folders and this README are the entire
deliverable; anything else you find alongside them is not part of it.

### Check it worked

Start a new session in that project and ask **"which ACA skills do I have?"** You should get **forty-four**.
Fewer, or none, almost always means the folders are nested one level too deep — see the warning
above. (If you were given a partial set on purpose, count what you were sent rather than this number.)

⚠️ **Keep the folders flat inside `.claude/skills/`.** Skills are discovered at exactly
`.claude/skills/<skill-name>/SKILL.md`. Grouping them into subfolders like
`.claude/skills/teaching/aca-101-tribe-building/` means they are never found and silently never
load, which is hard to notice because nothing errors.

## Using them

Skills load themselves when they are relevant, so most of the time you just describe your problem:
"which part of ACA covers hooks", "break this ad down into its building blocks", "give me angles for
this offer". Claude picks the matching skill.

You can also name one directly if you want a specific one.

### Every skill tells you what it needs

Each `SKILL.md` opens with **What this skill needs from you**, so you can see what you will be
asked for before anything runs. The three kinds behave differently on purpose:

| Kind | What happens when it runs |
|---|---|
| **teach** | Answers or explains straight away. It lists context that would make the answer more specific to you, but it will never hold an answer hostage to a questionnaire |
| **teach + do** | Explains the method first, then asks for what the artifact needs, then produces it |
| **do** | Tells you its inputs, asks for whichever are missing, then produces the artifact |

The "do" skills ask rather than assume. If one needs your price point and you have not given it,
it will ask. That is deliberate: a guessed input produces a confident, wrong artifact that reads
exactly like a right one.

### How to read the quotations

**Quote marks mean your faculty's own words, verbatim.** Anything in `"quotes"` — inline or in an
indented block — is transcribed exactly as it was said or written in your course material, down to
the mid-sentence restarts and the odd transcription slip. Where the recording renders a name or a
word strangely, a ⚠️ note says what the source says against what was meant. Nothing is tidied up
silently, because a quotation that has been smoothed is no longer evidence of what the course
teaches.

**Italics and `backticks` mean our own example**, written to illustrate a point — a sample line of
ad copy, a persona phrase, a template like `X will outperform Y, because Z`. They are not quotations
and are not attributed to anyone.

⚠️ **Bracketed capitals are blanks to fill**, as in `[PRODUCT NAME]`. Where a worksheet in your
material named a specific brand or person, the skill carries the field and not the name.

## What is here

Three kinds of skill, told apart by their names. A **number** after `aca-` means a course skill; a
**verb** means it produces something.

### Course skills

One per ACA course. `teach` skills explain a method; `teach + do` skills explain it and then
produce that course's artifact.

| | Skill | Course | Faculty | Kind |
|---|---|---|---|---|
| ✅ | `aca-100-course-outline` | 100 · Welcome & Course Outline | Mirella Crespi | teach |
| ✅ | `aca-101-tribe-building` | 101 · Tribe Building on Social Media | Seth Godin | teach |
| ✅ | `aca-102-state-of-paid-social` | 102 · State of Paid Social & Consumer Psychology | Mirella Crespi | teach + do |
| ✅ | `aca-103-creative-fundamentals` | 103 · Creative Fundamentals | Mirella Crespi | teach + do |
| ✅ | `aca-104-terrible-great-ads` | 104 · How to Make Terrible Great Ads | George Mack | teach |
| ✅ | `aca-105-ai-powered-strategist` | 105 · The AI-Powered Creative Strategist | Reza Khadjavi | teach |
| ✅ | `aca-201-meta-ads` | 201 · Mastering the Essentials of Meta Ads | Ashley Vinson | teach |
| ✅ | `aca-202-creator-advertising` | 202 · Creator Advertising: The Strategy Before the Brief | Ashley Vinson | teach + do |
| ✅ | `aca-210-tiktok-ads` | 210 · TikTok Ads Essentials | Mirella Crespi | teach |
| ✅ | `aca-230-cross-channel` | 230 · Cross Channel Strategies | Carlotta Costanzo | teach + do |
| ✅ | `aca-301-reverse-engineering-ads` | 301 · Reverse Engineering Winning Ads | Zach Murray | teach + do |
| ✅ | `aca-302-research-for-creative-strategy` | 302 · Research for Creative Strategy | Mirella Crespi | teach + do |
| ✅ | `aca-401-brief-development` | 401 · Brief Development | Mirella Crespi | teach + do |
| ✅ | `aca-402-key-metrics` | 402 · Key Metrics, Thumbstop & CTR Tactics | Chloe Rhys | teach + do |
| ✅ | `aca-403-storyboarding` | 403 · Storyboarding | Mirella Crespi | teach + do |
| ✅ | `aca-404-viral-short-form` | 404 · Engineering Viral Short-Form Content | Luke Kostka | teach + do |
| ✅ | `aca-501-content-production` | 501 · Content Creation & Production | Mirella Crespi | teach + do |
| ✅ | `aca-502-ugc-talent` | 502 · How to Cast and Direct UGC Talent Effectively | Chloe Rhys | teach + do |
| ✅ | `aca-601-launching-campaigns` | 601 · Launching Ad Campaigns | Mirella Crespi | teach + do |
| ✅ | `aca-602-creative-testing` | 602 · Creative Testing Best Practices | Carlotta Costanzo | teach + do |
| ✅ | `aca-701-creative-analysis` | 701 · Creative Analysis & Optimization | Evan Lee | teach |
| ✅ | `aca-702-growth-creative-machine` | 702 · Building a Growth Creative Machine | Udi Avital | teach |
| ✅ | `aca-703-sprint-planning` | 703 · Sprint Planning & Creative Volume | Chloe Rhys | teach + do |
| ✅ | `aca-704-growth-operating-system` | 704 · The Growth Creative Operating System | Mirella Crespi | teach |
| ✅ | `aca-801-ai-creative-strategy` | 801 · AI-Powered Creative Strategy | Jesse Ketonen | teach |
| ✅ | `aca-802-ai-image-video-ads` | 802 · Prompt to Production: AI-Generated Image & Video Ads | Rory Flynn | teach + do |
| ✅ | `aca-803-creative-automation` | 803 · The Creative Automation Workshop | Rory Flynn | teach + do |

### Worksheet skills

The worksheets and prompt packs, each lifted out so it can be run on its own against a real brand.

| | Skill | Produces | From |
|---|---|---|---|
| ✅ | `aca-map-consumer-psychology` | A filled Consumer Psychology worksheet for a brand | Course 102 |
| ✅ | `aca-analyze-building-blocks` | One ad broken into its building blocks, ending in its reusable formula | Course 103 |
| ✅ | `aca-build-angles` | Angles for an offer across all 10 angle types, plus the testing plan | Course 103 |
| ✅ | `aca-find-cross-vertical-inspiration` | A cross-vertical research plan: unexpected industries chasing your audience, and what to verify | Course 230 |
| ✅ | `aca-reverse-engineer-ad-script` | One brand's winning script rewritten natively for another, same beats, every line original | Course 301 |
| ✅ | `aca-audit-ad-account` | A filled Quick Performance Analysis or In-Depth Creative Audit. ⛔ Needs exported data | Course 302 |
| ✅ | `aca-build-audience-personas` | Personas with a Creative Translation column, built from mined customer language | Course 302 |
| ✅ | `aca-analyze-competitor-creative` | A worksheet per competitor plus the five-slide deck, with inference marked as inference | Course 302 |
| ✅ | `aca-plan-creative-sprint` | ACA's 28-column sprint board filled. ⛔ Emits structure only, never ACA's client data | Course 703 |
| ✅ | `aca-name-creative-assets` | ACA's 3-sheet Ad Naming Convention Generator, with its code collisions fixed and flagged | Course 601 |
| ✅ | `aca-track-creative-tests` | ACA's 19-column Creative Testing Tracker filled, with the 3 fields it omits flagged | Course 602 |
| ✅ | `aca-plan-creative-volume` | How much creative an account needs at its spend level, with both recordings' numbers | Course 601 |
| ✅ | `aca-run-creative-qa` | ACA's 8-page Creative QA Checklist filled against a real asset. ⛔ Needs the asset | Course 501 |
| ✅ | `aca-brief-ugc-creator` | A UGC casting call, and ACA's Content Creator Brief filled for a real brand | Course 502 |
| ✅ | `aca-research-trends` | A trend placed as Moment/Signal/Force, relevance-tested, and rebuilt as a template | Course 302 |
| ✅ | `aca-write-ai-image-prompts` | Filled image and video prompts in ACA's formulas, the parameter block, and the iteration plan | Course 802 |
| ✅ | `aca-build-visual-brand-profile` | A Visual Brand Profile in ACA's six sections, plus the system prompt that consumes it | Course 803 |

✅ shipped in this folder · ⬜ planned, not here yet. Check which folders are actually present
before relying on one; the table says what is planned, the folder listing says what you have.

#### These four ask before they invent

Each carries a rule about the input it can be given, because each has a different way of producing
something that looks right and is not:

- **`aca-map-consumer-psychology`** separates research *supplied* from research merely *named*
  ("we have 400 reviews" is not the reviews), and separates a client's facts from a client's
  unverified assertions. It ends every worksheet with a **claims register**, because a provenance
  note on a section does not travel with the one line somebody copies into an ad.
- **`aca-analyze-building-blocks`** will not tear down an ad from a link or a brand name. A teardown
  is written in the language of observation, so an invented one is indistinguishable from a real
  one. It asks for a description first, and marks what it could not see rather than scoring it.
- **`aca-build-angles`** keeps ACA's `[BRACKETS]` where a fact is missing instead of filling them.
  Nine of the ten angle types invite a specific invention: a discount, a customer count, an
  endorser, a competitor's weakness, a mechanism. The bracket plus a note of what is needed is the
  deliverable, and it doubles as a list of what to go and find.
- **`aca-find-cross-vertical-inspiration`** treats every brand it names as a **research target, not
  a finding.** The underlying prompt asks a model to name specific companies in industries it has
  not researched, and it will — some real and accurate, some real but wrong, some neither, all in
  the same tone. The skill delivers a verification plan alongside the list and marks the list
  unverified inside the document, where the marking survives being pasted into a deck.

### Course skills and worksheet skills overlap on purpose

`aca-102` and `aca-map-consumer-psychology` both carry the Consumer Psychology worksheet.
`aca-103`, `aca-analyze-building-blocks` and `aca-build-angles` all carry the building blocks and
the ten angle types. That is deliberate: **every skill has to work with none of the others
installed**, so none of them can point at a sibling for its content.

The split is by job, not by subject:

| You want to | Use |
|---|---|
| Understand the method, or answer a question about it | the **course** skill |
| Run it on a real brand, a real ad, or a real offer | the **worksheet** skill |

Asking a worksheet skill what an angle is gets you interrogated about your product. Asking a course
skill to produce a worksheet gets you taught first. Both work; the routing above is faster.

### Start here

`aca-100-course-outline` is the front door. It holds the full curriculum map (all 26 courses, who
teaches them, how long they run, what modules they contain) and routes to whichever skill fits the
question. If you are not sure which skill you want, ask it.

## Coverage

⭐ **All twenty-six courses are covered.** The only gap is the 900-Level certification, for which ACA has
sent no material at all.

| Level | Courses | Skills |
|---|---|---|
| 000 · 100 | 100, 101, 102, 103, 104, 105 | ✅ **complete — all 6 course skills and all 3 worksheet skills** |
| 200 · Platforms & Channels | 201, 202, 210, 230 | ✅ **complete — all 4 course skills and 1 worksheet skill** |
| 300 · Research & Insights | 301, 302 | ✅ **complete — both course skills and all 5 worksheet skills** |
| 400 · Creative Strategy & Ideation | 401, 402, 403, 404 | ✅ **complete — all 4 course skills** |
| 500 · Content Creation & Production | 501, 502 | ✅ **complete — both course skills and 2 worksheet skills** |
| 600 · Creative Testing | 601, 602 | ✅ **complete — both course skills and 3 worksheet skills** |
| 700 · Performance Analysis & Iterations | 701, 702, 703, 704 | ✅ **complete — all 4 course skills and 1 worksheet skill** |
| 800 · AI-Powered Creative Strategy | 801, 802, 803 | ✅ **complete — all 3 course skills and 2 worksheet skills** |
| 900 · Certification | exam, capstone | not yet |

`aca-100-course-outline` knows the whole curriculum, including the levels with no skills yet, so it
can still tell you which course covers a topic and who teaches it.

## A note on course numbers

ACA renumbered its courses for launch, and material made before the renumber uses the old codes. A
bare "course 301" can mean two different courses depending on which numbering someone has in front
of them. These skills use the **current shipping** numbers throughout, and
`aca-100-course-outline` explains the overlaps. When a number is ambiguous, naming the instructor
settles it, because the faculty did not change when the numbers did.
