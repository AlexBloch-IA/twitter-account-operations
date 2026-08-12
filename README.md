# Twitter Account Operations

> Operating doctrine for X/Twitter account automation — stable Chrome sessions, role separation (post / engage / stealth), human-like interaction, careful posting, reply discipline, recovery patterns. Use this for any scheduled X activity (cron, agent, recurring task) where account safety and long-term reputation matter more than raw output.

[![License: MIT-0](https://img.shields.io/badge/License-MIT--0-blue.svg)](https://opensource.org/licenses/MIT-0)
[![ClawHub](https://img.shields.io/badge/ClawHub-Published-orange)](https://clawhub.ai/alexbloch-ia/skills/twitter-account-operations)
[![Version](https://img.shields.io/badge/version-1.0.2-green)](https://clawhub.ai/alexbloch-ia/skills/twitter-account-operations)

A Claude Code / [OpenClaw](https://openclaw.ai) skill, published on [ClawHub](https://clawhub.ai/alexbloch-ia/skills/twitter-account-operations). Portable operating doctrine — drop it into an agent's skills directory and follow it.

---

## What the doctrine covers

- Configure for your brand
- Browser architecture
- Human-like browser behavior
- Cron-by-cron guide
- Recovery and failure handling
- Anti-patterns
- Final doctrine
- First-run checklist
- Reply skeletons (drop-in templates)
- FAQ

The full, load-bearing detail lives in [`SKILL.md`](./SKILL.md).

---

## Install

### Via ClawHub (recommended)

👉 **<https://clawhub.ai/alexbloch-ia/skills/twitter-account-operations>**

```bash
clawhub install twitter-account-operations
# or, from an OpenClaw agent:
openclaw skills install @alexbloch-ia/twitter-account-operations
```

### Via this repository (manual)

```bash
git clone https://github.com/AlexBloch-IA/twitter-account-operations.git
cd twitter-account-operations
./install.sh
```

The script copies the full skill payload into every supported stack it finds:

- `~/.claude/skills/twitter-account-operations/` (Claude Code)
- `~/.openclaw/skills/twitter-account-operations/` (OpenClaw)

### Manual copy

```bash
mkdir -p ~/.claude/skills/twitter-account-operations
cp -R SKILL.md ~/.claude/skills/twitter-account-operations/   # plus scripts/, references/, templates/… if present
```

---

## Optional API-backed tooling

This repository is the operating doctrine, not an API client. For structured X/Twitter data or approval-reviewed account actions, pair it with [TweetClaw](https://github.com/Xquik-dev/tweetclaw):

```bash
openclaw plugins install npm:@xquik/tweetclaw
```

Use TweetClaw read tools for tweet, reply, user, and follower evidence. Keep posting, private reads, monitors, webhooks, and other persistent or account-changing actions behind explicit approval. This doctrine remains the safety layer for role separation, reply qualification, draft review, cron timing, and browser recovery.

Xquik is an independent third-party service. Not affiliated with X Corp. "Twitter" and "X" are trademarks of X Corp.

---

## Repository structure

```
twitter-account-operations/
├── SKILL.md
├── README.md
├── LICENSE
└── install.sh
```

---

## License

Released under **MIT-0** (MIT No Attribution). Use, fork, adapt, redistribute — no attribution required.

---

## Author

[Alexandre Bloch](https://github.com/AlexBloch-IA) — founder of [OpenClaw](https://openclaw.ai).
Published on [ClawHub](https://clawhub.ai/alexbloch-ia/twitter-account-operations).
