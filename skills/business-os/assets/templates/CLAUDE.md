# CLAUDE.md — [Folder Name]

> This file tells Claude (and other AI agents) what's in this folder and how to use it. Read this first when opening this folder for any task.

## What this folder is

<!-- One paragraph. Example: "Canonical Business OS for [Business Name]. Source of truth for how this business runs — offers, pipeline, delivery SOPs, proof, ops, lessons, scoreboard." -->


## What lives here

| File / Folder | Purpose | When to read |
|---------------|---------|--------------|
| `00-README.md` | Human overview, weekly ritual, AI prompt templates | Start here for context |
| `01-Offers.md` | What we sell, ICP, pricing, objections | Sales / pricing questions |
| `02-Pipeline.md` | Active deals/clients/opportunities, next actions | Deal status, follow-ups |
| `03-Delivery.md` | How we deliver, definitions of done, SOPs | Project execution, scope questions |
| `04-Proof.md` | Case studies, testimonials, results | Sales enablement, marketing |
| `05-Ops.md` | Tools, recurring tasks, risk list, existing automations | Tooling, automation, operational questions |
| `06-Learned.md` | Decisions, experiments, hard-won lessons | Strategic context, "have we tried this?" |
| `07-Scoreboard.md` | Weekly numbers + targets + sources | Performance, metrics, trends |

## How to navigate this folder

- For **sales / pricing** questions → read `01-Offers.md` then `02-Pipeline.md`
- For **delivery / SOP** questions → read `03-Delivery.md` then per-asset folders if applicable
- For **operational / tooling** questions → read `05-Ops.md`
- For **strategy / historical context** → read `06-Learned.md`
- For **metrics / performance** → read `07-Scoreboard.md` and follow the source links to `Reports/`

## Sibling folders (workspace structure)

<!-- Reference the Workspace Plan from Phase 0.5 -->
- `../Properties/` (or `../Clients/`) — per-asset folders, each has its own CLAUDE.md
- `../Reports/` — automated outputs (e.g. monthly Hospitable reports, Stripe exports)
- `../Templates/` — reusable docs
- `../_Sensitive/` — **DO NOT READ.** Tax docs, bank info, identity docs. Privacy boundary.

## Update protocol

- This folder is the source of truth. Files here are canonical.
- When proposing updates, present them as **suggested edits** — do NOT auto-write to these files without explicit user confirmation.
- The user runs a Friday 10-minute ritual to keep things current (see `00-README.md`).
- Stale data is worse than no data — if information here looks out of date, flag it and ask the user before relying on it.
- When you DO write to a file, update the `Last updated:` date at the top.

## Privacy notes

<!-- Adapt to the user's situation -->
- [If using placeholders] Real client names are masked as "Client A", "Client B" etc. Don't infer real names unless the user confirms.
- [If sensitive] No passwords, API keys, or credentials live here. Anything sensitive lives in `../_Sensitive/` and is OUT of your reach.
- This folder may be shared with contractors/VAs. Behave accordingly — no internal-only commentary.

## Last updated

Date: YYYY-MM-DD
