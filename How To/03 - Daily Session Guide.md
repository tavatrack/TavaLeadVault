# Daily Session Guide

Every working session follows the same rhythm. Two things are automatic, one thing is manual.

---

## Starting a session

1. Open Claude Code
2. Make sure you're in the `TavaLeadVault` folder
3. Send your first message

**That's it.** When you send your first message, the vault automatically pulls the latest changes from GitHub. You'll always be working on the most current version without doing anything.

You might see a line like `Already up to date.` or `Updating abc123..def456` — that's the sync happening.

---

## Working

Talk to Claude like you normally would. Because Claude reads `CLAUDE.md` at the start, it already knows:
- What TavaLead is
- Who you are and who else is working on it
- What the conventions are
- What was worked on last session (from `current-issues.md`)

Good openers:
- *"Read current-issues.md and tell me where things left off"*
- *"I want to work on [thing] today — what do we know about it so far?"*
- *"Help me think through how [feature] should work"*

---

## Ending a session

**Before you close Claude Code**, do three things:

### 1. Update current-issues.md
Tell Claude: *"Update current-issues.md to reflect what we did today and what's left."* Claude will do this for you.

### 2. Commit your changes
Open Terminal, go to the vault folder, and run:

```bash
cd ~/Desktop/TavaLeadVault
git add .
git commit -m "brief description of what you did"
git push
```

Example commit messages:
- `"add product definition notes"`
- `"update architecture diagram"`
- `"matthew scratch: initial market research"`

### 3. That's it
Timmy (or Nick) will get your changes automatically next time they start a session.

---

## If you forget to push

Not the end of the world. Just push next time before you start. The other person might start a session on slightly old info, but nothing breaks.

---

## Quick reference

| What | How |
|---|---|
| Pull latest | Automatic on first message |
| Save your work | `git add . && git commit -m "message" && git push` |
| See what changed | `git status` |
| See who changed what | `git log --oneline` |
