# Changelog — hexa-bot

All notable changes to `hexa-bot` (need-singularity Robot substrate) are
documented in this file.

Format: [Keep a Changelog](https://keepachangelog.com/en/1.1.0/)
Versioning: [Semantic Versioning 2.0.0](https://semver.org/spec/v2.0.0.html)

---

## [1.0.0] — 2026-05-06

### Added

- Initial extraction from `n6-architecture@c0f1f570`.
- 4-verb spec corpus (HEXA family pattern):
  - `robotics/robotics.md`        ← `domains/infra/robotics/`
  - `transport/robotics-transport.md` ← `domains/infra/robotics-transport/`
  - `automation/control-automation.md` ← `domains/infra/control-automation/`
  - `dog_robot/dog-robot-test.md` ← `domains/life/dog-robot-test/`
- `cli/hexa-bot.hexa` placeholder dispatcher (4 sub-command + status +
  selftest + help + version).
- `hexa.toml` package manifest (MIT, hexa-lang ≥1.0.0).
- `install.hexa` hx install hook (no-op pre, selftest post).
- `tests/test_selftest.hexa` — 4-verb spec presence sentinel test.
- `LICENSE` (MIT).

### Status (raw#10 honest C3)

- 0/4 verbs empirically wired. All 4 ship as `.md` spec corpus.
- Working `.hexa` numerical sandbox deferred to post-v1.0 cycles.
- motorcycle / drone / autonomous-vehicle stack OUT-OF-SCOPE — planned
  for `need-singularity/hexa-mobility` standalone.

### Cross-link

- Sister: `need-singularity/hexa-bio` (molecular, 1/4 wired)
- Cousin: `need-singularity/hexa-codex` (AI substrate)
- Cousin: `need-singularity/anima` (consciousness substrate)
- Cousin: `need-singularity/lumiere` (apps-axis spike)

### Provenance

- Extracted-from: `n6-architecture@c0f1f570`
- Extraction date: 2026-05-06 (UTC)
