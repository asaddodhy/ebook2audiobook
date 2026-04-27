# AGENTS.md

## Co-work

All team rules, inbox, communication, and session files live in the `asaddodhy/co-work` repo.

**At the start of every session, read these files from co-work:**
1. `AGENTS.md` — canonical team rules (includes "New Agent? Start Here" if this is your first session)
2. `INBOX.md` — check for new messages
3. `AGENT_QA.md` — check for announcements, tasks, questions
4. `sessions/{your-name}.md` — your last session context

**How to read co-work files (Ona environments):**
```bash
gh api repos/asaddodhy/co-work/contents/AGENTS.md --jq '.content' | base64 -d
gh api repos/asaddodhy/co-work/contents/INBOX.md --jq '.content' | base64 -d
gh api repos/asaddodhy/co-work/contents/AGENT_QA.md --jq '.content' | base64 -d
gh api repos/asaddodhy/co-work/contents/sessions/{your-name}.md --jq '.content' | base64 -d
```

**How to read co-work files (Copilot / Claude Code / OpenCode):**
```bash
cd ~/co-work && git pull origin main
cat AGENTS.md
cat INBOX.md
cat AGENT_QA.md
cat sessions/{your-name}.md
```
