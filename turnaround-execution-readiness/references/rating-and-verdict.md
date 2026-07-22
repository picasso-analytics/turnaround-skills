# Ratings & Verdict

## RAG is based on realness, not artifact existence

A system does **not** go green because a plan/binder/schedule exists. It goes green because it
survives the interrogation — proven, owned, wired in, and able to pass its tell.

**Execution Control Systems (Track 1):**

- **Green — Ready / Real:** exists, **named owner with bandwidth**, sustainable mechanism, right
  cadence, **proven** (prior-TA evidence or dry-run), working **action loop**. Passes the tell.
- **Amber — At Risk:** exists but **materially gapped** — no prior-TA proof, owner unclear or
  overloaded, cadence too slow, or a weak action loop. **Recoverable if closed before execution.**
- **Red — Not Ready:** absent, or **paper-only** (can't pass the tell), or fatally gapped. Will
  hurt execution.

**Time-Phased Readiness (Track 2):** same colors, but **calibrated to T-minus** — on-track for
the runway (green) / at-risk-for-the-runway (amber) / showstopper or can't-close-in-time (red).
See `time-phased-readiness.md`.

## The overall verdict

**Judgment-led, ECS-weighted, time-aware — never mechanical color-summing** (summing colors is
just the checkbox trap wearing a suit). Reason to the verdict and defend it with named findings.

Two forces drive it:

1. **ECS is weighted heavily** — the control systems are the crown jewels.
2. **Every gap is weighed against the runway left to close it** (RAG × time-to-close). An amber
   at T-6mo is recoverable; the same amber at T-2wk is effectively red — no time to fix it.

**Anchor rules:**

- **Any ECS Red** (a control system absent or paper-only) → **Not Ready** — *unless* there's a
  **credible, resourced closure plan achievable in the remaining T-minus**, in which case it
  drops to **Ready with Conditions** (the conditions = those closure actions, with owners and
  dates).
- **ECS Ambers + time-phased gaps** → judged by **runway**: closeable before execution →
  **Ready with Conditions**; not closeable in time → escalates toward **Not Ready**.
- **All Green / on-track for the runway** → **Ready.**

The verdict **always names the specific blocking findings and the conditions** — never just a
color or a vibe.

## Verdict labels

- **Not Ready**
- **Ready with Conditions**
- **Ready**

## Writing a finding

Each finding in the register carries:

- **Item** — which system (1–9) or domain (1–12).
- **RAG** — red / amber.
- **The gap** — what's missing or paper-only, stated plainly.
- **Why it matters in execution** — the concrete consequence (schedule slip, safety exposure,
  phantom progress, nightshift drag, etc.).
- **Severity** — informed by RAG × time-to-close.
- **Closure condition** — what must be true to close it, with **owner and date placeholders**.
  Flag *what* must close; do **not** architect the fix (diagnostic posture).
