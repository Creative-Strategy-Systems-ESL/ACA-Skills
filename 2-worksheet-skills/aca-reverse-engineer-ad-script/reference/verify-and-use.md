# Verifying the brand brief, and checking the rewrite

⚠️ **Read this before running step 2.** Everything in this file is this skill's addition. ACA does
not warn about any of it.

## The problem in one paragraph

Step 2 says *"Using your knowledge of TARGET BRAND, build a brand brief"* and asks for seven things:
positioning, core values, tone of voice, target customer, visual and lifestyle world, key products,
and what makes them different. **A model will produce all seven for any brand name it is given**,
including one it has never encountered, one that changed direction last year, and one that does not
exist. The output will be fluent, specific and internally consistent. Then every line of the final
script is derived from it.

⛔ **The script is downstream of the brief, so a wrong brief does not produce an obviously wrong
script. It produces a good script for a brand that isn't the client.** That is much harder to catch
in review, because the failure is invisible in the artifact where the work is judged.

## How reliable each of the seven outputs is

Not equally, and the differences are predictable:

| Output | Reliability | Why |
|---|---|---|
| **Key products or collections** | ⚠️ Lowest | Product lines change constantly. Names, collections and hero SKUs go stale faster than anything else here |
| **Visual and lifestyle world** | ⚠️ Low | Highly inferable from category, which is exactly what makes a confabulation read as plausible |
| **Core values / what they avoid** | ⚠️ Low | Often reconstructed from what a brand of this type *would* say |
| **Tone of voice** | ⚠️ Medium | Usually directionally right for well-known brands, unreliable for small ones |
| **Target customer** | ⚠️ Medium | An inference from the category and price point. Reasonable as a hypothesis |
| **Brand positioning** | ✅ Higher | The most-written-about fact about any brand, so best represented |
| **What a competitor would never say** | 🔍 The tell | See below |

⭐ **Question 7 is the diagnostic.** *"What would a competitor never say that this brand would?"* A
researched brief answers it with something that would be actively wrong from the brand next door. A
fabricated brief answers it with something any brand in the category could claim: "quality
craftsmanship", "we care about our customers", "sustainability". **If the answer fits three
competitors, the brief is generic and the rewrite will be too.**

## What to do

### If the tool can browse

**Then do.** The prompt's own ROLE line says the writer *"know how to do independent research"*,
which contradicts step 2's *"using your knowledge"*. Resolve it in favour of research.

Check, in this order, because it is cheapest to most expensive:

1. **The brand's own site** — how they describe themselves, current collections, the language on
   product pages
2. **Their recent ads**, in a public ad library — tone in the medium the rewrite is for, which is not
   the same as tone on the website
3. **Their social** — the voice they use when not selling

Then rewrite the brief from what you found and mark anything you could not confirm.

### If the tool cannot browse, or the brand is genuinely unknown

⛔ **Do not silently produce the brief anyway.** Two honest routes:

**Route A, preferred: ask for the brief.** The person requesting the rewrite usually works on the
brand and can answer all seven in five minutes, better than any research could. **Ask for questions 1,
2, 3 and 7** and infer the rest. That is a far better use of a round trip than a fabricated brief.

**Route B: produce it as a hypothesis, labelled.** If the request is one-shot and has a deadline,
write the brief, mark it clearly, and say what would change if it is wrong:

> ⚠️ **BRAND BRIEF UNVERIFIED.** Built from general knowledge of [BRAND], not from their current site
> or ads. The positioning and customer profile are the load-bearing assumptions; if either is wrong,
> the script's tone and its central claim both change. Check these before production.

**Ask and deliver, rather than ask and wait** — unless the person is clearly still in conversation
with you.

### Marking it inside the document

⛔ **Put the flag in the brief itself, not only in your covering message.** A script gets pasted into
a deck, forwarded, and produced by someone who never saw the conversation. Mark each unverified item
where it sits:

```
Core values: Slow production, material honesty, repair over replacement
              ⚠️ UNVERIFIED — inferred from category, not confirmed on their site
```

That is the only place the caveat still exists when the script reaches the person spending money on
it.

---

## Checking the rewrite

Five checks, in the order they are worth running.

**1. Source-noun sweep.** Search the finished script for every proper noun, place and product from
the source transcript. There should be zero hits. This catches the most common failure, which is a
beat that carried the source's content through step 1.

**2. The lift test.** Put the source and the rewrite side by side, beat for beat. If any line is the
source's sentence with the nouns swapped, it is a lift, not a rewrite. Rewrite that beat from the
*structure* rather than from the source's line.

**3. The question-7 test on the output.** Would this script be wrong coming from the target's nearest
competitor? If it would work equally well for either, the brand brief did not do its job and the
script is category wallpaper.

**4. Length.** ACA asks for approximate parity with the source. Check it, because the original's
length was set by a media slot and drifting 40% longer means it no longer fits what it was modelled
on.

**5. The closing note.** It must name **structural** elements. If the note says "I kept the warm,
authentic feel", that is tone, not structure, and it suggests the deconstruction in step 1 was thin.
A good note reads like *"preserved the five-beat problem-to-proof arc and the cold open on an
unresolved question; translated the factory-access beat into a studio-access beat."*

## When this is the wrong tool

**The source has no script.** A montage with music and three words of supers has no narrative arc to
extract. There is nothing here to reverse-engineer.

**You want several concepts rather than one adaptation.** This produces one script from one source.
For angle variety across an offer, that is a different job.

**The source is not actually working.** The whole method assumes the source ad earned its structure.
Nothing here validates that assumption, so an admired-but-unproven ad transfers its structure just as
willingly as a winner does.

⚠️ **The course's own selection rule is admiration, not performance** — *"pick three ads you
genuinely think are great"*. That is fine for training the eye and weaker as a basis for spending
production money. If run length or performance data is available for the source, use it.
