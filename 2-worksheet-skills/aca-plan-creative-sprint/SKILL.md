---
name: aca-plan-creative-sprint
description: Fills Ad Creative Academy's Creative Sprint Planning board for a real sprint, in the workbook's own 28-column job record and its five-stage status flow from Planning through In Progress, Review, Complete and Launched. Every job carries its request type (MORE, FIX, ADAPT or NEW), concept, angle, product, format, variant count, aspect ratios, launch date and channel, and the board's supporting tabs cover per-brand goals, products, an angle library with per-angle performance, a promo calendar and weekly delivery. Use this when a creative team needs a shared pipeline, when jobs keep getting lost between brief and launch, when planning a week or a quarter of creative, or when someone asks for a sprint tracker. Requires the jobs - it cannot plan a sprint it has not been told about.
---

# Fill the Creative Sprint Planning board

Produces **Ad Creative Academy's Course 703 artifact** — Chloe Rhys's planning board, the one her
team runs at OpenStore.

⭐ **The board is a pipeline, not a list.** A job has one row and moves through five status sheets;
the row is the same 28 columns at every stage.

## ⛔ Read this before producing anything

**The workbook ACA ships is a working board, not a blank template.** It contains real third-party
data: client brand names in its promo calendar, live Facebook Ads Manager links carrying real
account, business and campaign IDs, and staff names on real job records.

⛔ **Never reproduce any of it.** Emit the **structure** — sheet names, column headers, status values,
request types — and fill it only with what the user gave you. **No brand from ACA's calendar, no
person, no ads-manager URL, ever**, including as an example.

⚠️ **Use placeholders when you need to show the shape**: `[BRAND]`, `[REQUESTER]`, `[CREATOR]`,
`[LINK]`.

## What this skill needs from you

**Required:**

1. **The jobs** for this sprint — what is being made, and why
2. **The request type of each** — MORE, FIX, ADAPT or NEW. ⛔ If they were not typed, the mix cannot
   be checked, and the mix is the point of a sprint

**Optional, and each one fills real columns:**

3. Brand, product and angle for each job
4. Format, and how many variants each concept needs
5. Which aspect ratios are required
6. Requester and creator, if the board is shared
7. Due dates, and whether a job is business-as-usual or time-sensitive
8. Base job, for MOREs and FIXes — what this one iterates on
9. Reference links and creative direction

⛔ **Never invent a job, a date, a launch channel or a variant count.** This board is a team's shared
source of truth: a row somebody did not ask for becomes work somebody is expected to deliver.

⛔ **Never fill a Creative Link or a Launch Date that has not happened.** Those two columns are how
the board distinguishes planned from live, and a speculative entry makes a sprint look shipped.

## How to run it

1. **One row per job**, in the earliest status that honestly applies
2. ⭐ **Check the mix before delivering** — the four request types against ACA's target shares. A
   sprint that is all NEW has no pipeline behind it; a sprint that is all MORE is not learning
   anything
3. **Group by status**, since that is how the board is read at a standup
4. **Leave unknowns blank rather than guessed**, and list them

## ⚠️ What this skill is not

**It does not decide how many jobs a sprint should hold.** The five variables that set volume are
`aca-703-sprint-planning`, and Course 601's competing ladder is in `aca-plan-creative-volume`.

**It is not the test log.** A creative test's hypothesis, result and learning belong in
`aca-track-creative-tests`. This board tracks *production*; that one tracks *evidence*.

**It does not automate anything.** ACA's *Sprint Planning Operation System Worksheet* documents the
engineering stack OpenStore built around this board — Apps Script, n8n, Slack, a dashboard. It is
not a fillable worksheet, and it is carried inside `aca-703-sprint-planning`.

## Reference files

| File | Read it when |
|---|---|
| `reference/the-board.md` | ⭐ All 28 columns, the five status sheets, the supporting tabs, and the shape to emit |
| `reference/provenance.md` | ⚠️ **Read before reproducing anything from ACA's file.** What was redacted and why, and the defects in the shipped workbook |
