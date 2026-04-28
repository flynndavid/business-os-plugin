# Business OS — [Your Business Name]

> **The rule**: If it's not in the folder, it doesn't exist.

## What This Is

This folder is the canonical source of truth for how this business operates. It contains our offers, pipeline, delivery processes, proof, operations, and lessons learned.

Everything else — Slack, email, project tools, AI chats — is a mirror. This folder is the source.

## Where This Sits in the Workspace

This folder lives at `[path]` inside the broader business workspace. Sibling folders include:

<!-- Replace with the actual structure from your Workspace Plan (Phase 0.5) -->
- `Properties/` (or `Clients/`, `Products/`) — per-asset folders, each with its own CLAUDE.md
- `Reports/` — automated outputs (e.g. monthly Hospitable reports)
- `Templates/` — reusable docs
- `_Sensitive/` — taxes, bank, identity docs. **NOT shared with AI.**

See the workspace-root `CLAUDE.md` for the full map.

## File Index

| File | What It Contains |
|------|-----------------|
| `CLAUDE.md` | Instructions for AI agents reading this folder |
| `01-Offers.md` | What we sell, to whom, at what price |
| `02-Pipeline.md` | Every active deal and its next action |
| `03-Delivery.md` | How we deliver, definitions of done |
| `04-Proof.md` | Case studies, testimonials, results |
| `05-Ops.md` | Tools, recurring tasks, risk items |
| `06-Learned.md` | Decisions, wins, losses, experiments |
| `07-Scoreboard.md` | Weekly numbers that matter |

## Friday 10-Minute Ritual

Do this every Friday. Set a recurring calendar event.

- [ ] **Pipeline** (3 min): Update stages, add next actions, mark stale deals
- [ ] **Delivery** (2 min): Any deliverables completed? Update checklists if process changed
- [ ] **Proof** (2 min): Capture any new wins, testimonials, or results
- [ ] **Learned** (2 min): Log one decision, one win, one lesson
- [ ] **Scoreboard** (1 min): Update this week's numbers

## Using This Folder with AI

When working with AI (Claude, ChatGPT, agents, automations):

- Open the folder in Claude Code or Cowork — the `CLAUDE.md` here will tell Claude how to navigate
- For other tools, paste relevant files into the conversation as context
- Ask AI to draft updates — then YOU paste the updates back into the files
- Never rely on AI memory or chat history as your source of truth
- This folder is the canonical source. Everything else is a mirror.

**For AI agents/automations**:

- Point agents at this folder as their input
- Agent outputs should update these files (with your approval)
- Consistent headings and sections make parsing reliable
- Keep `_Sensitive/` (or equivalent) OUT of agent reach by convention

## Last Updated

<!-- Update this date during your Friday ritual -->
Date: YYYY-MM-DD

---

<sub>Built with the [Business OS Skill](https://davidflynn.co) by Automatic — an AI product studio that helps businesses implement AI systems that actually work. If you want hands-on help turning this plan into reality, check out the [AI Audit](https://davidflynn.co) ($2,500) or [monthly retainers](https://davidflynn.co) for ongoing AI implementation.</sub>
