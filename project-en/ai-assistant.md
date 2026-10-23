---
title: Working with an AI assistant
tags: [guide, ai]
status: shipped
---
# Working with an AI assistant

These notes are plain Markdown files, so an AI assistant can work on them directly: it reads a note, edits it, and the change shows up in the open editor at once. You do not copy anything between a chat and your notes.

## What it looks like

1. Open the assistant from its button in the header. It docks beside the page and sees which note you have open.
2. Ask in your own words, for example:
   - *"Move Notifications to shipped and tick the criteria that are done."*
   - *"Add an open-questions section to Returns, based on the Pickup flow."*
   - *"Redraw the Pickup flow as a sequence diagram."*
3. The assistant edits the note. Your editor updates immediately, and if you had unsaved text in it, the two are merged.
4. Look at the result in the Changes panel, and keep it or undo it, like any other edit.

## Why it works here

- A note is a file, so there is nothing hidden for the assistant to guess about.
- Every edit is an ordinary change in history, so you can always see what moved and go back.
- The same notes work with or without the assistant. Turning it off loses nothing.

## Try it on this notebook

The [overview](product-overview.md) is a good first request: *"Summarise what is shipped, building and still on the backlog, using the other notes."*

In this demo copy the assistant is not connected. In your own workspace it is available from the assistant button in the header.
