# Capture or update current state

1. Re-read `state/protocol.md` and the affected category page. Identify whether the input establishes an existing practice, a context change, an observation, a status reconfirmation, or an adopted/paused/stopped practice. A suggestion or question alone does not establish use.
2. Preserve the user's actual wording and uncertainty where it matters. Record partial information now; do not require a complete profile. If the input is ambiguous about current use and that affects the update, ask a focused question or use `unknown` instead of guessing.
3. Reuse the existing stable item ID. For a new practice, search all category pages and allocate the next unused `P` ID. A brand or product replacement serving the same practice can retain the ID; apply the replacement checks below and record the prior context in history. A genuinely distinct practice gets a new ID. Select one category as its canonical home. If needed, add a category page and link it from the overview.
4. Update the relevant practice card using `.agents/templates/practice.md`, or shared context in the overview. Record the last reported status and its actual confirmation date. Date any reported frequency/amount separately; a status-only check must not refresh frequency or dose. Keep one or more user purposes, preference and its reason, observations, and the latest state-decision link in the same card. Preserve evidence links on an unchanged practice; when its product or use context changes, retain only established applicability and label uncertain or historical links as described below. Record an observation as a user report rather than a proven causal effect.
5. Record a dated decision for the update using `decisions/template.md`. Baseline onboarding may use one record for several related items. State what changed and why; link the user's adoption to the reviewed proposal where applicable. Add a record instead of erasing a previous decision.
6. Link item-specific updates from the affected card. Context-only updates can be linked from the affected goal or constraint. Update the overview's edit date only if the overview changed; this is not a practice confirmation. Do not manufacture effective dates or duration: distinguish the recording date, the report date, and any explicitly reported start/stop date. Advance only the confirmation fields supported by the user's statement. If moving a card, preserve its ID, dates, and history and fix its links; do not duplicate it.
7. Inspect the diff and local links. Ensure cards and decisions agree, IDs remain unique across categories, and no unconfirmed field was refreshed or attributed to a replacement. Check that each displayed evidence link identifies its applicability after a context change. Preserve unrelated edits and stopped/paused items. Summarize the changes and any remaining material unknowns.

## Product or regimen replacement checks

Apply these checks when the product, formulation, dose, route, frequency, or other evidence-relevant use changes. Buying another unit of an unchanged product is not a replacement of its context and does not by itself reconfirm use.

1. Capture the before-and-after context in the new state decision: product/formulation and regimen as known, dated usage details, relevant preferences/observations, and prior evidence links. Keep unknown details unknown. Preserve enough of the old context that its reports and evidence remain interpretable after the card is updated.
2. Read each existing evidence decision's assessed outcome and use context. Classify its applicability to the replacement:
   - **Applicable:** the recorded scope covers the replacement's relevant characteristics. Retain the link and explain the match in the state decision. A brand change alone does not invalidate evidence that genuinely covers both products.
   - **Needs reassessment:** relevant identity, formulation, regimen, or evidence scope is missing or uncertain. Label the link with this status and the uncertainty; do not present it as support for the replacement.
   - **Historical:** the review concerns the previous setup and does not cover the replacement. Preserve the link in the state decision/history, or clearly label it historical on the card. Do not present it as current support.

   These labels describe whether the review addresses this setup, not whether its verdict is favorable or certain. A negative or inconclusive review can still be Applicable.
3. If a review already assesses the replacement, attach it only for its matching objective/context. Check every affected objective independently. Preserve original review dates; checking applicability is not a new scientific review. Do not mark the old research conclusion superseded merely because the user switched products: it can remain valid for the old setup.
4. Check product-specific usage and personal facts separately from evidence. An amount, frequency, preference, reaction, or benefit reported for Product A does not automatically describe Product B. Preserve it with A in history; leave B's corresponding details unknown unless the user's report establishes them. Carry forward unaffected practice-level goals or preferences only where their scope is clear. A dose-only change need not erase facts still clearly about the same product.
5. Record the change even if research or replacement details are incomplete. Ask only what matters to the immediate task, and use the review workflow if an applicability assessment needs new research. Do not require a full literature review just to record a switch. A future plan or purchase still does not establish current use.

## Replacement examples

These are fictional examples of the intended update behavior, not executed behavioral tests.

| User input and prior context | Result |
| --- | --- |
| “I switched from A to B.” A had a product-specific review and a reported nightly amount. | Keep the practice ID, record B as reported in use, preserve A's context/history, and leave B's amount/frequency unknown. Label A's product-specific review Historical. |
| “I use B now, once nightly.” A review already covers B for one of two objectives. | Record B's stated frequency with today's report date. Attach the matching review for that objective; assess the other objective separately. |
| “I changed the amount of A.” The existing review covers only the old dose. | Record the new amount as supplied. Preserve facts still about A, and label the old-dose evidence historical for this regimen; uncertain broader applicability needs reassessment. |
| “I bought another bottle of A.” The formulation is unchanged. | Preserve applicable evidence and its dates. The purchase alone does not refresh use confirmation or frequency. |

## Small example

Input: “I use Brand A cleanser every evening. I picked it randomly. I might try Brand B.”

Record a Brand A cleanser card in Skin with last reported status `active`, today's status confirmation, the stated frequency with its report date, and the arbitrary choice. Record the possible alternative in a review only if useful to the task. Do not activate Brand B, assume a skincare goal, or record daily adherence.

Input: “I stopped that cleanser yesterday because it stung.”

Mark the existing practice's last reported status `stopped`, with today's status confirmation. Record the user's reported reason and effective stop date, deriving “yesterday” from the user's date/timezone. Keep its ID and history. Do not infer an allergy or select a replacement unless the user requested a review.

Input six months after a prior report: “Yes, I still use that shampoo.”

Reconfirm the status as of today. Do not assume the old frequency still applies or that use was continuous for six months. If the user instead says “I used it daily without interruption for those six months,” record that scoped continuity claim as a user report.
