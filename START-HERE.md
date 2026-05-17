# TavaLead — Start Here

Welcome to the shared vault. Read this once, then work from `CLAUDE.md` and `current-issues.md`.

---

## First-time setup (do this once)

### 1. Clone the repo

```bash
git clone https://github.com/tavatrack/TavaLeadVault.git ~/Desktop/TavaLeadVault
```

### 2. Open in Claude Code

Open your terminal in the `TavaLeadVault` folder and launch Claude Code. The `CLAUDE.md` loads automatically — Claude will have full context every session.

### 3. Open in Obsidian (optional but recommended)

Open Obsidian → Add vault → Open folder as vault → select `TavaLeadVault`. All the `[[wiki links]]` will work natively. You can read and write notes in Obsidian, and they'll sync to the other person through git.

### 4. Your personal folder

`Matthew/` and `Timmy/` folders are yours for personal scratch notes and draft ideas. Shared decisions and finished thinking go in the root wiki pages.

---

## Every session — the two rules

**Before you start:** Git pull happens automatically when you send your first message to Claude. You're always on the latest.

**Before you stop:** Commit and push your changes.

```bash
git add .
git commit -m "describe what you did"
git push
```

If you leave something unfinished, note it in `current-issues.md` with your name before pushing so the other person knows where things stand.

---

## How the vault works

| File | Purpose |
|---|---|
| `CLAUDE.md` | Master context — Claude reads this first every session |
| `index.md` | Map of all wiki pages |
| `current-issues.md` | Active blockers and in-progress work |
| `Matthew/` | Matthew's personal notes |
| `Timmy/` | Timmy's personal notes |
| `Architecture/` | System design docs |
| `PRDs/` | Product requirements |
| `Build Log/` | Session-by-session log of what was built |
| `Research/` | Market research, competitor notes, references |

---

## If you get a git conflict

Someone pushed while you were working. Run:

```bash
git pull
```

If there's a conflict in a markdown file, open it, keep both versions of the content (merge manually), then commit. Don't lose anyone's work.

---

*Questions → ask Nick.*
