---
name: houdata-documents
description: Create, migrate, restyle, or review editable Houdata and CacheDB documents in native Google Docs or DOCX while preserving headings, numbered lists, tables, links, images, and brand furniture. Use for policies, technical briefs, product documentation, document templates, Google Drive migration batches, or document-layout QA; use a presentation skill for slide decks.
---

# Houdata Documents

Apply the Houdata document system without flattening editable content. Treat `references/tokens.json` as the shared brand-token source and read `references/document-system.md` before changing layout or page furniture.

## Authority

1. Preserve explicit user instructions and authoritative source content.
2. Use the supplied native Google Docs template when one governs the output.
3. Apply this skill for Houdata-specific brand and layout decisions.
4. Use the available Google Docs or document-editing skill for connector safety, native structure, and rendered verification.

Do not change an original source file during migration. Create or update only the designated branded copy.

## Workflow

1. Identify the document as corporate Houdata material or CacheDB product material.
2. Inventory the source hierarchy, native lists, tables, links, images, headers, footers, and section breaks.
3. Copy the native template or approved branded document topology. Do not rebuild a supplied Google Docs template through DOCX.
4. Replace example content while preserving the template's editable structure.
5. Apply the cover, content header, reading column, heading hierarchy, tables, lists, and images defined in `references/document-system.md`.
6. Re-read native structure after every section-, header-, table-, or index-changing edit.
7. Render and inspect every page before accepting the result.
8. For a batch, complete and approve one representative pilot before migrating the remaining documents.

## Brand architecture

- Use `[symbol] houdata.` for corporate identity, cover endorsement, and page furniture.
- Keep `houdata` lowercase and the final period teal when color is available.
- Use **CacheDB** as the product name in product titles and capability documents.
- Do not use `houdata.` as a replacement for the CacheDB product name.

## Preservation rules

- Keep covers, text, tables, and diagrams editable.
- Preserve native numbered and bulleted lists; never replace numbering with typed bullets or a different list type.
- Preserve links, section order, tables, images, captions, and operative policy language.
- Remove example content, accidental blank pages, duplicate headers, and stale template facts.
- Never use a rasterized full-page cover as the editable template surface.

## Batch migration

- Read originals from the user-designated source folder.
- Write only final branded copies to the designated `branded` folder.
- Keep originals unchanged.
- Do not retain abandoned branded variants unless the user requests version history as separate files.
- Track each source-to-destination mapping and final QA state.

## Completion gate

Reject the document when any of these remain:

- different header height or width between content pages;
- header on the editable cover;
- missing logo or incorrect `houdata.` lockup;
- missing lateral reading margin or hanging first line;
- heading indentation that differs from the body column;
- flattened or renumbered lists;
- broken tables, clipped images, blank pages, or rasterized editable content;
- corporate/product naming inconsistency;
- unverified rendered pages.
