# UI/UX Inspector — Universal Skill for Claude Code

A deep UI/UX audit skill for any product, platform, or audience.
Works with screenshots, Figma URLs, live URLs, and HTML files.

## What it does

- **Quick Audit** (~2 min) — critical issues, risk table, quick wins
- **Full Audit** (~10 min) — 30 UX laws, cognitive load, emotional design (Norman), competitive patterns, full risk table
- **Smart Intake** — asks up to 3 questions before starting if context is missing
- **Any language** — responds in the user's language (English default)
- **Any product type** — auto-detects category and picks relevant competitor references

## Installation

**Requires:** [Claude Code](https://claude.ai/code) (CLI or desktop app)

1. Move the `uxui-inspector-universal` folder into your Claude skills directory:

```
~/.claude/skills/uxui-inspector-universal/
```

On Mac/Linux:
```bash
mv uxui-inspector-universal ~/.claude/skills/
```

On Windows:
```
Move the folder to: C:\Users\<YourName>\.claude\skills\
```

2. Restart Claude Code (or start a new session).

3. The skill is now available. Trigger it by sharing a screenshot, Figma URL, or live URL and asking for a UX/UI review.

## Usage examples

```
[attach screenshot] — what's wrong with this UI?
[figma.com/...] — do a full audit
[localhost:3000] — check this design
audit this screen [html file]
```

To go deeper after a Quick Audit, reply: `full audit` or `yes`.

For accessibility compliance, use `/wcag-inspector` (separate skill).

## Trigger phrases

EN: "check this design", "audit this screen", "what's wrong with this UI", "give me UX feedback", "analyze this mockup", "ui review", "ux audit", "review this prototype"

UA: "перевір інтерфейс", "зроби аудит", "що не так з цим екраном"

RU: "проверь интерфейс", "сделай аудит", "покритикуй", "дай фидбек по дизайну"

ES: "revisa este diseño", "audita esta pantalla"

---

Made by [@mchukreiev](https://www.linkedin.com/in/mchukreiev/) · Powered by Claude
