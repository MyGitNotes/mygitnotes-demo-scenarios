---
title: Pickup message and reminder
tags: [work-package, backend]
status: blocked
---
# Pickup message and reminder

**Owner:** @tomasz. **Accountable:** @maren. The spec is [Notifications](../project-en/spec-notifications.md).

When a shopkeeper checks a parcel in, the neighbour gets an SMS within a minute that names the shop and carries a six-digit pickup code. If the parcel is still on the shelf after three days, one reminder follows. The first message cannot be turned off. Reminders can. The channel was decided on 14 October: [SMS first](decisions/sms-first.md).

## Done when

- A message from the registered sender name reaches a real phone in under a minute after check-in, in production, not only on the provider's test number.
- The reminder goes out on day three and never twice.
- A neighbour who turned reminders off still gets the first message.

## Where it stands

The code generator and the provider account are done, and the message text is agreed with two shop owners. The work is **blocked on the sender name**: the provider has the registration since 16 October and has not approved it. Until then messages go from the provider's shared test sender, which only reaches phones we have added by hand. This is risk R1 in the [risk register](risks.md).

## Tasks

- [x] @tomasz Generate the six-digit pickup code, unique among waiting parcels ⏫ 🛫 2026-10-12 📅 2026-10-16 ✅ 2026-10-15
- [x] @maren @tomasz Pick the channel for the pickup message ⏫ 🛫 2026-10-12 📅 2026-10-14 ✅ 2026-10-14
- [x] @tomasz Open the account with the SMS provider and send a test message 🔼 🛫 2026-10-14 📅 2026-10-16 ✅ 2026-10-16
- [x] @rhea Write the message text with two shop owners 🔼 🛫 2026-10-19 📅 2026-10-23 ✅ 2026-10-22
- [ ] @tomasz Get the sender name approved by the provider 🔺 🛫 2026-10-16 📅 2026-10-23
- [ ] @tomasz Switch the first message to the registered sender and time it on a real phone ⏫ 🛫 2026-10-26 📅 2026-10-28
- [ ] @tomasz Add the reminder job for parcels still waiting after three days 🔼 🛫 2026-10-26 📅 2026-10-30
- [ ] @ines Add the switch that turns reminders off, never the first message 🔼 🛫 2026-10-26 📅 2026-10-30
