---
name: houdata-diagram-assets
description: Create or review Houdata architecture diagrams, presentation visuals, and technical-document assets using Lucide, Simple Icons, and Houdata-specific semantic assets. Do not use for general product-console UI icons.
---

# Houdata Diagram Assets

Use this skill for Houdata presentations, architecture diagrams, technical documents, and sales-engineering visuals. It does not replace the standard icon library already used by the Bulma product console.

The first Houdata-specific semantic assets live in `assets/icons/`. Extend that family only for concepts that generic libraries cannot express clearly.

## Asset sources

- Use Lucide for general technical concepts and neutral UI symbols.
- Use Simple Icons for external technology and vendor logos; check the individual license and brand guidance before distribution.
- Use Houdata-specific SVG assets for proxy, targeted invalidation, agent policy, and Observe → Decide → Act → Measure concepts.

## Houdata geometry

- Use a 24×24 base grid with a 2 px optical stroke.
- Prefer geometric construction, straight segments, and restrained corner rounding.
- Use a consistent visual weight; do not mix filled and outline styles without a semantic reason.
- Design diagram symbols for 24–64 px first; presentation assets may be larger.
- Keep the symbol's folded-plane language as a restrained motif, not as a logo repeated throughout a diagram.

## Semantic palette

- Ink/graphite: default and neutral icons.
- Accent teal: active, connected, optimized, selected, or intelligent action.
- Amber: attention, pending, degraded, or requires review.
- Red: error, unsafe consistency, or destructive action.
- Warm white: dark-surface inverse icons.

Read shared values from `references/tokens.json`.

## Core diagram families

- Query, normalized query, slow query, query plan.
- Database, table, row/ID, protocol translation.
- Proxy, route, connection, upstream.
- Cache hit, cache miss, stale, invalidation, dependency.
- Agent, recommendation, Rhai rule, simulation, approval, rollback.
- Latency, throughput, time series, health, alert.

## Delivery rules

- Prefer standalone SVG with an accessible label when interactive.
- Do not embed text inside an icon.
- Provide light-surface, dark-surface, and monochrome variants where applicable.
- Prefer SVG assets that remain editable in PowerPoint, Google Slides, and diagram tools.
- Document the meaning and provenance of every non-obvious asset.
