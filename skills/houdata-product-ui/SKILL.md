---
name: houdata-product-ui
description: Build or review Houdata's Bulma-based database proxy admin and operations console, including metrics, query tables, cache states, agent workflows, and light/dark modes. Use for the product console; marketing website work is outside this skill's scope.
---

# Houdata Product UI

Use this skill for the Houdata admin and operations console. It assumes Bulma is the implementation framework and `houdata-brand-ui` is the source of brand tokens.

## Workflow

1. Read `references/tokens.json` and apply its semantic colors.
2. Model the task as an operator workflow: discover, inspect, decide, act, verify.
3. Use Bulma primitives where possible; add Houdata-specific modifiers instead of unrelated one-off styles.
4. Support both dark and light modes for every new screen.
5. Validate dense tables, keyboard focus, empty/loading/error states, and responsive degradation.

## Console patterns

- Overview: query rate, cache hit ratio, latency, database time, cache time, invalidations, and resource use.
- Query explorer: searchable table with normalized query, database, frequency, latency, hit/miss, affected tables, and agent analysis action.
- Query detail: time series, executions, cache events, invalidations, dependencies, and recommended Rhai rule.
- Rule workflow: proposal, explanation, simulation, approval, rollout, measurement, and rollback.
- Status language: teal for active/optimized/connected; amber for attention; red for error or unsafe consistency; neutral graphite for inactive.

## Visual rules

- Prefer calm density over visual noise.
- Keep primary actions obvious and secondary actions quiet.
- Use cards for summary metrics, tables for investigation, drawers for detail, and modals only for consequential confirmation.
- Never make teal the default color of every icon or label.
- Preserve clear separation between database time and cache time.

## Acceptance checklist

- Bulma-compatible markup and modifiers.
- Dark and light variants.
- Accessible contrast and keyboard focus.
- Distinguishable hit, miss, invalidated, stale, error, and loading states.
- Agent-generated rules are presented as proposals with auditability and rollback.
