# hcode

**One-person engineering with a disciplined SDLC approach.**

*Parallel agents. Deliberate integration.*

hcode is a local desktop IDE that lets a solo builder run multiple bounded agent
roles with disciplined handoffs, spec freezes, and merge gates — keeping one
human accountable while the supporting work stays legible and contained.

---

## Why it exists

- **One engineer stays in control** while agents specialize into distinct roles.
- **See collisions before they become conflicts** — overlapping work is flagged
  at review time, not at merge time.
- **Solo work behaves like a disciplined SDLC**, with falsifiable checkpoints
  instead of one long undifferentiated conversation.

---

## The lifecycle (L1–L7)

Each level is a distinct, falsifiable role. Work only moves forward through an
explicit handoff.

| Level | Role                | Agent         | Function                                                  |
| ----- | ------------------- | ------------- | --------------------------------------------------------- |
| L1    | Spec Owner          | Claude        | Writes the contract and freezes the scope                 |
| L2    | Adversarial Review  | Codex         | Challenges ambiguity before code exists                   |
| L3    | Test Author         | Codex         | Writes tests blind to the implementation                  |
| L4    | Implementer         | Antigravity   | Builds against the frozen spec and tests                  |
| L5    | Code Reviewer       | Claude        | Reviews the diff against the contract                     |
| L6    | Execution Harness   | Antigravity   | Runs checks in a controlled environment                   |
| L7    | Script Gate         | Deterministic | Measures the repository and emits the merge verdict       |

---

## Operating invariants (R1–R5)

1. **R1 — Author ≠ Checker.**
2. **R2 — Implementer ≠ Test Author.**
3. **R3 — No model owns final judgment.**
4. **R4 — Handoffs are version-controlled.**
5. **R5 — Measure the actual repository.**

---

## Features

- **Permission review** — approve or deny agent requests without hunting for panes.
- **Conflict-aware review** — Monaco-based diff comparison with overlap flagging.
- **Source control integration** — real terminals, a resizable usage panel, and a
  visible integration queue.
- **Role-based lifecycle** — distinct, falsifiable roles at every handoff.
- **Spec freeze** — after L2 review, the contract is versioned.

---

## Models and tools

hcode drives Claude, Codex, Grok, Antigravity, or a plain shell. You bring your
own subscriptions and credentials.

---

## Built with

Tauri · Rust · React · Vite

---

## Platform and status

| | |
| --- | --- |
| Platform | macOS for now|
| Version | 0.1.5 |
