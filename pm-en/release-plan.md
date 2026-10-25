---
title: Release plan, Cubbyshelf v1.1
tags: [plan, release]
status: in progress
---
# Release plan, Cubbyshelf v1.1

**Goal:** a neighbour hears that a parcel has arrived, within a minute, with a code, and the shopkeeper hands it over by checking that code. Version 1.0 shipped on Thursday 24 September with check-in, a waiting list and marking a parcel collected, but no message and no code check. Version 1.1 closes the loop.

:::key-numbers{title="The release at a glance"}
- **12 Nov**｜Release day｜Thursday. The staged rollout starts the same day
- 5｜Milestones｜Scope freeze, feature complete, release candidate, go/no-go, release
- 3 days｜Store review buffer｜Added after the [v1.0 retro](meetings/2026-10-02-v1-retro.md)
- 6｜People｜One accountable name per area, see [the team](team.md)
:::

## Scope

What is in v1.1, with the spec note each item comes from:

| In v1.1 | Spec | Owner |
| --- | --- | --- |
| The pickup message with a six-digit code, by SMS | [Notifications](../project-en/spec-notifications.md) | @tomasz |
| A reminder after three days, with an off switch for reminders | [Notifications](../project-en/spec-notifications.md) | @tomasz |
| Code check at the counter: a code works once | [Pickup flow](../project-en/spec-pickup-flow.md) | @ines |

What is not, and stays on the backlog until v1.2: [barcode scanning](../project-en/spec-barcode-scan.md) and [returns](../project-en/spec-returns.md). Both were asked for. Neither is needed for the message and the code to work, and each would add a week of testing.

## Milestones

The dates are fixed backwards from release day. Each milestone has its own note with exit criteria, and shows on the calendar and on the Gantt view of the to-do tool.

::::timeline{title="The plan by calendar week" from="41" to="47" ticks="41,42,43,44,45,46,47"}
:::lane{title="Plan"}
- 41｜Kickoff, 5 Oct
- **42**｜[Scope freeze](milestones/m1-scope-freeze.md), 16 Oct
:::
:::lane{title="Build"}
- 42–44｜Message, reminder, code check
- **44**｜[Feature complete](milestones/m2-feature-complete.md), 30 Oct
:::
:::lane{title="Test"}
- 44–46｜Beta, regression, pilot shops
- **45**｜[Release candidate](milestones/m3-release-candidate.md), 6 Nov
:::
:::lane{title="Ship" highlight}
- **46**｜[Go/no-go](milestones/m4-go-no-go.md), 10 Nov, and [release](milestones/m5-release.md), 12 Nov
- 46–47｜Staged rollout
:::
::::

## Go or no-go

On Tuesday 10 November @maren asks each owner one question. The answer is go only if all of these hold on the release candidate:

| Check | Who answers |
| --- | --- |
| No open bug that blocks check-in, the message or the code check | @kofi |
| The full regression passes on the exact build that was submitted | @kofi |
| Both builds are approved and waiting to be published (iOS set to manual release, Android under managed publishing) | @ines |
| The SMS sender name is approved, and a message to a real phone arrives in under a minute | @tomasz |
| The three pilot shops have done the counter flow once without help | @leo |
| The [risk register](risks.md) has no open risk rated red | @maren |

## Rollout and rollback

The release goes out in steps, so a problem reaches few shops before it is noticed: 10% of shops on Thursday 12 November, 50% on Friday, 100% on Monday 16 November, each step only after 24 hours without a trigger. On iOS the release is manual and uses phased release, which Apple runs on a fixed seven-day schedule, so it cannot follow the Android steps; if a trigger fires, @ines pauses the phased release, and once Android has reached 100% without a trigger she chooses release to all.

A rollback is called by @maren, on advice from @tomasz, if any trigger fires:

- the messages sent per check-in fall below 90% for an hour;
- the app crashes for more than 2% of sessions;
- a shopkeeper cannot hand over a parcel with a valid code.

Rolling back the app does not roll back the database. Version 1.1 adds columns and never removes one, so the old app keeps working against the new schema, and a fix goes forward as 1.1.1 once the cause is known.

*This is a sample notebook from [MyGitNotes](https://mygitnotes.com/). [What this example shows](https://mygitnotes.com/use-cases/pm).*
