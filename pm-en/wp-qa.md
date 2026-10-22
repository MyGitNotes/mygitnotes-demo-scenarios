---
title: Test plan
tags: [work-package, qa]
status: in progress
---
# Test plan

**Owner:** @kofi. **Accountable:** @maren.

The v1.0 regression suite stays, and v1.1 adds cases for the message, the reminder and the code check. Everything runs on the two beta groups, TestFlight internal on iOS and the internal track on Android, then on the three pilot shops' own phones before the release candidate.

:::parts{title="Test cases by area" unit="cases"}
- Check-in and waiting list｜38｜Carried over from v1.0
- Pickup message｜20｜Content, timing, wrong number
- Reminder｜14｜Day three, off switch, never twice
- Code check at the counter｜24｜Right code, wrong code, used code, name fallback
- Store and upgrade｜16｜Update from 1.0, fresh install, offline start
:::

## How a bug is handled

A bug found in beta gets a title that a shopkeeper would understand, the build number, and one of three levels. **Blocker** stops the release: check-in, the message or the code check does not work. **Major** is fixed before the release candidate. **Minor** goes to v1.2. @kofi sets the level and @maren is the only one who can lower a blocker.

## Tasks

- [x] @kofi Update the v1.0 regression suite for the new check-in screen 🔼 🛫 2026-10-12 📅 2026-10-16 ✅ 2026-10-16
- [x] @kofi Set up the TestFlight internal group and the Android internal track 🔼 🛫 2026-10-13 📅 2026-10-19 ✅ 2026-10-20
- [ ] @kofi Run the full regression on the first beta build ⏫ 🛫 2026-10-30 📅 2026-11-03
- [ ] @kofi @leo Run the counter flow in the three pilot shops 🔼 🛫 2026-11-02 📅 2026-11-05
- [ ] @kofi Retest on the release candidate 🔺 🛫 2026-11-06 📅 2026-11-09
