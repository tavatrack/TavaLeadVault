# How Claude Reads the Vault

Understanding this makes you 10x better at using Claude in here.

---

## What Claude reads automatically

Every session, Claude reads `CLAUDE.md` first. That file contains:
- What TavaLead is
- Who's on the team and what they own
- The tech stack and conventions
- Current status

This means you never have to re-explain the project. You can just say *"help me build the scraper"* and Claude already knows what you're building, what tools to use, and what conventions to follow.

---

## What Claude doesn't read automatically

Everything else — the wiki pages, your personal folder, `current-issues.md` — Claude only reads when you or Claude explicitly references it.

**Good habit:** start sessions by telling Claude to read `current-issues.md`:
> *"Read current-issues.md and tell me where we left off"*

Or if you're going deep on something:
> *"Read Architecture/overview.md before we start"*

---

## How to update Claude's knowledge

If you make a decision that should be permanent — a stack choice, a pricing decision, a role change — tell Claude to write it into `CLAUDE.md` or the relevant wiki page. That way every future session has the updated context.

Example:
> *"We've decided to use Supabase as the database. Add that to CLAUDE.md under Tech Stack and create a stack-decisions.md page explaining why."*

---

## The wiki link system

Pages reference each other with `[[double brackets]]` like `[[current-issues]]`. This works in both Claude Code and Obsidian. When you tell Claude to read a page, use the same format:
> *"Read [[architecture-overview]] and summarize the current design"*

---

## What makes Claude less useful

- Letting `CLAUDE.md` get stale — if it doesn't reflect what's actually happening, Claude gives outdated advice
- Not updating `current-issues.md` — Claude won't know what's in progress
- Asking Claude things that are already documented without pointing it to the doc — always reference the page

---

## The memory system

The vault also has a `MEMORY.md` file (and a `memory/` folder when it grows). This is for facts that should persist forever — account credentials structure, key decisions, things Claude should never forget. You don't need to manage this manually — just tell Claude *"remember that..."* and it will handle it.
