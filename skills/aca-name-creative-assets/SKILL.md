---
name: aca-name-creative-assets
description: Builds a creative naming convention and emits Ad Creative Academy's Ad Naming Convention Generator, all three sheets - the settings tab with its eight tracked dimensions and dropdown values, the generator tab that assembles the name string, and the ad type library of 18 video types, 16 graphic types and 8 triggers. Flags the six naming elements Course 601 teaches that the sheet has no column for, and the defects in ACA's shipped file including two dimensions sharing a code and three inconsistent code sets. Use this when nobody can tell which ads worked because of how they are named, when creative and media teams need a shared convention, when setting up a new account, or when someone asks for a naming convention or UTM structure. Requires knowing what you want to compare later - the convention is designed backwards from that.
---

# Name creative assets

Produces **Ad Creative Academy's Course 601 artifact** — Mirella Crespi's naming generator.

> "Let's start with something that **seems simple but is incredibly powerful**: naming conventions."

⭐ **The convention is designed backwards from the comparisons you want to run.** ACA's own argument:

> "Are image ads working better than video ads? Is UGC working better than studio production? Are ads
> with the VO better than ads with just music? And are funny hooks working better than hooks that
> show the problem first? **You can't answer any of these questions if your creatives are not named
> or tagged effectively.**"

⛔ **Ask what they want to compare before building anything.** A convention assembled without that
question will be missing exactly the field they need, which is what happened to ACA's own sheet.

## What this skill needs from you

**Required:**

1. **What you want to be able to compare later.** The four questions above are the starting set; the
   real ones are whatever this account argues about
2. **Who has to use it** — this is a joint document. *"This is a combined effort between creative
   strategists and media buyers. There's simply no way around it"*

**Optional, and each fills real dropdown values:**

3. The products or bundles being advertised
4. Who produces the creative: agencies, in-house, creators — by name
5. The talent that appears, or whether it is mashups, AI avatars or text-to-video
6. Asset lengths that actually get made
7. Landing page types
8. Whether the account already has a convention, and whether it is being followed

⛔ **Never invent a dropdown value.** The settings tab is what every future name is built from: a
producer or product name that does not exist becomes a category nobody can fill and a comparison that
never resolves.

⚠️ **Ask whether they will actually maintain it.** ACA names the alternative: *"if you're using a
tool like Motion... **you don't have to actually be using these naming conventions**, you can tag the
assets directly."* ⭐ A half-followed convention is worse than no convention, because it produces
comparisons that are silently wrong rather than obviously missing.

## How to run it

1. **Start from the comparisons**, and derive the dimensions each one needs
2. **Emit all three sheets** in ACA's structure — see `reference/the-generator.md`
3. ⛔ **Flag the six elements Course 601 teaches that ACA's sheet omits**, and say whether this
   account needs them. Three of the four questions above cannot be answered without them
4. ⛔ **Fix the code collisions**, and say you fixed them. ACA's file gives two dimensions the same
   code and uses three different code sets across its own tabs
5. **Name the delimiter and the separator explicitly**, and state what happens to spaces

## ⚠️ What this skill is not

**It is not a UTM or tracking-link builder.** ACA's second tab assembles a parameter string, and
verifying that a link resolves and reports correctly in analytics is a media-buying task the sheet's
own instructions hand back to the buyer.

**It does not tell you what to name a concept.** Concept IDs and hook identifiers come from the work;
this is the container for them.

**It does not decide what to test or track.** That is `aca-602-creative-testing`, and
`aca-track-creative-tests` for the log.

## Reference files

| File | Read it when |
|---|---|
| `reference/the-generator.md` | ⭐ All three sheets, every dimension and value, and the shape to emit |
| `reference/provenance.md` | ⚠️ **Read before reproducing a code.** The defects in ACA's shipped workbook, and what its ad-type library does not match |
