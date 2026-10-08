# My life protocol

Overview edited: 2026-10-07. This date does not confirm any practice.

Start here to navigate the protocol. This file owns shared goals and constraints; the linked category pages own the practice records. The baseline has not yet been recorded, which does not mean the user has no routine.

## Browse by category

- [Skin](categories/skin.md) — skincare, sun protection, and skin treatments
- [Hair](categories/hair.md) — washing, scalp care, and hair treatments
- [Oral health](categories/oral-health.md) — dental care and related practices
- [Exercise](categories/exercise.md) — training, sports, mobility, and physical activity
- [Sleep](categories/sleep.md) — sleep routine and environment
- [Nutrition](categories/nutrition.md) — food practices, supplements, and nutritional goals
- [Nails](categories/nails.md) — nail care and treatments

These are navigation categories, not a recommended routine. Add a category when actual use requires it. Keep each practice on exactly one category page; cross-link it from related areas rather than copying it.

## What the state can establish

Practice cards record **last reported status** and **when that status was confirmed**. They describe what the user reported at a particular time. Older information remains visible as a dated report; it must not silently become a claim about current or uninterrupted use.

The assistant updates reports when the user shares a change or confirms relevant details during a conversation. Before a recommendation depends on older information, it should selectively reconfirm the relevant practice. It can show dated summaries without conducting a full check-in. No confirmation date is refreshed merely because a file was edited or a review was performed.

## Goals

No personal health or care goals have been recorded yet.

## Constraints and preferences

| Context | Current information |
| --- | --- |
| Approach | Start small; minimize ongoing research and maintenance effort |
| Choosing alternatives | Consider incremental benefit, compatibility, price, availability, and effort |
| Existing choices | Some are strongly preferred; others were arbitrary. Item-specific reasons are not recorded yet |
| Budget | Not yet provided; do not assume a spending limit |
| Shopping location and stores | Not yet confirmed |
| Relevant conditions, reactions, or clinician instructions | Not yet provided; unknown does not mean absent |

## Format and meaning

- `active`: the user reported doing or using it at the last status confirmation.
- `paused`: the user reported a temporary suspension, with the reason or restart condition if known.
- `stopped`: the user reported stopping it; retain its ID and history.
- `unknown`: an item is recorded, but its use status has not been established.

Use stable IDs such as `P001`, `P002`, and so on across all categories. Never reuse an ID. Use the [practice-card template](../.agents/templates/practice.md) when recording a practice. Keep unknown fields explicitly unknown and optional details limited to what helps a decision.

A candidate that is merely being considered belongs in a [decision record](../decisions/README.md), not in the category pages. Owning a product alone does not establish active use.

Two confirmations separated by months do not establish continuous use between them. Record duration or continuity only if the user explicitly reports it. Dates and measurements must come from actual reports or observations; daily adherence is not inferred. Research findings and their sources belong in decision records.
