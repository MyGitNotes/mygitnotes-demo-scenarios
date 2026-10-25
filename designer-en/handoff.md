---
title: Handoff checklist
tags: [mossgate, handoff, specs]
status: in review
---
# Handoff checklist

What Dana, the printer, the signwriter and the app developer each need to work without calling me. Written last, sent after sign-off.

## Colour

| Name | Hex | RGB | Notes |
| --- | --- | --- | --- |
| Moss | `#596B43` | 89, 107, 67 | Primary. Sign, house-blend tin, mark. |
| Clay | `#B9694E` | 185, 105, 78 | Accent. Not for text (3.3 : 1 on oat). |
| Oat | `#F0E9D8` | 240, 233, 216 | Paper and backgrounds. |
| Charcoal | `#30312D` | 48, 49, 45 | Body text. |

Print colours are matched by the printer against a physical swatch, not from these hex values. I will approve the proof.

Spot colour for the label text: Charcoal, mixed to a drawdown on the actual kraft stock. CMYK equivalents for digital proofs only, from a plain conversion of the values above: Moss 17/0/37/58, Clay 0/43/58/27, Oat 0/3/10/6, Charcoal 2/0/8/81.

## Type

- **Headings:** Fraunces, a soft serif with some wobble that echoes the glaze.
- **Text and interface:** DM Sans.

Both are open-licence (SIL OFL) and free to use on print, web and the app. I checked the licences before choosing, so the shop never faces a font invoice later.

## The mark

- Clear space around the mark: the height of the leaf, on all sides.
- Minimum size: 12 mm in print, 24 px on screen. From 8 to 12 mm use the simplified mark (leaf without midrib); do not use the mark below 8 mm. The fern seal is a separate stamp for lids and bag closures, never smaller than 20 mm.
- Never: tilt it, outline it, put it on a photograph without a solid panel, or colour the leaf differently from the arch.

## Name and lockups

- **Wordmark:** MOSSGATE in Fraunces capitals, letter-spaced a little open. This answers the capitals question from the brief. Lowercase "mossgate" would put an "n" shape next to a mark that round 1 worked hard to keep from reading as one, and capitals hold up at sign distance.
- **Lockups:** horizontal (mark left of the wordmark, the mark as tall as two capitals) and stacked (mark above the wordmark). Use the horizontal one on the window vinyl and the tin label, and the mark alone on the hanging sign.
- **Shop name on the window vinyl:** the wordmark in moss on glass, drawn as outlines so no one needs the font.

## Files

| File | Who needs it |
| --- | --- |
| `mossgate-mark.svg`, `.pdf` (vector, four colourways) | Everyone |
| `mossgate-mark-simple.svg` (leaf without midrib, for 8 to 12 mm) | Everyone |
| `mossgate-lockups.svg`, `.pdf` (horizontal and stacked, wordmark outlined) | Printer, signwriter |
| `mossgate-fern-seal.svg` | Stamp maker, bag closures |
| `tin-label-s.pdf`, `tin-label-m.pdf`, `tin-label-l.pdf` (dielines, one spot colour) | Printer |
| `tin-emboss-die.pdf` (mark only, 100% black) | Die maker |
| `window-vinyl.pdf` (cut vinyl, 1:1, one colour) | Vinyl cutter |
| `sign-artwork.pdf` (1:1 at 60 cm) | Signwriter |
| `ui-tokens.json` (colours and type) | App developer |
| `poster-template.pdf` (editable date band) | Dana |

## Before I send it

- [x] Colour contrast checked for every text pair
- [x] Font licences checked
- [x] Mark tested at 5 mm, 8 mm and 12 mm in ink
- [ ] Leaf curve redrawn in the master vector
- [ ] Lockups drawn in the master vector
- [ ] Five more people for the "n" test
- [ ] App direction reviewed against the developer's components
- [ ] Dana's written sign-off on the colourways

Sign-off goes by email, with these files attached, so there is one dated record of what was approved.

*This is a sample notebook from [MyGitNotes](https://mygitnotes.com/). [What this example shows](https://mygitnotes.com/use-cases/designer).*
