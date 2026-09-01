---
name: aca-803-creative-automation
description: Ad Creative Academy Course 803, Rory Flynn of Systematiq Ai - building an automated AI ad engine instead of prompting one image at a time. Covers the three core AI skills that make you tool-agnostic (deconstruction, system prompts, workflow development), the keep-this-change-that edit formula for in-context image models, the six parts of a system prompt with limits as the load-bearing one, node-based workflow building, batch processing so one input returns twenty outputs, and the reusable image generator whose only per-brand variable is a Visual Brand Profile. Use this when a team is prompting by hand and cannot keep up, when output is inconsistent between people, when the same creative job is being redone every week, or when someone wants to build a tool rather than make an asset. Reach for it whenever AI workflows, automation, batch generation or system prompts come up.
---

# Course 803: The Creative Automation Workshop

**Rory Flynn**, founder of Systematiq Ai, and the same faculty member who teaches Course 802. 1h 34m 13s,
6 modules.

> "We are going to go into a little bonus module on workflow building. Now that we've done a lot of things
> with the images and the videos ... **so we can actually start to build little micro tools**"

⭐ **This is the only course in the programme that builds a tool rather than an asset**, and the only one
that cites another course: it assumes Course 802 and explicitly extends it.

## What this skill needs from you

**Required:**

1. **The repeating job.** ⛔ **This course is for work that happens more than once.** A one-off image is
   faster by hand; the whole argument is *"there's no more single thoughts"*.
2. **The brand, and 10 or so of its images.** The Visual Brand Profile is built from them and it is the
   piece that makes a workflow reusable.
3. **What one run should produce** — 20 static variants, a prompt set, a video, an edited product shot.

**Useful:**

4. Who else will run it. ⭐ **Workflows are shareable and that is half their value**: *"It's something that
   can be shared between you or your team or a friend or whoever."*
5. Whether they already have prompts that work, which become the system prompt
6. Whether the assets ship as-is or get finished by a designer. ⚠️ **They are not finished goods** — see
   the scope note

⛔ **Never present a tool-specific workflow as the skill.** The course's own argument is the opposite:
*"it won't be about the tools, it'll be about what you can do with them."* The three core skills work
anywhere; the node editor is one implementation.

## Where to go

| They are asking | Go to |
|---|---|
| What do I actually need to learn? | `reference/three-core-skills.md` |
| How do I write a system prompt? | `reference/three-core-skills.md`, the six parts |
| How do I edit an image with a prompt? | `reference/three-core-skills.md`, keep-this-change-that |
| How do I build the workflow? | `reference/workflows-and-batch.md` |
| How do I get 20 outputs instead of 1? | `reference/workflows-and-batch.md`, batch |
| How do I point it at a different brand? | `aca-build-visual-brand-profile` |
| Where did these claims come from? | ⚠️ `reference/provenance.md` |

## The through-line

> "**We don't want single outputs anymore. We have to think in batch.** So like in this case it's how do
> I put this image in, write a prompt and **I get 20 outputs instead of one** and 20 different variations."

⭐ **That is the whole course in one sentence**, and it is a different claim from Course 702's volume
argument. 702 says produce more ads. This says **build the thing that produces them**, so volume stops
being a headcount problem.

## How to run it

⛔ **This is for work that repeats.** A one-off image is faster by hand, and the whole argument is that single
outputs are the thing to stop making.

1. **Confirm the job repeats.** If it does not, route to Course 802 and stop here.
2. **Teach the three core skills** from `reference/three-core-skills.md` — deconstruction, system prompts,
   workflow development. ⭐ Someone who learns only the node editor has learned nothing portable.
3. **Give the keep-this-change-that edit formula**, same file, with the keep clause stated explicitly. The
   model will not guess which part is the product.
4. **Write the system prompt** in its six parts, same file. ⛔ Limits is the load-bearing part: without it the
   model answers conversationally and breaks the next node. ⭐ **Its core-focus section is where the Visual
   Brand Profile goes**, so build that first if the output has to be on-brand —
   `aca-build-visual-brand-profile`, if installed. It is the one variable that repoints the whole workflow.
5. **Build the workflow** with `reference/workflows-and-batch.md`. ⛔ Everything must be connected — the most
   common silent failure is a workflow that runs and quietly ignores your product.
6. ⛔ **Test before batching.** Batching a broken system prompt costs twenty generations to discover.
7. **Batch it**: ask for ten prompts, separate them with a delimiter the content cannot contain, split, run.
8. ⭐ **Hide the system prompt in app mode.** It is the tool's logic, not its input.
9. ⭐ **Swap the profile to point it at another brand.** Nothing else in the workflow changes, and that is
   the test that a tool was built rather than one job done.
10. **Check the output is treated as raw.** These are assets to finish, not finished assets.

## Answering well

**Lead with the three core skills, not the tool.** Deconstruction, system prompts, workflow development.
*"These are three tools that are three skills that can be used anywhere in any time, in any medium. And
basically this will make you sort of tool agnostic."* ⭐ **Someone who learns only the node editor has
learned nothing portable**, which is the argument the course makes about itself.

**Deconstruction is Course 802's asset cloning, generalised.** Rory says so: *"think about the image
deconstruction model that we did"*. ⭐ **And he extends it past images** — *"that same process of
deconstruction can work for video. It'll work for sound, it'll work for music, it'll work for ... add
scripts or, you know, copy."*

**The edit formula is two words.** *"what is editing. Essentially it's if you break it down to its core
component components, **keep this change that**."* ⛔ **Then say what to keep explicitly**, because the
model will not guess which part is the product.

**In system prompts, limits do the work.** Six parts: actors, goal, output, core focus, format, limits.
⭐ *"limits probably the most important thing"* — and his worked example shows why: without *"do not
include any explanation, just provide the prompt"*, the model returns conversation that breaks the next
node in the chain.

⚠️ **Be honest about what comes out.** *"I would consider all of these **raw assets** that you're going to
have to sort of doctor up in your own way."* The workflow removes the repetition, not the craft.

## ⚠️ Scope

Building the machine. ⛔ **No metric, benchmark or performance claim appears anywhere in this course** —
what to test is Course 602, what the numbers mean is Courses 402 and 701, and what the ad should say is
Course 401. ⚠️ **It also does not decide creative volume**: Course 703's five variables and Course 601's
spend ladder do that.

⛔ **And it is the most tool-dependent course in the programme.** Every walkthrough runs inside one
third-party node editor. Carry the three core skills as the durable part and treat the tool as one
example, which is what the course itself asks for.

## Reference files

| File | Read it when |
|---|---|
| `reference/three-core-skills.md` | Deconstruction, the edit formula, and the six parts of a system prompt |
| `reference/workflows-and-batch.md` | Node basics, building the generator, app mode, and batch processing |
| `reference/provenance.md` | ⚠️ **Read before quoting any tool claim.** Includes the duplicated-source note and the conflict with Course 802 |
