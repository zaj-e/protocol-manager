# Protocol Manager

An AI assistant that evaluates health and personal-care claims against your current routine, evidence, preferences, budget, and real purchasing options. It remembers why a decision was made so you do not have to repeat the investigation.

This first iteration runs through a repository-aware assistant such as Codex. The files supply its instructions and persistent state; there is no separate model, server, or scheduled service.

## Start here

1. Open this folder in your repository-aware assistant. It should read [AGENTS.md](AGENTS.md). If your tool does not automatically load that file, explicitly ask it to read and follow it.
2. Give it one existing routine or a few products. For example: “Record these as my current skincare routine. I like this moisturizer; the cleanser was an arbitrary purchase.”
3. Open [state/protocol.md](state/protocol.md) and choose a category to see what it recorded. Category pages use readable practice sections. These same Markdown files are readable in an editor, a Git hosting service, or any Markdown viewer.
4. Send a claim or question: “This video recommends this product. Would changing from what I use be worthwhile for me?” The assistant follows the review workflow and saves a decision record.
5. Report a real change: “I switched to it yesterday,” or “I stopped because it irritated my skin.” The assistant updates the protocol and records what changed.

You can edit the Markdown files yourself. User edits are authoritative; the assistant must read the latest file rather than overwrite it from conversation memory.

## Where things live

| Path | Purpose |
| --- | --- |
| [docs/north-star.md](docs/north-star.md) | Current product purpose, priorities, and path forward |
| [docs/origin.md](docs/origin.md) | Original intent from the founding conversation |
| [docs/founding-messages.md](docs/founding-messages.md) | Verbatim founding messages and early feedback from this chat |
| [docs/earlier-proposal.md](docs/earlier-proposal.md) | Recovered historical proposal and its design implications |
| [AGENTS.md](AGENTS.md) | Entry instructions and behavioral rules for the assistant |
| [.agents/workflows/review.md](.agents/workflows/review.md) | Evaluate claims and possible changes |
| [.agents/workflows/update.md](.agents/workflows/update.md) | Capture existing practices and update state |
| [state/protocol.md](state/protocol.md) | Shared context and category navigation |
| [state/categories/](state/categories/) | Canonical practice cards grouped by area |
| [.agents/templates/practice.md](.agents/templates/practice.md) | Small format for a dated practice record |
| [decisions/](decisions/README.md) | Dated reasoning, changes, and conditions for reconsideration |
| [evaluations/](evaluations/README.md) | Scientific reasoning cases and honestly scoped execution records |

`.agents/workflows/` contains repository instructions loaded through `AGENTS.md`. These are not automatically installed personal ChatGPT skills, separate agents, or an autonomous agent fleet.

## Persistence and visibility

The canonical protocol consists of `state/protocol.md` for shared context and its linked category pages for practices. Each practice appears in one category only. Decision records explain its history. A recommendation stays in a decision record until you adopt it. Unknown information remains explicitly unknown.

A tool can serve several purposes. Reviews assess a specific outcome and use context, and cards link applicable evidence by objective. The latest state update is kept separate from those evidence links. Ask “update knowledge about this practice for this goal” to reassess selected conclusions with the existing review workflow; the review date does not confirm that you still use it.

Reviews check consequential premises and distinguish measured outcomes from inference. A material correction reconsiders dependent advice and updates evidence links while preserving reported use and original history.

The repository is initialized on `main` with a foundation commit. Later edits can be inspected with `git diff`; save checkpoints with `git add` and `git commit` when useful. Assistant state updates do not require a commit to become canonical. The assistant reports modified paths and meaningful changes after each update.

The source repository is [zaj-e/protocol-manager](https://github.com/zaj-e/protocol-manager), on `main`. The repository is public; personal state and decision records committed and pushed here will also be public. No API keys or external services are required. Online research depends on the assistant's browsing capabilities.

## Staying connected to reality

The assistant learns through your reports and edits; it cannot observe your routine on its own. Each practice stores its last reported status and the date that status was confirmed. Frequency or amount is also a dated report. “Active on October 7” does not establish use six months later or six months of continuous use.

Report changes naturally when discussing a routine. Before making a decision that relies on an older report, the assistant asks a focused question about the relevant practice. If an answer is unavailable, it can still investigate general evidence and give a conditional conclusion. An overview displays the last confirmation rather than demanding that you reconfirm everything.

Time passing does not automatically change a status or refresh a confirmation. No daily interview or scheduled check-in is required. This keeps uncertainty visible; it cannot guarantee live synchronization without new input.

## How this grows

First populate one domain, then use one real incoming claim to exercise a review. Revise the workflow where actual use reveals friction. Read the [North Star](docs/north-star.md) before adding features.

Further splitting a large category, generating a dashboard, adding a mutation CLI, and selective monitoring are possible later steps, each contingent on a demonstrated need. The foundation has no automated monitoring, inventory accounting, daily adherence logging, or application UI.

## Validation scope

The foundation and category revision received structural checks, not independent behavioral validation. The [2026-10-08 author exercise](evaluations/2026-10-08-author-exercise.md) adds targeted source checks, same-session reasoning demonstrations and an executed fictional correction exercise with file-preservation assertions. No independent fresh-session model test or before/after comparison was run. [Regression cases](evaluations/README.md) document how to perform that next. Instructions guide an existing AI; they do not enforce its behavior like application code or guarantee error-free reasoning.
