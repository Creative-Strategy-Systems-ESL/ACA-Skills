---
name: aca-audit-ad-account
description: Audits an ad account's creative performance and produces Ad Creative Academy's Course 302 artifacts - the Quick Performance Analysis Worksheet for a fast health check, or the In-Depth Creative Audit Worksheet for a full teardown. Finds the unicorn ad and dissects it into its success formula, reads hook rate and hold rate, compares 7-day against 30-day to separate creative fatigue from scaling problems, breaks performance down by format, element and audience, then turns it into creative principles, a testing plan and a refresh roadmap. Use this when someone takes over an account, asks what is working and why, wants to know why performance dropped, needs to decide what to make next, or has exported ad data and does not know what to do with it. Requires actual performance data - it cannot audit an account it has not seen numbers from.
---

# Audit an ad account's creative

**Ad Creative Academy**, Course 302 (Mirella Crespi), module 1. Two worksheets and twelve AI prompts.

> "Great creative strategy is not built on guesswork. It's built on insights."

## What this skill needs from you

⛔ **Required, and there is no way around it: exported performance data.**

Mirella is explicit that the prompts *"aren't replacements for accessing your ad data — you'll still
need to pull those reports."*

⛔ **If no data is supplied, do not produce an audit.** Say what to export instead. An audit of an
account nobody has looked at is a plausible-sounding document with no facts in it, and it is worse
than nothing because it reads like work.

**The minimum export**, and the smallest useful version of each:

| For | Pull |
|---|---|
| The unicorn | All-time creative report: spend, ROAS or CPA, launch date, days active |
| Section 2 | Last 30 days, top 5 to 10 creatives by primary KPI, with format |
| Section 3 | The same for the last 7 days |
| Sections 4 and 5 | 3-second video views, ThruPlays and impressions per creative |
| Section 6 | Last 6 months, top performers by month or quarter |

**Also required:**

1. **Which audit.** Quick (a monthly health check) or In-Depth (taking over an account)
2. **The primary KPI** the account is judged on

**Optional, and it sharpens the audit:**

3. A description of each creative, or the creatives themselves. Without this the audit can rank
   numbers but cannot say *why*, which is the entire point
4. Breakdowns by age, gender, geography, or by prospecting versus retargeting
5. Production cost per creative, for the cost-effectiveness section

⚠️ **Creative descriptions are the input people forget and the one that decides whether this is an
audit or a spreadsheet summary.** If only numbers arrive, say what the audit can and cannot conclude
without them.

## Which audit to run

| | **Quick Performance Analysis** | **In-Depth Creative Audit** |
|---|---|---|
| When | Monthly or quarterly health check | Taking on a new account |
| Sections | 9 | 9 parts |
| Answers | What should we make next? | What actually drives performance here? |

Both live in `reference/the-worksheets.md`.

## ⛔ The metric warning that governs everything else

**The course names no thresholds.** There is no "a good hook rate is X" anywhere in it. Part 1 of the
in-depth worksheet asks you to record your *own* current average, top and bottom performer, and set
targets from those.

⛔ **Do not supply an industry benchmark for hook rate, hold rate or anything else and attribute it
to this course.** If someone needs one, say the course deliberately does not give one and that the
account's own baseline is the benchmark it uses.

⚠️ **ACA does give numbers, but in a different course.** `aca-402-key-metrics` (Chloe Rhys) carries
thumbstop and CTR bands **with the advertiser they came from attached** — one brand, men's apparel,
on Meta. If someone insists on a reference point, that is the honest one to offer: name it as
Chloe's, say which brand, and say the account's own baseline still outranks it. What stays banned is
inventing a figure, or attributing any figure to this course.

## How to run it

1. **Confirm the North Star metric first.** Part 1 of the in-depth worksheet, and it comes first for
   a reason: an audit measured against the wrong metric produces confident, wrong conclusions and
   every later section inherits them. *"There is no point in looking at ROAS or CPA if there is
   another metric like contribution margin that you should be paying attention to."*
2. **Find and dissect the unicorn.** `reference/the-worksheets.md`, section 1.
3. **Work the sections in order.** Each compares back to the unicorn.
4. **Use the prompts to accelerate the analysis, not to replace the data.**
   `reference/the-prompts.md`.
5. **End on the three action outputs**: creative principles, a testing plan with hypotheses, and an
   optimization roadmap.

## ⚠️ The unicorn is a warning as well as a prize

The worksheet frames section 1 as finding your best ad. The delivered course adds the half the
worksheet leaves out:

> "We don't really want that. You don't want to have that single creative that consistently
> outperforms everything else in the ad account. **Our goal is to strive for some balance.**"

**So report the unicorn twice:** as the success formula to mine, and as a concentration risk. An
account resting on one creative is one fatigue cycle from a cliff.

⭐ **The question that decides which reading dominates** is the worksheet's own *"fatigue rate
comparison (unicorn vs. recent ads)"* and *"potential new success factors identified"*. If nothing
is approaching the unicorn, the risk reading is the headline.

## Answering well

**Break down by element, not by ad.** *"Analyze your creative performance by specific elements rather
than just looking at top-line results."* "Ad 47 did well" is not a finding. "Ads opening on the
problem scenario beat ads opening on the product" is.

**Say which window a conclusion came from.** The whole point of comparing 7 days, 30 days and 6
months is separating *"enduring creative principles versus temporary trends"*. A finding from one
window is a guess.

**Every test needs a hypothesis.** The worksheet asks for *"clear hypotheses for each test based on
audit findings"*. A test list without hypotheses is a production schedule.

⚠️ **This is not a paid-media audit.** *"These are not ad account audits from the paid media
perspective."* Bidding, budget structure, campaign architecture and account hygiene are out of scope.
If the data shows a media problem, say so plainly and say it is outside what this audit covers.

## Reference files

| File | Read it when |
|---|---|
| `reference/the-worksheets.md` | Both worksheets, section by section, with what goes in each field |
| `reference/the-prompts.md` | The twelve AI prompts, what each is for, and what to check in their output |
| `reference/provenance.md` | ⚠️ **Read before quoting any figure or threshold.** Source, what dates, and what is ACA's versus this skill's |
