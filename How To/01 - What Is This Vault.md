# What Is This Vault?

## The simple version

The vault is a shared folder that lives on your computer. Inside it are markdown files (just text files) that act as a shared brain for the project — notes, decisions, docs, and context.

When you open Claude Code inside this folder, Claude automatically reads all of it. So every time you ask Claude something, it already knows the project, your roles, the conventions, and where things left off.

## Why it's not in the cloud (and why that's fine)

The vault lives on your laptop, not in the cloud. That's intentional — Claude works with local files.

But it stays in sync with the other person through GitHub (like Google Drive but for code). Every time you start a session, your vault automatically pulls the latest from GitHub. When you're done, you push your changes back up. Matthew gets your changes, you get Matthew's. It stays in sync without you having to think about it much.

```
Your laptop          GitHub (middle copy)       Other person's laptop
TavaLeadVault/  ←──  tavatrack/TavaLeadVault  ──→  TavaLeadVault/
   (local)              (shared in cloud)               (local)
```

## What lives in the vault

| File / Folder | What it is |
|---|---|
| `CLAUDE.md` | The master brief — Claude reads this first, every session |
| `START-HERE.md` | First-time setup guide |
| `current-issues.md` | What's in progress, what's blocked |
| `index.md` | Map of all pages in the vault |
| `Matthew/` | Matthew's personal scratch notes |
| `Timmy/` | Timmy's personal scratch notes |
| `Architecture/` | How the product is built |
| `PRDs/` | Product requirements |
| `Build Log/` | Log of what was done each session |
| `Research/` | Market research, competitor notes |
| `How To/` | These guides |

## What the vault is NOT

- It's not a live shared session. You and Timmy don't talk to the same Claude at the same time — you each have your own.
- It's not stored in the cloud. It's on your machine. GitHub is just the sync layer.
- It's not automatic backup. You have to push when you're done (see the session guide).
