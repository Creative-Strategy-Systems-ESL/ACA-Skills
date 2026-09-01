# Automating the sprint system

⚠️ **What this section is, and what it is not.** ACA ships an asset for this course called the
*Sprint Planning Operation System Worksheet*. **It is not a worksheet and there is nothing to fill
in.** It is engineering documentation for the internal creative-operations stack OpenStore built
around the sprint board, credited to **Billy Bjork** alongside Chloe.

⭐ **It is still worth having**, because it is the only place in the programme that shows what the
sprint board looks like once a team has outgrown doing it by hand.

## The problem it was built for

> "Our challenge was to scale creative operations to deliver **150+ unique ad creatives per week
> across 40+ brands.**"

⭐ **That number is the context for everything in Course 703.** The five volume variables, the
cruising-speed argument and the four request types all come from a team operating at that scale. A
brand running one account does not need any of this machinery — but the concepts underneath it still
apply.

## The three components

| Component | What it does |
|---|---|
| **Creative Sprint Planning** | *"Central project management system that tracks projects through all stages, implements naming conventions, and facilitates collaboration between strategists, editors and designers"* |
| **Automated Notifications** | Slack notifications triggered by status changes, ⭐ *"allowing users to update project statuses directly from Slack messages"* |
| **Performance Dashboard** | Browsing every ad in the portfolio launched on Meta and TikTok. Users take their own copy, then filter and sort by metrics like spend, CTR and ROAS |

**The stack named:** Google Sheets Apps Script with external API integrations including **iconik** for
media asset management · **n8n** for node-based workflow orchestration · a data pipeline doing
**daily metric refreshes from Meta and TikTok**.

## The six workflow steps

| Step | What happens |
|---|---|
| **1. Job creation** | Jobs are added with **dynamically generated names** from user input. On a status change, a script **auto-increments a brand-specific counter** to assign the job number. Supports batch creation |
| **2. Review link generation** | After the first revision, assets are exported to the media asset manager and **review links are generated automatically by looking up the job name** |
| **3. Trigger Slack notifications** | Status changes send payloads onward, which route to the right Slack message |
| **4. Interactive Slack messages** | When notes are left on a first creative, editors and designers get a notification **they can change the job status from** |
| **5. Processing Slack interactions** | Those interactions route back and update the sheet |
| **6. Performance analytics** | The dashboard, filtered |

⭐ **Steps 1 and 2 are the ones worth copying even without the engineering.** Auto-generated job names
and auto-assigned numbers are what make the naming convention hold — Course 601's whole argument is
that a convention only works if it is followed every time, and a system that generates the name
removes the chance to get it wrong.

⭐ **Steps 3 to 5 solve the real operational problem**, which is that status only stays current if
updating it is easier than not updating it. A board nobody updates is worse than no board, because it
reports confidently and wrongly.

## The dashboard's filters

**And this is the payoff, because it shows what the board's columns are actually for:**

| Filter |
|---|
| Brand |
| Channel — Meta or TikTok |
| Requester (strategist) |
| Creator (editor/designer) |
| Job Format — video or static |
| ⭐ **Job Type — New, More, Fix, Adapt** |
| Date range (launch date) |
| ⭐ **Wins and Pre-Wins** — internal top-performer criteria |

⭐ **Every filter is a column on the sprint board.** That is the argument for filling the board
properly: each field you leave blank is a question you cannot ask later. Filtering performance by
**Job Type** is what tells you whether your MOREs actually out-hit your NEWs, which is the number
that should set next quarter's mix.

⚠️ **"Pre-Wins" appears only here.** Course 703 defines a win with four criteria and never mentions a
pre-win, so its threshold is not held. Treat it as OpenStore's internal tier, not a taught concept.

## ⛔ What to take from this if you are not building it

**You do not need Apps Script, n8n or Snowflake.** The transferable rules:

1. **Generate job names and numbers rather than typing them**, however you do it
2. **Make the status update happen where the person already is**, not in a sheet they have to open
3. ⛔ **Record job type on every job**, because it is the filter that makes the sprint mix
   answerable rather than aspirational
4. **Define your win criteria once and store them as a flag**, so "which of these won" is a query
   rather than an argument

⚠️ **The documentation names a public repository and an individual's contact details.** They are not
reproduced here; the architecture above is what matters and it is described in full.
