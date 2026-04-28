# Workspace Plan — [Business Name]

> Generated during Business OS setup (Phase 0.5). This is the plan for how local files are organized for AI-safe use.

## Top-level layout

```
[ASCII tree of the proposed structure goes here]

Example:
~/Documents/[BusinessName]/
├── BusinessOS/                  ← canonical operating docs (this skill creates these)
│   ├── 00-README.md
│   ├── CLAUDE.md
│   └── 01-Offers.md … 07-Scoreboard.md
├── Properties/                  ← per-asset folders, AI-safe
│   ├── PropertyA/
│   │   ├── CLAUDE.md
│   │   ├── Reports/
│   │   ├── Maintenance/
│   │   └── Listings/
│   └── PropertyB/…
├── Reports/                     ← automated outputs (Hospitable, Stripe, etc.), AI-safe
├── Templates/                   ← reusable docs, AI-safe
└── _Sensitive/                  ← NOT shared with AI
```

## What's safe for AI

These folders can be opened in Claude Code, Cowork, or any agent and have their contents read:

| Folder | What's in it |
|--------|-------------|
| `BusinessOS/` | Canonical operating docs |
| `Properties/` (or equivalent) | Per-asset folders with reports, listings, maintenance |
| `Reports/` | Automated outputs (PMS, accounting, analytics) |
| `Templates/` | Reusable docs |

## What stays OUT of AI reach

Never open these folders in an agent context. Keep them sibling-only — not nested inside any folder you'd point an agent at.

| Folder | Why |
|--------|-----|
| `_Sensitive/` | Tax docs, bank statements, identity docs |
| | (add others as needed) |

## Where to store this workspace

- **Local-only** (recommended): `~/Documents/[BusinessName]/` — fastest for AI agents, no cloud sync delays
- **Cloud-synced with offline access**: Drive/Dropbox folder set to "available offline" — works but slower than local
- **Cloud-only**: NOT recommended — agents will hit network latency on every file read

## Suggested moves (if refactoring an existing folder)

| Current location | Move to | Why |
|------------------|---------|-----|
| `~/Desktop/2024-Taxes.pdf` | `_Sensitive/Taxes/` | Sensitive material out of agent reach |
| `~/Downloads/Property-A-monthly-report.pdf` | `Properties/PropertyA/Reports/` | Per-asset organization |
| | | (add others) |

## CLAUDE.md placement

Every folder an agent might open should have a CLAUDE.md. Minimum:

- `BusinessOS/CLAUDE.md` — full instructions (use the `assets/templates/CLAUDE.md` template)
- Workspace-root `CLAUDE.md` — short, points at sub-folders, flags `_Sensitive/` as DO NOT READ
- Per-asset `CLAUDE.md` — even one-liners are fine ("Property A — Reports/, Maintenance/. Owner: X. Cleaner: Y.")

## Last updated

Date: YYYY-MM-DD
