# Your First Session

Setup is done. Here's how to actually start working.

---

## Open the vault in Claude Code

1. Open Claude Code
2. Open the `TavaLeadVault` folder — File → Open Folder → select it from your Desktop
3. You should see the vault files in the sidebar

---

## Send your first message

Type this to Claude:

> *"Read CLAUDE.md and current-issues.md. Tell me where the project stands and what we should be working on."*

Claude will read both files and give you a summary of the project and what's been left open. This is how every session starts.

---

## Your first real task

The product isn't fully defined yet — that's intentional. Your first job as a team is to answer:

- What does TavaLead actually do?
- Who is the customer?
- How does it make money?

Start that conversation with Claude:

> *"We're defining what TavaLead is. Here's what I'm thinking: [your idea]. Help me stress-test it — who's the customer, what's the problem we're solving, and how does this make money?"*

Claude will push back, ask the right questions, and help you build it out. When you land on something solid, tell Claude to write it into `CLAUDE.md` so it's locked in for every future session.

---

## End your first session

When you're done, even if nothing is finished:

1. Tell Claude: *"Update current-issues.md to reflect what we discussed today"*
2. Then run in Terminal:

```bash
cd ~/Desktop/TavaLeadVault
git add .
git commit -m "first session — [one line of what you did]"
git push
```

That's it. The other person gets your work next time they start.

---

## You're in the rhythm now

Every session from here follows `How To/03 - Daily Session Guide.md`. First session is the same as every other session — read the files, do the work, push when done.
