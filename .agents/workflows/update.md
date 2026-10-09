# Capture or update current state

1. Re-read `state/protocol.md` and the affected category page; read `state/reactions.md` when recording a reaction or checking relevant past experience. Identify whether the input establishes an existing practice, a context change, an observation, a status reconfirmation, or an adopted/paused/stopped practice. A suggestion, purchase, or question alone does not establish use.
2. Preserve the user's actual wording and uncertainty where it matters. Record partial information now; do not require a complete profile. If current use is ambiguous and affects the update, ask a focused question or use `unknown` instead of guessing. Hypothetical examples are not personal reports.
3. Reuse the existing stable item ID. For a new practice, search all category pages and allocate the next unused `P` ID. A product replacement serving the same practice can retain the ID; apply the replacement checks below. A genuinely distinct practice gets a new ID. Select one canonical category, adding a category and overview link only when needed.
4. Update the card using `.agents/templates/practice.md`, or the shared context in the overview. Record last reported status and its actual confirmation date. Date frequency/amount separately; a status-only check must not refresh them. Keep the user purposes, choice and reasons, report source, and dated observations on the card. Preserve applicable objective-specific research links without refreshing review dates.
5. Keep meaningful history with the practice, grouped by product or setup: what changed, why, actual report/effective dates, previous usage details, and observations needed to interpret it. Preserve material prior information before replacing latest fields. A first report can use the card's source and observations; it does not require a duplicate baseline narrative. An unchanged reconfirmation updates only the supported fields and does not require a new diary entry. Context changes stay with the relevant goal or constraint. Do not create numbered event files.
6. Record actual reported adverse reactions only in `state/reactions.md`, in the relevant product/practice section, whether or not a card exists. Include source/report date, any separately reported event date, product identity, use context, description, outcome, and uncertainty about cause. Replace the empty-state statement when the first real report arrives. Keep material follow-up and corrections in that section. Link from the practice card; do not duplicate symptoms or assign a cause, allergy, ingredient, or reaction to a replacement without supporting information.
7. Update the overview's edit date only if the overview changed; it is not a practice confirmation. Distinguish recording/migration date, report date, and explicitly reported start/stop date or continuity. Advance only fields supported by the user's statement. When moving a card, preserve ID, sources, dates, meaningful history, and links; do not duplicate it.
8. Inspect the diff and local links. Ensure one canonical card per ID, one canonical home for reaction details, agreement between cards and relevant research, and no unsupported field refresh or transfer to a replacement. Check retained evidence applicability. Preserve unrelated user edits and stopped/paused items. Summarize changed paths and material unknowns. Ordinary state updates do not create research pages.

## Product or regimen replacement checks

Apply these checks when product, formulation, dose, route, frequency, or other evidence-relevant use changes. Buying another unit of an unchanged product is not replacement or confirmation of use.

1. Preserve the previous setup in the card's meaningful history before updating it: product/formulation and regimen as known, dated usage details, relevant preferences/observations, research links and their assessed context. Link the old product's canonical reactions entry where one exists. Capture the new setup only as reported, keeping missing details unknown.
2. Read each linked research section's assessed outcome and use context. Classify applicability to the replacement:
   - **Applicable:** the scope covers the relevant characteristics. Retain the link and briefly explain the match beside it or in the card's replacement history. A brand change alone does not invalidate research that covers both.
   - **Needs reassessment:** relevant identity, formulation, regimen, or scope is missing or uncertain. Label the link and uncertainty; it is not support for the replacement.
   - **Historical:** the review concerns the previous setup. Preserve the link with that setup in card history, or clearly label it historical if shown beside current evidence.
   These labels identify scope, not whether a conclusion is favorable. A negative or inconclusive review can be Applicable.
3. Attach research already covering the replacement only for matching objectives and contexts. Check objectives independently and preserve review dates. An applicability check is not a new scientific review, and switching products does not supersede a conclusion valid for the old setup.
4. Assess personal facts separately from research. Amount, frequency, preference, reaction, and benefit for Product A do not automatically describe Product B. Preserve A's details in card history or its canonical reactions section, and leave B's corresponding details unknown unless reported. Carry forward unaffected practice-level goals or preferences only where their scope is clear. A dose-only change need not erase facts clearly about the same product.
5. Record the reported change even if details or research are incomplete. Ask only what matters to the immediate task; use the review workflow when new research is needed. A future plan or purchase still does not establish current use.

## Examples

These are fictional illustrations, not executed behavioral tests.

| User report | Update |
| --- | --- |
| “I switched from A to B.” | Keep the practice ID; preserve A's dated setup and observations in card history and any reaction in its canonical entry. Report B active; leave B's amount/frequency unknown. Classify each research link for B. |
| “I use B now, once nightly.” | Record B's status and frequency with the report date. Link matching research for each objective independently; do not transfer unrelated findings. |
| “I changed the amount of A.” | Preserve the previous amount/context and record the new amount. Retain personal facts still clearly applicable; reassess research scope without refreshing review dates. |
| “I bought another bottle of A.” | Preserve reported-use dates and applicable research. The purchase alone does not refresh status or frequency. |
| “I stopped that cleanser yesterday because it stung.” | Record stopped status with today's report date and yesterday's effective stop date in the user's timezone. Put the dated reaction report in `state/reactions.md`, link it from the retained card, and infer no allergy. |
| “Yes, I still use that shampoo,” after six months. | Reconfirm status only. Preserve the older frequency date; do not infer continuous use. An explicit report of daily uninterrupted use can establish only the period actually reported. |

For “I use Brand A every evening; I picked it randomly; I might try B,” record A with dated status/frequency and its arbitrary choice. B remains a candidate in relevant research if a review is requested; it is not activated.
