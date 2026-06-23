# web-monitor — Monitor web pages for content changes

> Track any URL for updates with CSS selector targeting and local diff storage. No external service needed.

[![OpenClaw Skill](https://img.shields.io/badge/OpenClaw-Skill-blueviolet)](https://github.com/NachaFromMars)

## Overview
web-monitor watches web pages for content changes using a Python script with beautifulsoup4. Stores snapshots locally, computes diffs, supports CSS selectors to monitor specific sections. All data stays on your machine.

## Features
- Add URLs with optional CSS selector targeting
- Check all or one URL for changes
- View diffs between snapshots
- Local storage — no external service

## Usage / Quick Start
```bash
uv run --with beautifulsoup4 python scripts/monitor.py add "https://example.com" --name "Site"
uv run --with beautifulsoup4 python scripts/monitor.py add "https://example.com" -n "Pricing" -s ".pricing-table"
uv run --with beautifulsoup4 python scripts/monitor.py check
uv run --with beautifulsoup4 python scripts/monitor.py diff "Pricing"
```

## Trigger Keywords (OpenClaw)
watch website, monitor page, track changes, detect updates, page change alerts, new posts monitor

---
Part of the [NachaFromMars](https://github.com/NachaFromMars) OpenClaw skill ecosystem.
