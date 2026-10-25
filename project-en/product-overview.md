---
title: Product overview
tags: [spec, overview]
status: shipped
---
# Product overview

## The problem

Corner shops end up holding parcels for the whole street. They keep them behind the counter with a pen-and-paper list, and a neighbour who comes by when the shop is busy waits while the shopkeeper hunts.

## The idea

Cubbyshelf turns the pen-and-paper list into three steps:

1. **Check in.** The shopkeeper types the recipient's name and a shelf number, and the parcel is logged.
2. **Notify.** The neighbour is told it has arrived and gets a six-digit pickup code. See [Notifications](spec-notifications.md).
3. **Hand over.** The neighbour shows the code, the shopkeeper confirms it, and the parcel is marked collected. See [Pickup flow](spec-pickup-flow.md).

## What shipped in v1

- Check-in by typing a name and a shelf number.
- A list of waiting parcels, oldest first.
- Marking a parcel collected.

## Not in v1

Barcode scanning ([Barcode scanning](spec-barcode-scan.md)) and returns ([Returns](spec-returns.md)) are still on the backlog.

*This is a sample notebook from [MyGitNotes](https://mygitnotes.com/). [What this example shows](https://mygitnotes.com/use-cases/project).*
