# Changelog

All notable changes to this skill are documented here.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this skill adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.1.0] — 2026-05-18

### Added

- **Quick config (YAML)** block in Section 0 — drop-in `config.yaml` for agents that read structured config, including a `schedule.windows` block for cron timing.
- **Compatibility table** in Section 0 — install paths for Claude Code, OpenClaw, ClawHub, Cursor / Copilot CLI, and generic LLM agents.
- **Section 7 — First-run checklist**: 7-item checklist before enabling any cron, plus a bash one-liner to init memory files.
- **Section 8 — Reply skeletons**: 3 drop-in reply templates (Answer-first, Empathy + redirect, Polite correction) with "what to never paste verbatim" guardrails.
- **Section 9 — FAQ**: 6 questions (OpenClaw requirement, multi-account, X API rate limits, threads vs single tweets, Premium/Blue, suspension handling).
- `init-memory.sh` script shipped with the GitHub repo — interactive or non-interactive memory dir bootstrap; idempotent.

### Changed

- README badges updated to v1.1.0.

### Unchanged (no breaking changes)

- Sections 1-6 (the core doctrine) are byte-identical to v1.0.0. Existing crons keep working without modification.

## [1.0.0] — 2026-05-18

### Added

- Initial release.
- Three-role mental model (`tw-post` / `tw-engage` / `tw-stealth`) for any X account.
- Human-like browser discipline: right page first, let UI load, read before clicking, click once and verify.
- Full cron-by-cron playbook: weekly planning, notifications check, keyword monitor (morning/midday/evening), reply pass, original posts (morning/noon/evening), thread generator, result publish, daily metrics recap.
- Strict reply qualification — no impulse posting, no generic CTAs.
- Full recovery playbook (browser down, frozen, account cockpit unstable, too many tabs, composer stuck, page unusable).
- Explicit anti-patterns to avoid.
- `install.sh` for one-command install into Claude Code or OpenClaw skills directories.

[1.1.0]: https://github.com/AlexBloch-IA/twitter-account-operations/releases/tag/v1.1.0
[1.0.0]: https://github.com/AlexBloch-IA/twitter-account-operations/releases/tag/v1.0.0
