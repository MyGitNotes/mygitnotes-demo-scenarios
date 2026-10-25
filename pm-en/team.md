---
title: Team and who owns what
tags: [team, roles]
status: reference
---
# Team and who owns what

Six people run this release. The handle in the first column is the name used as @handle on a task, so the to-do tool can filter by person.

| Handle | Name | Role on this release | Looks after |
| --- | --- | --- | --- |
| @maren | Maren Holloway | Product manager, runs the release | Plan, weekly status, go/no-go, store text |
| @tomasz | Tomasz Hartl | Backend | Pickup codes, messages, reminders, rollout watch |
| @ines | Ines Calder | Mobile, iOS and Android | Counter screen, builds, store submission |
| @kofi | Kofi Tennant | QA | Test plan, regression, beta groups |
| @rhea | Rhea Santoro | Design | Counter screen, message text, help sheet |
| @leo | Leo Fenwick | Shop onboarding and support | Pilot shops, help sheet, calls on release day |

## Who owns what

A full RACI matrix is more paperwork than help for six people who sit in one room. Each area has exactly one accountable name, the person who answers for it at the go/no-go call. Everyone else is listed only when they must be asked or told.

| Area | Responsible | Accountable | Consulted | Informed |
| --- | --- | --- | --- | --- |
| [Pickup message and reminder](wp-notifications.md) | @tomasz | @maren | @rhea, @leo | @kofi |
| [Code check at the counter](wp-pickup-code.md) | @ines | @maren | @tomasz, @rhea | @leo |
| [Test plan](wp-qa.md) | @kofi | @maren | @ines, @tomasz | @leo |
| [Shop onboarding](wp-onboarding.md) | @leo | @maren | @rhea | everyone |
| [Store release and rollout](wp-store-release.md) | @ines | @maren | @tomasz, @kofi | @leo |

## How we decide

Decisions that change the plan use DACI: one **driver** who prepares the question, one **approver** who decides, **contributors** who are asked, and the people who are **informed**. The first one, [SMS first](decisions/sms-first.md), is written up that way. A decision that does not change the plan is made by whoever owns the task.

## Working agreements

- A task has one or two owners and never a team name. "Someone should check the limits" is not a task.
- A task has a due date. Without one it is an idea, and it stays in the notes until someone dates it.
- Mondays at 10:00 there is a fifteen-minute sync. On Fridays @maren writes the weekly status.
- Status colours: **green** means the next milestone is on track, **amber** means a risk has a name and a date, **red** means the next milestone will slip.

*This is a sample notebook from [MyGitNotes](https://mygitnotes.com/). [What this example shows](https://mygitnotes.com/use-cases/pm).*
