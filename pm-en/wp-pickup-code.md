---
title: Code check at the counter
tags: [work-package, mobile]
status: in progress
---
# Code check at the counter

**Owner:** @ines. **Accountable:** @maren. The spec is Pickup flow.

A neighbour shows the six digits from the message. The shopkeeper types them in, the app shows the parcel, and one tap marks it collected. A code works once. After collection it is dead.

## Done when

- A valid code finds exactly one waiting parcel, and the screen says whose it is.
- A code that was already used, or does not exist, is refused with a message the shopkeeper can read out loud.
- Name matching still works as the last resort, and says so on screen. The wording is the open decision below.
- Collecting never deletes a parcel. It leaves the waiting list and stays in the history.

## Notes

The counter screen is the one place a shopkeeper uses with a neighbour waiting, so the target is under ten seconds from the first digit to "Collected". @rhea drew it with large digits and one primary button, and the first build runs on @ines's phone.

Open question from the spec: what the shopkeeper sees when the code is wrong and the neighbour offers a name instead. Two neighbours can share a name, so the screen must make the fallback feel like a fallback.

## Tasks

- [ ] @rhea Design the counter screen: six digits in, parcel out 🔼 🛫 2026-10-12 📅 2026-10-16
- [ ] @ines Build code entry and the Collected confirmation ⏫ 🛫 2026-10-19 📅 2026-10-29
- [ ] @tomasz Make a code work once and refuse it after collection ⏫ 🛫 2026-10-21 📅 2026-10-27
- [ ] @maren @rhea Decide the wording shown when the code does not match and a name is tried 🔽 🛫 2026-10-23 📅 2026-10-28
- [ ] @kofi Write the test cases for a wrong code, a used code and two parcels with one name 🔼 🛫 2026-10-26 📅 2026-10-29
