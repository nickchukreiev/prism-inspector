# Prism — UX/UI & Accessibility Inspector
### A skill for Claude Code

Complete interface quality toolkit: UX/UI design critique + WCAG 2.2 AA accessibility compliance.
One entry point. You choose the depth.

---

## What's inside

```
prism-toolkit/
├── prism/                       ← Main unified tool (start here)
├── uxui-inspector-universal/    ← Standalone UX/UI only
└── wcag-inspector-universal/    ← Standalone accessibility only
```

Install `prism` for the full experience.
The standalone skills are for users who want only one type of audit.

---

## Three modes

Drop in any interface: screenshot, Figma URL, live URL, or HTML file.

```
🎨  UX/UI   — design quality, 30 UX laws, interaction patterns
♿  WCAG    — WCAG 2.2 AA compliance, pass/fail per criterion
✨  Both    — complete picture (recommended)
```

**UX/UI Quick Audit** (~2 min) → critical issues, risk table, quick wins
**UX/UI Full Audit** (~10 min) → 30 UX laws, cognitive load, Norman's 3 levels, competitive patterns, Nielsen heuristics
**WCAG Audit** → exact contrast ratios, keyboard nav, ARIA, heading structure, legal risk flags

At the end — always offered: go deeper · run the other inspector · export PDF

---

## Supported inputs

Screenshot (PNG/JPG) · Figma URL · Live URL / localhost · HTML file

---

## Supported languages

**EN · UA · RU · ES · DE · JA · FR**

Prism detects your language from your first message and responds throughout the session.
UX law names and WCAG criterion IDs always stay in English as international identifiers.

---

## Installation

Requires: [Claude Code](https://claude.ai/code)

**Download:** [Latest release →](../../releases/latest)

### Install Prism only (recommended)
```bash
cp -r prism ~/.claude/skills/
```

### Install everything
```bash
cp -r prism uxui-inspector-universal wcag-inspector-universal ~/.claude/skills/
```

**Windows:** copy folder(s) to `C:\Users\<YourName>\.claude\skills\`

Restart Claude Code or start a new session. Skills load automatically.

---

## Usage examples

```
give me UX feedback [screenshot]
check accessibility https://example.com
full audit [figma URL]
audit this [HTML file]
beide analysieren [screenshot]       ← German
зроби повний аудит [screenshot]      ← Ukrainian
revisa este diseño [URL]             ← Spanish
このUIをチェック [screenshot]         ← Japanese
```

---

## Example session

```
You:   [screenshot] give me UX feedback

Prism: ## 🎨 UX/UI Quick Audit — Login Screen
       🔴 Critical: no error state on failed login
       🟡 Moderate: CTA label "Submit" is outcome-ambiguous
       ⚡ Quick win: add placeholder text to email field

       What's next?
       • 🔬 Full UX/UI Audit (~10 min) — say "full audit"
       • ♿ WCAG check — say "wcag"
       • 📄 Export PDF — say "export PDF"

You:   both

Prism: [runs WCAG + combined summary with issues ranked by priority]

You:   export PDF

Prism: ✅ Saved: prism-audit-login-2026-05-07.html
       Open in browser → Cmd+P (Mac) / Ctrl+P (Win) → Save as PDF
```

---

Made by [@mchukreiev](https://linkedin.com/in/mchukreiev) · Powered by Claude
