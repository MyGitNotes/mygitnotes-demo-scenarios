---
title: Store release and rollout
tags: [work-package, mobile]
status: planned
---
# Store release and rollout

**Owner:** @ines. **Accountable:** @maren.

Getting a build in front of shops is its own piece of work. Apple says it reviews about 90% of submissions in under 24 hours, which leaves some that take longer, so the plan does not rely on the average: the build is submitted on Friday 6 November, three working days before the go/no-go call, with *release manually* selected. Google Play reviews a release too, and Google says that can take up to seven days or more, so the Android bundle is submitted the same day as the iOS build with managed publishing switched on: once it is approved it waits until @ines publishes it, then goes out as a staged rollout.

## Done when

- The release candidate is tagged, uploaded to both stores, and both builds are approved and waiting to be published.
- Store text, screenshots and the "what is new" note are in place.
- The rollout moves 10%, 50%, 100% only when 24 hours pass with no [rollback trigger](release-plan.md).

## Notes

If review rejects the iOS build, @ines replies the same day, and the go/no-go call on 10 November decides whether to wait or to move the release to 19 November. Expedited review is kept for a blocker found after approval, not for a late submission.

## Tasks

- [ ] @maren @rhea Write the store text and refresh the screenshots 🔼 🛫 2026-11-02 📅 2026-11-06
- [ ] @ines Cut the release candidate build from the release branch ⏫ 🛫 2026-11-05 📅 2026-11-06
- [ ] @ines Submit the iOS build for review with manual release 🔺 🛫 2026-11-06 📅 2026-11-06
- [ ] @ines Submit the Android bundle for review with managed publishing on 🔼 🛫 2026-11-06 📅 2026-11-06
- [ ] @tomasz Watch the error rate and the message count for 24 hours after each rollout step 🔼 🛫 2026-11-12 📅 2026-11-16
- [ ] @maren Raise the rollout to 50%, then to 100%, when no trigger has fired 🔼 🛫 2026-11-13 📅 2026-11-16
