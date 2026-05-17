# Collaboration Rules

Simple rules that keep two people from stepping on each other.

---

## The one rule that matters most

**Push before you stop. Pull before you start.**

The auto-pull on session start handles the second part. The first part is on you — always push when you're done working.

---

## Personal vs. shared

| Goes in your personal folder (`Matthew/` or `Timmy/`) | Goes in root wiki pages |
|---|---|
| Half-baked ideas | Finished decisions |
| Personal to-do lists | Shared to-do lists (current-issues.md) |
| Draft thinking | Product specs, architecture docs |
| Anything you're not ready to share | Anything the other person needs to know |

---

## Leaving unfinished work

If you stop mid-task, open `current-issues.md` and add a note:

```
## In Progress
- [Matthew] Building the scraper — stopped at step 3, email extraction is broken
```

That way Timmy doesn't have to guess where you were.

---

## If you get a conflict

A conflict means you and the other person both changed the same file at the same time. Git will warn you when you push. Fix it like this:

```bash
git pull
```

Open the conflicted file — you'll see markers like `<<<<<<< HEAD`. Keep both versions of the content (manually merge them), then:

```bash
git add .
git commit -m "resolve conflict in [filename]"
git push
```

If this looks scary — just message the other person and sort it out together. It's always fixable.

---

## CLAUDE.md is shared ground

`CLAUDE.md` is the most important file. Both of you read it, Claude reads it, Nick reads it. Changes to it affect everyone's sessions.

- Don't make big changes to `CLAUDE.md` without a quick check-in
- If you add something important (stack decision, new role, pricing), commit it with a clear message so the other person sees it in `git log`

---

## Commit message convention

Keep it short and in plain English. Start with what you did:

- `"add product definition first draft"`
- `"update current-issues after today's session"`
- `"timmy: scraper prototype v1"`
- `"fix: remove duplicate entry in index.md"`
