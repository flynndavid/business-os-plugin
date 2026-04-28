# Business OS — Cowork Plugin

A Cowork / Claude Code plugin that helps a business owner set up an **AI-ready local workspace** and generate a canonical **Business OS** folder of markdown files.

## What it does

The skill walks the user through a 45-90 minute wizard that produces:

1. **A workspace plan** — a sane local folder layout with explicit Claude-safe boundaries (sensitive material kept OUT of agent reach).
2. **8 Business OS markdown files** — Offers, Pipeline, Delivery, Proof, Ops, Learned, Scoreboard, README — populated with real data, not blank templates.
3. **CLAUDE.md instruction files** — at the workspace root and inside the BusinessOS folder, so any AI agent that opens the workspace knows what's there and how to navigate it.

## How it works

Every step follows **RESEARCH → ASK → GENERATE**:

- **Research** — Claude pulls from connected tools (email, meeting notes, Notion, Drive, Hospitable, Stripe, etc.), the user's website, memory, and past conversations to form a draft.
- **Ask** — Claude presents what it found and asks the user to confirm or correct, instead of asking them to fill in blanks.
- **Generate** — Claude writes the populated artifact (folder plan, markdown file, CLAUDE.md).

No business types are hard-coded. The skill infers from available data and adapts file names + sections to the business shape (service biz, agency, SaaS, property portfolio, content creator, e-commerce, mix).

## Install (Cowork / Claude Code)

```bash
# From the user's plugin marketplace, or by adding this repo as a marketplace source:
/plugin marketplace add <github-url>
/plugin install business-os
```

Or clone this repo into the user's plugin directory and restart Claude Code / Cowork.

## Use

After install, the skill triggers automatically on prompts like:

- "Help me organize my business"
- "Set up my Business OS"
- "Get my files ready for Claude"
- "Build a CLAUDE.md for my workspace"

## Structure

```
business-os/
├── .claude-plugin/
│   └── plugin.json
├── README.md
└── skills/
    └── business-os/
        ├── SKILL.md
        ├── assets/templates/
        │   ├── 00-README.md          # Human overview of the BusinessOS folder
        │   ├── 01-Offers.md          # What we sell, ICP, pricing, objections
        │   ├── 02-Pipeline.md        # Active deals + next actions
        │   ├── 03-Delivery.md        # SOPs + definitions of done
        │   ├── 04-Proof.md           # Case studies, testimonials, results
        │   ├── 05-Ops.md             # Tools, recurring tasks, risk list
        │   ├── 06-Learned.md         # Decisions, experiments, lessons
        │   ├── 07-Scoreboard.md      # Weekly numbers + targets
        │   ├── CLAUDE.md             # AI-instruction file for the BusinessOS folder
        │   ├── Workspace-Plan.md     # Output of the workspace audit phase
        │   ├── Client-Onboarding.md  # Per-client onboarding template
        │   └── Proposal.md           # Standard proposal template
        └── references/
            └── examples.md           # Fallback shape patterns
```

## Author

Built by [Automatic](https://davidflynn.co) — an AI product studio that helps businesses implement AI systems that actually work.
