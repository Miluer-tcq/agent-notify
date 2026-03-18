# PR: Add agent-notify skill

## Summary

Add `agent-notify` — a cross-platform notification sound & taskbar flash skill for AI coding agents.

## What it does

When Claude needs confirmation or completes a task, this skill configures hooks to:
- Play a system sound (or custom audio file)
- Flash the taskbar icon (Windows) / bounce Dock icon (macOS) / show desktop notification (Linux)

## Why it's useful

Users frequently switch to other windows while waiting for Claude. Without notifications, they keep checking back manually. This skill solves that pain point with a one-command setup wizard.

## Features

- Auto-detects OS (Windows/macOS/Linux) and agent environment
- Quick setup (one-click) and custom setup (interactive) modes
- Configurable sound files and taskbar flash count
- Bilingual (English + Chinese) interaction
- Works with Claude Code, OpenClaw, Codex, Kiro, Cursor

## Skill structure

```
agent-notify/
├── SKILL.md (skill.md)
├── scripts/
│   ├── notify-windows.ps1
│   ├── notify-macos.sh
│   └── notify-linux.sh
└── config/
    └── default.json
```

## Testing

Tested on Windows 11 with Claude Code. Sound plays and taskbar flashes correctly on Notification and Stop hooks.
