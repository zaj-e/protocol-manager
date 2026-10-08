# Capture or update current state

1. Re-read `state/protocol.md` and the affected category page. Identify whether the input establishes an existing practice, a context change, an observation, a status reconfirmation, or an adopted/paused/stopped practice. A suggestion or question alone does not establish use.
2. Preserve the user's actual wording and uncertainty where it matters. Record partial information now; do not require a complete profile. If the input is ambiguous about current use and that affects the update, ask a focused question or use `unknown` instead of guessing.
3. Reuse the existing stable item ID. For a new practice, search all category pages and allocate the next unused `P` ID. A brand or product replacement serving the same practice can retain the ID with the prior product recorded in history; a genuinely distinct practice gets a new ID. Select one category as its canonical home. If needed, add a category page and link it from the overview.
4. Update the relevant practice card using `.agents/templates/practice.md`, or shared context in the overview. Record the last reported status and its actual confirmation date. Date any reported frequency/amount separately; a status-only check must not refresh frequency or dose. Keep purpose, preference and its reason, observations, and the latest decision link in the same card. Record an observation as a user report rather than a proven causal effect.
5. Record a dated decision for the update using `decisions/template.md`. Baseline onboarding may use one record for several related items. State what changed and why; link the user's adoption to the reviewed proposal where applicable. Add a record instead of erasing a previous decision.
6. Link item-specific updates from the affected card. Context-only updates can be linked from the affected goal or constraint. Update the overview's edit date only if the overview changed; this is not a practice confirmation. Do not manufacture effective dates or duration: distinguish the recording date, the report date, and any explicitly reported start/stop date. Advance only the confirmation fields supported by the user's statement. If moving a card, preserve its ID, dates, and history and fix its links; do not duplicate it.
7. Inspect the diff and local links. Ensure cards and decisions agree, IDs remain unique across categories, and no unconfirmed field was refreshed. Preserve unrelated edits and stopped/paused items. Summarize the changes and any remaining material unknowns.

## Small example

Input: “I use Brand A cleanser every evening. I picked it randomly. I might try Brand B.”

Record a Brand A cleanser card in Skin with last reported status `active`, today's status confirmation, the stated frequency with its report date, and the arbitrary choice. Record the possible alternative in a review only if useful to the task. Do not activate Brand B, assume a skincare goal, or record daily adherence.

Input: “I stopped that cleanser yesterday because it stung.”

Mark the existing practice's last reported status `stopped`, with today's status confirmation. Record the user's reported reason and effective stop date, deriving “yesterday” from the user's date/timezone. Keep its ID and history. Do not infer an allergy or select a replacement unless the user requested a review.

Input six months after a prior report: “Yes, I still use that shampoo.”

Reconfirm the status as of today. Do not assume the old frequency still applies or that use was continuous for six months. If the user instead says “I used it daily without interruption for those six months,” record that scoped continuity claim as a user report.
