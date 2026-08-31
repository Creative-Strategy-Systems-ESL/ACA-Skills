# Auditing an account you did not build

**⚠️ This file is this skill's assembly, not a module of the course.** Every check in it comes from
Ashley's material — the objectives table, the targeting argument, the creative best practices, the
seven watchouts, the measurement section — put into the order a diagnosis actually needs. ACA does
not ship it as a sequence.

It exists because "I've inherited this account and it's a mess" is the most common way this course
gets used, and because working the modules in teaching order is the wrong order for triage.

## ⛔ The triage order, and why it is this way

> **Objective → measurement → targeting → creative.**

Work it in that order and stop at the first thing that is broken, because everything downstream
inherits it. The usual instinct is to reach for creative first, which is the most expensive possible
place to start and often fixes nothing.

- **A wrong objective cannot be fixed by better creative.** Meta will keep pursuing the goal it was
  given. This is the single most consequential setting in the account.
- **Broken measurement means you cannot tell whether anything you change worked.** Fixing it costs
  nothing and is worth doing before spending on assets.
- **Narrow targeting raises costs in an auction and excludes buyers**, and it is a settings change,
  not a production job.
- **Creative is the biggest lever** — but only once the three above are not lying to you.

---

## 1. Objective

- [ ] **What objective is it running?** Get this before anything else.
- [ ] **Does it match the business outcome the client actually wants?** If they want sales and the
      objective is Traffic or Engagement, stop here — this is the finding.
- [ ] **Traffic running on an ecommerce account?** ⚠️ Expect exactly the symptom pattern of cheap
      clicks and no revenue. *"Clicks do not equal sales."*
- [ ] **Engagement being used as a performance objective?** *"We were never able to prove that
      there's any correlation between getting a high engagement and actual business outcomes."*
- [ ] **Leads or App promotion running alone?** Both should be paired with an awareness campaign.
- [ ] **Sales objective without the prerequisites?** Pixel, CAPI, catalog where relevant, and a
      full-funnel campaign alongside. See `the-system.md`.

⭐ **The pattern worth recognising instantly:** a good CPC with no sales is not a half-working
campaign. It is the system doing precisely what it was told, and the cost efficiency is a score in
the wrong game.

## 2. Measurement

- [ ] **Is the pixel installed, and is it actually firing on purchase?** Not "is it in the account"
      — is the event landing. On an inherited account, assume nothing.
- [ ] **Is the Conversions API set up?**
- [ ] **Is there any conversion history, and what shape is it?** Steady, or one spike?
- [ ] **Which attribution model is the reporting using?** If last click, read the tequila analogy in
      `testing-and-measurement.md` before quoting the number to anyone.
- [ ] **Does any other system claim the same conversions?** Email, affiliate, an ecommerce
      dashboard. ⚠️ **If two platforms each claim credit for the same orders, both numbers are
      inflated** — reconcile against the backend order count before presenting either.
- [ ] **Is there a test running at all? A holdout?** If not, nobody in the account currently knows
      what is working, including whoever is telling you what is wrong.

⚠️ **The course gives no minimum conversion volume for the Sales objective**, no learning-phase
threshold, and nothing on attribution windows. Those are real gaps. Do not invent numbers for them
— check Meta's own current documentation.

## 3. Targeting

- [ ] **How narrow is it?** Interest stacks and tight age bands are the common inherited problem.
- [ ] **Would broadening be affordable?** The rule is *"as broadly as your budget and logic will
      allow"*, and Advantage Plus audience where budget permits.
- [ ] **Is any narrowing genuinely product-linked**, or is it a proxy someone assumed? A cut that
      the product itself demands is reasonable; a demographic guess usually is not.
- [ ] **How many placements?** Meta's own recommendation as of the recording is at least six. More
      placements do not raise costs and usually lower them.
- [ ] **Is auto-placement doing the resizing?** Preview every placement before trusting it.

## 4. Creative

- [ ] **How many genuinely distinct ideas are running** — as opposed to how many ad IDs exist?
      ⭐ Three colourways of one video is **one** creative input. See `andromeda-update.md`.
- [ ] **Do the ads carry different jobs?** Demo, objection handling, proof, offer, lifestyle.
- [ ] **Does the creative match the objective?** Watchout 6, and the one that lands on the
      strategist.
- [ ] **Brand and message in the first two seconds?**
- [ ] **Subtitles, and readable on a phone?**
- [ ] **Does each ad stand alone**, without assuming the viewer saw the others?
- [ ] **Anything cropped by the safety zones?**
- [ ] **Music rights? Category rules?**
- [ ] **How long has it been running?** Fatigue is normal by week four to eight and is not evidence
      the creative was bad.

## 5. What to say when someone blames the creative

Frequently the agency or the previous owner will assert the creative is the problem. It may be. But:

- **A creative diagnosis made without measurement is an assertion**, not a finding.
- **New creative built on the wrong objective inherits the wrong objective.**
- **"More variations" is not the same ask as "more distinct concepts"** — see `andromeda-update.md`,
  and re-scope the quote before agreeing to it.

⭐ **If they insist the creative is fine and the client agrees, use Ashley's demo**: record your own
feed, splice the ad in, watch the room change. *"The contrast is often stark and well, a bit
depressing."*

---

## ⚠️ What this course cannot tell you about an inherited account

Name these as gaps rather than guessing, because a confident wrong answer here costs real money:

| Not covered | Where it belongs |
|---|---|
| Account structure — campaign vs ad set counts, budget allocation strategy, when to consolidate | Meta's own documentation |
| Minimum conversion volume before the Sales objective is viable | Meta's documentation |
| Attribution windows | Meta's documentation |
| Benchmarks by vertical — what a good CPC, CPM or ROAS is for *your* category | Nowhere in this course. Any number you have seen quoted is not from here |
| **Regulated categories** — health, supplements, finance, alcohol, gambling | ⚠️ The course says to know Meta's ad rules and gives social issues and teen targeting as its only examples. If the brand makes health or efficacy claims, get the current policy checked before commissioning anything. A rejected ad set is a worse outcome than a badly targeted one |
