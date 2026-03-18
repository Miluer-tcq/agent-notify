# PR: Add agent-notify to claude-code-skills collection

## Skill: agent-notify

**Repository:** https://github.com/Miluer-tcq/agent-notify

**Description:** Cross-platform notification sound & taskbar flash for AI coding agents. When Claude needs confirmation or completes a task, plays a system sound and flashes the taskbar/dock icon. Supports Windows, macOS, and Linux.

**Key features:**
- One-click setup wizard (bilingual EN/ZH)
- Auto-detects OS and agent environment (Claude Code, OpenClaw, Codex, Kiro, Cursor)
- Configurable custom sounds and flash count
- System hooks: Notification + Stop events

**Category:** Productivity

**Install:**
```bash
git clone https://github.com/Miluer-tcq/agent-notify.git
cp -r agent-notify ~/.claude/skills/
```

Then say `notify` or `提示音` in Claude Code.
