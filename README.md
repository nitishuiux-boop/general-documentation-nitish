# General Documentation - Nitish

A Claude Code skill that makes any documentation task land in one shot, written the way Nitish wants it, without re-explaining preferences every time.

## What it does

- Runs 5 checks before writing: what was asked, smallest output, edit vs create, which page is main, are the claims true.
- Applies clear DO and DON'T rules: plain words, CEO-briefing tone, tables and short lists, airplane-manual structure for configs, evidence only where needed.
- Checks claims against the source of truth (code, data, spec repo) before they go into a doc.
- Handles Notion safely: matches the existing format, avoids column layouts, re-checks toggle nesting after edits.
- Updates itself: after each documentation task, any correction about how docs are written is logged in `learnings.md`.

## Install

```bash
git clone <this repo> ~/.claude/skills/general-documentation-nitish
```

## Files

- `SKILL.md`: the rules
- `learnings.md`: corrections log, read first, overrides SKILL.md
