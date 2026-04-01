# EventHive: Risk Assessment Wizard

> AI-powered step-by-step wizard that turns your venue's generic risk assessment PDF into a complete event-specific risk register. Upload the venue PDF, import supplier data, and walk through each risk area.

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Part of EventHive](https://img.shields.io/badge/Part%20of-EventHive-orange)](https://eventhive.io)

![Screenshot](thumbnail.png)

## Quick Start

### Browser Mode (no install)

1. Download the [latest release](../../releases/latest) or clone this repo
2. Open `tool.html` in any modern browser
3. Start using it — data saves automatically (requires EventHive hosting for full cloud sync)

### Also Available on EventHive

This tool is available on [EventHive](https://eventhive.io) — the free platform for event professionals. On EventHive, your data syncs across devices, integrates with your other tools, and includes AI assistance from Erleah.

> **AI features** in this tool are optional. They require an API key (OpenAI, Anthropic, or compatible).
> All core functionality works without AI.

---

## Features

- Upload venue risk assessment PDF for AI analysis
- Import supplier and activity data from Ops Tracker
- Step-by-step guided risk identification wizard
- AI-suggested controls and 5×5 P×S risk scores
- Risk register with all standard hazard categories
- Mitigation action tracking
- Export risk register for Risk Assessment Compiler

---

## Customising This Tool

This tool was built using AI-assisted development ("vibe coding").
To customise it for your needs:

1. **Fork this repo** (click the Fork button above)
2. **Clone your fork** locally
3. **Read the [AI Coding Docs](https://github.com/Visual-Hive/ai-coding-docs)** — our methodology for building tools like this with AI
4. **Open in your AI editor** (Claude Code, Cursor, Copilot, etc.)
   - The `.clinerules` file gives your AI assistant context about this tool
   - For Claude Code: run `claude` and the rules load automatically
5. **Modify, test, deploy** — it's just HTML, CSS, and vanilla JS

> **Tip:** The `manifest.json` file defines the configuration schema.
> If you add new configurable options, update it so your tool works with the EventHive platform's config editor.

---

## Data Storage

| Mode | Where | Persistence |
|------|-------|-------------|
| Browser | localStorage (fallback) | Until browser data cleared |
| EventHive | Cloud database (PostgreSQL) | Synced across devices |

This tool stores data in `eventhive_event_{eventSlug}_risk`. In cloud-hosted mode on EventHive, data is synced to a PostgreSQL database.

---

## Related Tools

- [Risk Assessment Compiler](https://github.com/Visual-Hive/eventhive-tool-risk-assessment-compiler) — exports risk register to Compiler
- [Event Ops Task & Supplier Tracker](https://github.com/Visual-Hive/eventhive-tool-ops-tracker) — imports supplier and activity data

---

## Contributing

PRs welcome! Please read the [Contributing Guide](https://github.com/Visual-Hive/eventhive-tools/blob/main/CONTRIBUTING.md) first.

---

## License

MIT — free to use, modify, and distribute.

Built by [Visual Hive](https://visualhive.io) as part of the [EventHive](https://eventhive.io) open-source toolkit.
