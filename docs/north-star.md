# North Star

Version: 1. Founded: 2026-10-07. Basis: the user's founding conversation.

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

## V1 commitments

One assistant, one readable canonical protocol file, two task workflows, and dated decision records. Review on request. Preserve context, reasoning, and the boundary between a suggestion and an adopted practice.

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
| The current file becomes difficult to navigate | Split by domain with an explicit canonical index |
| Repeated edits cause format or consistency errors | Add validation or a small update tool |
| Opening Markdown proves inconvenient | Generate a view from canonical state |
| A specific unresolved question merits watching | Add narrowly scoped monitoring with a clear trigger |

These are options, not a committed roadmap. Before adding anything, name the actual friction it solves and how it supports the purpose above.

## Revising direction

This charter is editable. When experience or the user's instruction changes the product, revise the current purpose and scope, increment the version, and append a short dated entry below with what changed and why. Consult [origin.md](origin.md) for the original intent; do not let it veto later explicit direction.

### Revision history

- 2026-10-07 — V1: establish the foundation from the user's stated research burden, practical constraints, preference differences, and request for an adaptable project.
