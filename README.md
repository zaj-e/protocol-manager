# Protocol Manager

An AI assistant that evaluates health and personal-care claims against your current routine, evidence, preferences, budget, and real purchasing options. It remembers why a decision was made so you do not have to repeat the investigation.

This first iteration runs through a repository-aware assistant such as Codex. The files supply its instructions and persistent state; there is no separate model, server, or scheduled service.

## Start here

1. Open this folder in your repository-aware assistant. It should read [AGENTS.md](AGENTS.md). If your tool does not automatically load that file, explicitly ask it to read and follow it.
2. Give it one existing routine or a few products. For example: “Record these as my current skincare routine. I like this moisturizer; the cleanser was an arbitrary purchase.”
3. Open [state/protocol.md](state/protocol.md) to see what it recorded. The same Markdown file is readable in an editor, a Git hosting service, or any Markdown viewer.
4. Send a claim or question: “This video recommends this product. Would changing from what I use be worthwhile for me?” The assistant follows the review workflow and saves a decision record.
5. Report a real change: “I switched to it yesterday,” or “I stopped because it irritated my skin.” The assistant updates the protocol and records what changed.

You can edit the Markdown files yourself. User edits are authoritative; the assistant must read the latest file rather than overwrite it from conversation memory.

## Where things live

| Path | Purpose |
| --- | --- |
| [docs/north-star.md](docs/north-star.md) | Current product purpose, priorities, and path forward |
| [docs/origin.md](docs/origin.md) | Original intent from the founding conversation |
| [AGENTS.md](AGENTS.md) | Entry instructions and behavioral rules for the assistant |
| [.agents/workflows/review.md](.agents/workflows/review.md) | Evaluate claims and possible changes |
| [.agents/workflows/update.md](.agents/workflows/update.md) | Capture existing practices and update state |
| [state/protocol.md](state/protocol.md) | Canonical current context and protocol |
| [decisions/](decisions/README.md) | Dated reasoning, changes, and conditions for reconsideration |

`.agents/workflows/` contains repository instructions loaded through `AGENTS.md`. These are not automatically installed personal ChatGPT skills, separate agents, or an autonomous agent fleet.

## Persistence and visibility

The canonical state is `state/protocol.md`. Decision records explain its history; they are not a second current-state database. A recommendation stays in a decision record until you adopt it. Unknown information remains explicitly unknown.

The repository is initialized on `main` with a foundation commit. Later edits can be inspected with `git diff`; save checkpoints with `git add` and `git commit` when useful. Assistant state updates do not require a commit to become canonical. The assistant reports modified paths and meaningful changes after each update.

The source repository is [zaj-e/protocol-manager](https://github.com/zaj-e/protocol-manager), on `main`. The repository is public; personal state and decision records committed and pushed here will also be public. No API keys or external services are required. Online research depends on the assistant's browsing capabilities.

## How this grows

First populate one domain, then use one real incoming claim to exercise a review. Revise the workflow where actual use reveals friction. Read the [North Star](docs/north-star.md) before adding features.

Splitting a large state file, generating a dashboard, adding a mutation CLI, and selective monitoring are possible later steps, each contingent on a demonstrated need. V1 has no automated monitoring, inventory accounting, daily adherence logging, or application UI.

## Validation scope

The foundation was checked for local Markdown links, agreement between the state format and workflows, and clean Git packaging. These are structural checks. Live research and independent behavioral evaluation of the assistant have not been performed. Instructions guide an existing AI; they do not enforce its behavior like application code.
