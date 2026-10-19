---
title: Risk register
tags: [plan, risks]
status: in progress
---
# Risk register

Updated Friday 23 October. Each risk has one owner, a trigger that tells us it is happening, and a next step. Likelihood (L) and impact (I) are rated 1 (low) to 3 (high), and exposure is the product of the two. A risk of 6 or more is read out at every Monday sync, and the go/no-go call reads all of them.

| ID | Risk | L | I | Exposure | Owner | Trigger | What we do |
| --- | --- | --- | --- | --- | --- | --- | --- |
| R1 | The SMS sender name is not approved in time for feature complete | 3 | 3 | 9 | @tomasz | No approval by Wednesday 28 October | Chase the provider every other day. On 28 October @maren decides whether the beta uses the provider's shared sender. **This one is happening.** |
| R2 | App Store review rejects the build or takes longer than planned | 2 | 3 | 6 | @ines | Still in review 48 hours after submission | Submit three working days before the go/no-go call, answer the same day, keep expedited review for a blocker |
| R3 | Two neighbours share a name and a parcel is handed over to the wrong one | 2 | 3 | 6 | @maren | A pilot shop uses the name fallback more than once a day | The code is always asked first, and the name fallback makes the shopkeeper confirm the neighbour before the parcel is marked collected |
| R4 | Only one backend engineer, so an absence stops the message work | 2 | 3 | 6 | @maren | @tomasz is out for two days or more before the release candidate | @ines reviews every backend change and can run the reminder job locally |
| R5 | An SMS costs more than the shops will accept | 2 | 2 | 4 | @maren | The pilot shops' SMS bill is more than they said they would accept, see [SMS first](decisions/sms-first.md) | Reminders are capped at one per parcel; read the bill after two weeks |
| R6 | Shopkeepers do not read the help sheet and are surprised at the counter | 2 | 2 | 4 | @leo | A pilot shop phones with a question the sheet answers | Phone calls the day before, the sheet inside the app as well as on paper |

:::bars{title="Exposure of each open risk" unit="points" max="9"}
- **R1 sender name**｜9｜Happening
- R2 store review｜6
- R3 same-name handover｜6
- R4 one backend engineer｜6
- R5 message cost｜4
- R6 help sheet unread｜4
:::

## Closed

- **R0, store review took three days for v1.0.** Closed on 5 October by the three-working-day buffer in the [release plan](release-plan.md), an action from the [v1.0 retro](meetings/2026-10-02-v1-retro.md).
