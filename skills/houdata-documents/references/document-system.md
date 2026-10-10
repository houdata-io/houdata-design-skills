# Houdata document system

## Canonical template

Use a user-supplied or otherwise approved native Google Docs template when one governs the output. Create a native copy for each deliverable; do not edit a shared master while migrating source content.

## Brand tokens

- Deep surface: `#071923`
- Ink: `#102331`
- Warm white: `#F7F7F2`
- Accent teal: `#2FAF9F`
- Primary font: Inter
- Headings: Inter Semibold
- Body: Inter Regular

Read the complete shared token set from `tokens.json`.

## Page topology

### Cover

- Use an editable A4 page.
- Use the deep-surface background.
- Show the approved symbol followed by live `houdata.` text; use warm white for the name and teal for the period.
- Do not show the repeating content-page header on the cover.
- Keep the corporate eyebrow, document title, subtitle, document type, and optional metadata editable.
- Use Houdata as the corporate endorsement and name CacheDB in product-document titles.

### Content pages

- Use warm white as the reading surface.
- Use one compact, full-width deep-surface header on every content page.
- Use the approved `[symbol] houdata.` lockup in the header.
- Use 2 pt of vertical cell padding above and below the lockup.
- Make every default, first-page, and section header definition use identical height, width, padding, logo, and text styling.
- Keep the header band independent of reading-column margins.

## Google Docs geometry

Use zero left and right section margins when necessary to keep the header table full width. Apply the reading column to content, not to the section header.

For ordinary content paragraphs and headings, use:

- `indentStart`: 54 pt
- `indentFirstLine`: 54 pt
- `indentEnd`: 54 pt

The three values must match. In Google Docs, `indentFirstLine: 0` with `indentStart: 54` produces an unintended hanging indent: the first line touches the page edge while later lines remain inset.

Headings align to the same reading column as body text. Do not add another lateral heading indent. Express hierarchy through size, weight, color, and vertical spacing.

Preserve approved native table geometry from the template. Tables, images, and boxed content must align optically with the 54 pt reading column and must not force the header band to become inset.

## Type hierarchy

- Corporate eyebrow or section label: Inter Semibold, uppercase when appropriate, accent teal.
- Document title: Inter Semibold, ink on light pages and warm white on dark covers.
- Heading 1: Inter Semibold, ink.
- Heading 2: Inter Semibold; teal may identify a subordinate section when it remains legible and semantic.
- Body: Inter Regular, ink, comfortable line spacing.
- Metadata: smaller Inter Regular or Medium, quiet graphite/ink treatment.

Keep title punctuation natural. The teal final period is mandatory only in the visual `houdata.` lockup, not in every running-text company mention.

## Lists

- Preserve native Google Docs list semantics and list IDs.
- Preserve decimal, multilevel, alphabetical, and Roman numbering from the source.
- Do not turn `1.1`, `1.2`, or other structured numbering into generic bullets.
- Keep list indentation subordinate to the 54 pt reading column rather than resetting the list to the page edge.

## Tables

- Keep tables editable.
- Use a clear ink or deep-surface header row with warm-white text when appropriate.
- Distinguish body rows with restrained alternating warm-white/neutral treatment when the table has multiple rows.
- Keep borders quiet and typography consistent with the document.
- Repeat header rows when a long table spans pages if native Google Docs supports it.
- Verify every table at rendered size; one-row examples do not prove alternating-row behavior.

## Images and diagrams

- Prefer editable diagrams or high-resolution images with preserved aspect ratio.
- Align images to the reading column unless an approved full-width composition requires otherwise.
- Add a concise caption when the image needs interpretation or provenance.
- Do not use a full-page raster image as a document cover template.

## Migration sequence

1. Read the complete source and native structure.
2. Create a native copy of the approved template in the destination folder.
3. Replace cover fields and body content without changing the original.
4. Preserve native lists, tables, links, images, and heading roles.
5. Normalize every header definition, not only the header visible on the current page.
6. Apply the 54/54/54 paragraph-indentation contract to the reading column.
7. Inspect all rendered pages, then repair only the affected ranges.
8. Leave only the accepted branded file in the final folder.

## QA checklist

- Cover is editable and has no repeating header.
- Cover and headers use the correct Houdata symbol and `houdata.` lockup.
- Every content header has the same full width and compact height.
- Header vertical padding is 2 pt above and below.
- Titles, headings, first lines, and subsequent lines share the same reading-column margin.
- Heading levels add no unintended lateral indentation.
- Numbered lists retain their numbering and nesting.
- Tables distinguish header and body rows and remain editable.
- Images are legible, aligned, and not distorted.
- There are no blank pages, clipped elements, duplicate sections, or stale examples.
- Houdata/CacheDB naming follows the brand architecture.
- Connector readback and rendered-page inspection both pass.
