---
title: "Decision: SMS first"
tags: [decision]
status: done
---
# Decision: SMS first

**Decided Wednesday 14 October 2026.** Driver: @tomasz, who compared the options. Approver: @maren. Contributors: @rhea and @leo, who asked the shops. Informed: @kofi and @ines.

**The question.** How does a neighbour hear that a parcel has arrived? The [spec](../../project-en/spec-notifications.md) needs the message within a minute of check-in and says nothing about the channel.

**The decision.** The first message goes out by SMS in v1.1. Reminders are one per parcel, after three days. Push notifications are a later addition for neighbours who install the app.

::::argument-map{title="How does a neighbour hear that a parcel has arrived?" source="Weekly sync, 12 October, and the decision of 14 October"}
- [C] The first message goes out by SMS in v1.1

:::reason{to="C" id="R1" status="accepted"}
- [P1] Every neighbour has a phone number the shopkeeper can type at check-in
- _No app, account or follow is needed_
:::

:::reason{to="C" id="R2" status="accepted"}
- [P2] An SMS reaches a locked phone within a minute, as the spec requires
:::

:::objection{to="C" id="O1" status="accepted"}
- [P3] Each SMS costs money, and the shops pay for the volume
:::

:::objection{to="O1" id="O2" status="accepted"}
- [P4] The cost is a message and a single reminder per parcel, and the bill is read after two weeks
:::

:::objection{to="C" id="O3" status="rejected"}
- [P5] Push notifications cost nothing per message
:::

:::objection{to="O3" id="O4" status="accepted"}
- [P6] A push needs the neighbour to have installed Cubbyshelf, and most will not before their first parcel
:::
::::

## What follows

- The SMS provider account and the sender name are now on the critical path. That is risk R1 in the [risk register](../risks.md).
- The cost of a message goes into the pilot: the shops see their bill before they are asked to pay it.
- Push stays in the spec as a later channel.

## Tasks

- [ ] @maren Read the pilot shops' SMS bill after two weeks and decide whether reminders stay at one 🔽 🛫 2026-11-16 📅 2026-11-27
