---
title: Welcome to the release notebook
tags: [guide]
status: reference
---
# Cubbyshelf v1.1: the release notebook

This notebook is how a six-person team runs one release of a small product: who owns what, which dates matter, and what is at risk this week. The product is Cubbyshelf, the parcel-holding app described in the [Product spec notebook](../project-en/index.md). Version 1.1 adds the pickup message and the code check at the counter. The team, the shops and the numbers are all invented.

**Where we are:** Sunday 25 October 2026, eighteen days before release day (Thursday 12 November). The latest status note is [Friday 23 October](status/2026-10-23.md): amber, because the SMS sender name is still waiting for approval.

The dates in these notes are real calendar dates, and the to-do tool compares them with today's date. When you open a later copy of this demo, more open tasks will show as overdue than the status notes say. The weekly status notes are the record of how the plan stood on the day.

## What to try

1. **Filter the to-do tool by person.** Open the to-do tool in the right rail, set **People** to `tomasz`, then to `leo`. Each person's tasks come with their priority and dates.
2. **Sort by priority.** Set **Sort** to *Priority*. The 🔺 tasks come first, starting with registering the SMS sender name, which is also overdue.
3. **Open the Gantt.** Switch the to-do tool to its Gantt view. Each task is a bar from its start date to its due date, tinted by priority, and the five milestones are diamonds labelled with the note's title. Click a diamond to open that note.
4. **Look at the calendar.** Open the calendar and go to October and November 2026. The milestones show as diamonds on their days, and the day detail lists them under *Milestones* above the notes and tasks.
5. **Switch to the Kanban view.** The work packages and milestones are cards in five columns by status: *reference*, *planned*, *in progress*, *blocked* and *done*. Drag a card to change its status.
6. **Open the Friday review.** In the Focus menu, choose **Friday review**: the [release plan](release-plan.md), the latest status and the [risk register](risks.md) side by side, the way the team reads them before the Monday sync.
7. **Read the plan as figures.** The [release plan](release-plan.md) opens with key numbers and a `timeline` by calendar week, the [risk register](risks.md) ranks every open risk in a `bars` chart, each weekly status carries a `status-board`, the [test plan](wp-qa.md) splits its cases in a `parts` bar, and [SMS first](decisions/sms-first.md) draws the decision as an `argument-map`.
8. **Tick a task.** The note keeps the finish date next to the task. This is a demo copy: your changes stay in your browser for 24 hours and never reach anyone else.

## Notes in this notebook

| What | Note |
| --- | --- |
| People and decisions | [Team and who owns what](team.md), [SMS first](decisions/sms-first.md) |
| The plan | [Release plan](release-plan.md), [Risk register](risks.md) |
| Work packages | [Pickup message and reminder](wp-notifications.md), [Code check at the counter](wp-pickup-code.md), [Test plan](wp-qa.md), [Shop onboarding](wp-onboarding.md), [Store release and rollout](wp-store-release.md) |
| Milestones | [Scope freeze](milestones/m1-scope-freeze.md), [Feature complete](milestones/m2-feature-complete.md), [Release candidate](milestones/m3-release-candidate.md), [Go/no-go](milestones/m4-go-no-go.md), [Release day](milestones/m5-release.md) |
| Meetings | [v1.0 retro](meetings/2026-10-02-v1-retro.md), [Kickoff](meetings/2026-10-05-kickoff.md), [Monday sync, 19 October](meetings/2026-10-19-sync.md) |
| Weekly status | [9 October](status/2026-10-09.md), [16 October](status/2026-10-16.md), [23 October](status/2026-10-23.md) |

*This is a sample notebook from [MyGitNotes](https://mygitnotes.com/). [What this example shows](https://mygitnotes.com/use-cases/pm).*
