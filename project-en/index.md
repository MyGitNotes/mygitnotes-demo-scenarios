---
title: Welcome to the product spec
tags: [guide]
status: shipped
---
# Cubbyshelf: product spec

Cubbyshelf is a small app for corner shops that hold parcels for neighbours. A shopkeeper checks a parcel in, the neighbour is told it has arrived, and the parcel is handed over with a code. Everything here is a made-up example.

## What to try

1. **Switch to the Kanban view.** The notes are cards in four columns: *backlog*, *specifying*, *building*, *shipped*. Drag a card to another column, or change its status from the dot, and the file's status changes with it.
2. **Read the diagrams.** [Pickup flow](spec-pickup-flow.md), [Notifications](spec-notifications.md) and [Data model](data-model.md) each carry a diagram written as text. Open any of them in source mode and change a line to watch the diagram redraw.
3. **Ask the assistant to edit.** [Working with an AI assistant](ai-assistant.md) explains how an assistant can read and change these notes directly, and what you see when it does.
4. **Scan the status board.** Under *Notes*, a `status-board` groups the notes by how far along they are, and each entry links to its note.
5. **Edit freely.** This is a demo copy: your changes stay in your browser for 24 hours and never reach anyone else.

## Notes

::::status-board{title="Where each note stands"}
:::group{status="done" title="Shipped"}
- [Product overview](product-overview.md)｜the problem, the idea and what v1 does
- [Working with an AI assistant](ai-assistant.md)｜how an assistant edits these notes
:::
:::group{status="partial" title="Building"}
- [Notifications](spec-notifications.md)｜two of four acceptance criteria met
:::
:::group{status="partial" title="Specifying"}
- [Pickup flow](spec-pickup-flow.md)｜three open questions
- [Data model](data-model.md)｜four things to store
:::
:::group{status="none" title="Backlog"}
- [Barcode scanning](spec-barcode-scan.md)｜questions to answer before it is specified
- [Returns](spec-returns.md)｜questions to answer before it is specified
:::
::::

*This is a sample notebook from [MyGitNotes](https://mygitnotes.com/). [What this example shows](https://mygitnotes.com/use-cases/project).*
