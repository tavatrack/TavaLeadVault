# First Time Setup

Do this once. Takes about 10 minutes.

---

## Step 1 — Install Claude Code

Claude Code is the AI tool you'll use inside the vault.

1. Go to [claude.ai/code](https://claude.ai/code) and download the desktop app
2. Sign in with your Anthropic account (or create one — it's free to start)
3. Open it. You should see a terminal-style interface.

---

## Step 2 — Install Git

Git is the tool that syncs the vault between your machine and the shared GitHub.

Check if you already have it:
```bash
git --version
```

If you see a version number, you're good. If not:
- **Mac:** install from [git-scm.com](https://git-scm.com) or run `xcode-select --install` in Terminal
- **Windows:** install from [git-scm.com](https://git-scm.com)

---

## Step 3 — Clone the vault

This downloads the vault to your computer. Open Terminal (Mac) or Command Prompt (Windows) and run:

```bash
git clone https://github.com/tavatrack/TavaLeadVault.git ~/Desktop/TavaLeadVault
```

You'll now have a `TavaLeadVault` folder on your Desktop. That's your local copy.

---

## Step 4 — Open the vault in Claude Code

In Claude Code, open the folder:
- Click "Open folder" or use File → Open
- Select the `TavaLeadVault` folder on your Desktop

Claude will automatically read `CLAUDE.md` and have full project context from the start.

---

## Step 5 — Set up GitHub access (so you can push changes)

You need to tell Git who you are so your changes get attributed to you.

```bash
git config --global user.name "Matthew"
git config --global user.email "your@email.com"
```

You'll also need to log in to GitHub. The easiest way:
1. Go to [github.com](https://github.com) and create a free account if you don't have one
2. Send Nick your GitHub username — he'll invite you as a collaborator
3. Accept the invite from your email
4. When you first run `git push`, it'll ask you to log in — use your GitHub credentials

---

## Step 6 — Optional: Open in Obsidian

If you use Obsidian (a note-taking app), you can open the vault there too. All the `[[wiki links]]` in the vault work natively in Obsidian.

- Open Obsidian → Manage vaults → Open folder as vault → select `TavaLeadVault`

You can now read and write notes in Obsidian. Any changes sync through git just like everything else.

---

You're set up. Read `How To/03 - Daily Session Guide.md` next.
