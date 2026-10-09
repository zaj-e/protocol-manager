# North Star

Version: 6. Founded: 2026-10-07. Basis: the user's founding conversation, subsequent feedback, and recovered earlier proposal.

Source wording: [2026 founding messages and early feedback](founding-messages.md) and the [recovered earlier proposal](earlier-proposal.md). [origin.md](origin.md) provides a concise synthesis. These archives preserve what was said; the current charter describes the direction now.

## Purpose

Reduce the time and mental effort required to decide what health and personal-care practices are worth maintaining or changing. Turn incoming products, advertisements, recommendations, and new evidence into decisions that fit the user's actual goals, existing setup, preferences, budget, and access.

Success is a suitable, sustainable protocol that is easy to understand and maintain. The system should help the user avoid unnecessary investigations and changes while identifying improvements that matter.

## What drives the product

- The user already has practices and products. Some choices are strongly preferred; others were arbitrary. Capture the distinction and its reasons.
- Remembering a bottle or noticing it is running out usually needs little assistance. Routine inventory is not the principal value.
- Health and personal-care recommendations create a stream of noise. Evaluating credibility, relevance, compatibility, and incremental benefit is exhausting.
- Evidence and personal needs can change. Preserve enough reasoning to reconsider a conclusion without starting over.
- A theoretically better choice can be unsuitable because of price, availability, added effort, or a negligible advantage. Practical fit belongs inside the decision process.
- Begin small. Grow through demonstrated needs rather than accumulating features.
- Stay honest about reality: the assistant has dated reports, not live access to the user's behavior. Reconfirm relevant older information when a decision depends on it, with minimal check-in burden.
- Make the protocol easy for the user to browse by category as it grows. Human readability is part of its value.
- Support tools with multiple purposes. Tie each evidence conclusion to a specified objective/outcome and use context, rather than treating a product as globally validated.
- Allow selected conclusions to be challenged and reassessed on demand as evidence and needs change. Keep the evidence review date separate from confirmation of actual use.
- Reduce the user's scientific fact-checking burden: independently examine consequential premises, distinguish established findings from inference, and reconsider dependent advice when reasoning fails. Useful recommendations should communicate material uncertainty without requiring zero risk or perfect knowledge.

## Foundation commitments

One assistant, a readable overview linking canonical category pages, a single file for reported adverse reactions, topic research pages, and two task workflows. Review on request. Keep personal observations and meaningful prior product/setup context with each practice; keep reaction details in `state/reactions.md`, linked from cards. Represent practice state as last reported status with confirmation dates; never assume continuous use from elapsed time. A routine report or unchanged confirmation does not require a separate event record.

Practice cards can list several purposes and link research by objective. Reuse subject files in `research/`, with current conclusions and clearly labeled meaningful prior revisions on the same page. Preserve sources, use context, and why a conclusion changed without generating a chronological file per review. Selective reassessment checks earlier reasoning rather than automatically trusting it; a proposal remains separate from adopted use.

Important personal history must be discoverable before the user or assistant remembers to ask for it. Personalized product reviews consult the canonical reactions file and search relevant past setups and topic research, including stopped products and unknown reaction causes. Finding no recorded match does not establish no prior reaction. Verify retrieval with isolated fictional cases; structural checks and workflow instructions alone do not establish behavioral reliability. Markdown and scoped links support this foundation without a database or duplicate master history.

The user's personal health goals, exact products, budget, and shopping options still need to be provided. Founding the project does not supply those facts.

## Learn through use

1. Record one existing routine without making the user fill in a comprehensive questionnaire.
2. Review one actual claim against that baseline and the user's practical options.
3. Capture an adopted change or a reason to keep the current setup.
4. Observe what the user still had to research, remember, or repeat. Improve that bottleneck.

Judge early usefulness by whether the assistant saves investigation, explains its recommendation clearly, preserves current state accurately, and avoids unnecessary change. No numerical score or “state of the art” obligation is required.

## When to add structure

| Observed need | Possible response |
| --- | --- |
| A category becomes difficult to navigate | Split that category further while preserving one canonical home per practice |
| Repeated edits cause format or consistency errors | Add validation or a small update tool |
| Opening Markdown proves inconvenient | Generate a view from canonical state |
| A specific unresolved question merits watching | Add narrowly scoped monitoring with a clear trigger |

These are options, not a committed roadmap. Before adding anything, name the actual friction it solves and how it supports the purpose above.

## Revising direction

This charter is editable. When experience or the user's instruction changes the product, revise the current purpose and scope, increment the version, and append a short dated entry below with what changed and why. Consult [origin.md](origin.md) for the original intent; do not let it veto later explicit direction.

### Revision history

- 2026-10-07 — V1: establish the foundation from the user's stated research burden, practical constraints, preference differences, and request for an adaptable project.
- 2026-10-07 — V2: address the user's concerns about drift from actual behavior and readability at scale. Make status confirmations explicit, reconfirm relevant older reports on demand, and replace the master practices table with category pages and short practice cards. Preserve the original purpose and avoid daily interviews or a separate database.
- 2026-10-08 — V3: incorporate the [recovered earlier proposal](earlier-proposal.md). Explicitly support multiple purposes, objective-specific evidence, systematic reviews/meta-analyses as appropriate sources, and selective reassessment through the existing workflow. Preserve the current emphasis on decision support and practical fit; the earlier inventory framing does not override it.
- 2026-10-08 — V4: operationalize premise checking and correction of dependent advice, and explicitly allow standalone knowledge findings in existing review records. Preserve actionable guidance and small scope; add behavioral evaluation cases without claiming prompt instructions guarantee reliable reasoning.
- 2026-10-09 — V5: narrow the proposed V4 change to premise checking and correction handling; defer standalone-finding format changes. Independent behavioral benefit remains unverified.
- 2026-10-09 — V6: at the user's request, replace numbered chronological records with meaningful history on practice cards, one canonical reactions file, and research organized by topic/objective. The user identified growing diary entries and silent retrieval misses as risks. Preserve all recorded baseline details, sources, dates, and meaningful research revisions; remove the retired event-record files and templates. Keep the original decision-support purpose and make history checks explicit before personalized product advice. No independent retrieval-reliability claim is made by this migration.
