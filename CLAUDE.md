# TavaLead — Master Context File
> Read this completely before acting. Single source of truth.

## What is TavaLead

AI-powered lead generation product under the TavaTrack brand. Product definition in progress.

**Parent company:** TavaTrack Wyoming LLC  
**Founders:** Matthew + Timmy  
**Stakeholder access:** Nick (TavaTrack founder) — advisory + brand alignment

## Team Roles

| Person | Role | Owns |
|---|---|---|
| Matthew | TBD | TBD |
| Timmy | TBD | TBD |
| Nick | Advisory + brand alignment | TavaTrack brand decisions |

## Business Structure

Under TavaTrack Wyoming LLC (or separate entity — TBD).  
Billing: TBD  
Pricing: TBD

## Tech Stack

*To be defined. Document decisions here as they're made and link to [[stack-decisions]] for rationale.*

| Layer | Tool | Notes |
|---|---|---|
| TBD | | |

## Wiki Operations

**Session start:** (1) Read this file, (2) Read [[index]], (3) Check [[current-issues]]. Git pull runs automatically on your first message — you're always on the latest.

**Session end:** Update [[current-issues]], append Build Log entry, update [[index]], then:
```bash
git add .
git commit -m "describe what you did"
git push
```

**Collaboration rule:** If you're mid-task and leaving work incomplete, note it in [[current-issues]] with your name before pushing. The other person picks it up from there.

**Query:** Read [[index]] first, then read those pages directly. Don't rely on memory — verify against files.

Use Context7 for: any library or API you're unsure about.

## Current Architecture

*To be documented as built. Start with [[architecture-overview]] once the first design decision is made.*

## Coding Conventions

- DB fields: `lowercase_with_underscores`
- No hardcoded credentials — always `.env`
- Phone numbers: E.164 format (+1XXXXXXXXXX)
- Commit messages: imperative present tense ("add scraper" not "added scraper")
- Branch naming: `feature/[short-description]` | `fix/[short-description]`
- PRs required for anything touching shared infra — no direct pushes to main

## Key Decisions

*Log decisions here as they're made so they don't get re-litigated.*

| Date | Decision | Reason |
|---|---|---|
| | | |

## Status

*Updated each session.*

- **Current sprint:** Product definition — what does TavaLead do and for whom?
- **Blockers:** See [[current-issues]]

## Credentials & Accounts

All creds in `.env` files — never committed. Shared secrets stored in [agreed location — TBD].

---
*Last updated: May 2026*
