# hexa-bot v1.0.0 — Release Notes

**Date**: 2026-05-06
**Verdict**: SPEC_ONLY (0/4 verbs wired, 4/4 spec corpus)
**Provenance**: `canon@c0f1f570`
**License**: MIT

---

## TL;DR

`hexa-bot` v1.0.0 is the **initial extraction** of the n=6 Robot substrate
into a standalone `need-singularity` repo. It ships as a **spec-first**
4-verb bundle (robotics + transport + automation + dog_robot) with a
placeholder `.hexa` CLI dispatcher. Working numerical sandboxes are
explicitly out-of-scope for v1.0.0.

---

## What's in the box

```
hexa-bot/
├── LICENSE                  MIT
├── README.md                why · verbs · status · install · cross-link
├── CHANGELOG.md
├── RELEASE_NOTES_v1.0.0.md  (this file)
├── hexa.toml                package manifest
├── install.hexa             hx install hook
├── cli/
│   └── hexa-bot.hexa        4-verb placeholder dispatcher
├── robotics/
│   └── robotics.md          ← canon/domains/infra/robotics/
├── transport/
│   └── robotics-transport.md ← canon/domains/infra/robotics-transport/
├── automation/
│   └── control-automation.md ← canon/domains/infra/control-automation/
├── dog_robot/
│   └── dog-robot-test.md    ← canon/domains/life/dog-robot-test/
└── tests/
    └── test_selftest.hexa   4-verb spec presence sentinel
```

---

## 4-verb status table

| Verb         | Status | Working sandbox?            |
|--------------|--------|-----------------------------|
| `robotics`   | SPEC   | NO (post-v1.0)              |
| `transport`  | SPEC   | NO (post-v1.0)              |
| `automation` | SPEC   | NO (post-v1.0)              |
| `dog_robot`  | SPEC   | NO (post-v1.0)              |

---

## Honest scope (raw#10 C3)

- v1.0.0 is **spec-only**. The bundled CLI dispatches sub-commands but
  prints spec-file heads — it executes no working numerical sandbox.
- The n=6 invariant lattice (σ=12, τ=4, φ=2, J₂=24) is inherited from the
  canon canon; no independent verification for the robot axes.
- **motorcycle is intentionally absent.** It belongs to a planned post-v1.0
  standalone (`need-singularity/hexa-mobility`) covering the autonomous
  mobility bundle (motorcycle + drone + autonomous-vehicle, 자율 이동체).
- No real-hardware actuation. No ROS2 bridge. No safety certification.
  This repo is a spec corpus + dispatcher skeleton.

---

## Cross-link

- Sister substrate: `need-singularity/hexa-bio` (molecular, 1/4 wired —
  the precedent pattern this repo follows).
- AI substrate cousin: `need-singularity/hexa-codex`.
- Consciousness substrate cousin: `need-singularity/anima`.
- Apps-axis cousin: `need-singularity/lumiere`.
- Upstream canon: `need-singularity/canon` @ `c0f1f570`.

---

## Next cycle hooks

- Working `.hexa` modules per verb (4 × `<verb>/module/<verb>.hexa`).
- Falsifier preregister table per verb (mirroring hexa-bio stub pattern).
- Decision: spawn `hexa-mobility` standalone for autonomous mobility axis,
  or fold into a 5th verb here? (TBD next cycle.)
