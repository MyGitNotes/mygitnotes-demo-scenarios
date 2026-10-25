---
title: Barcode scanning
tags: [spec, backlog]
status: backlog
---
# Barcode scanning

## Why

Typing a name takes about twenty seconds per parcel. On a Monday after a holiday that adds up to an hour of the shopkeeper's day.

## Rough idea

Point the phone at the carrier's label. If the barcode is recognised, fill in the recipient and the shelf suggestion automatically.

## Questions before this is specified

- Which carriers' labels are worth supporting first?
- What happens when the barcode is unreadable? The typed flow must stay.
- Does it need the camera permission on first launch, or only when the shopkeeper taps Scan?

Depends on the [data model](data-model.md) having a place to store the carrier and tracking number.

*This is a sample notebook from [MyGitNotes](https://mygitnotes.com/). [What this example shows](https://mygitnotes.com/use-cases/project).*
