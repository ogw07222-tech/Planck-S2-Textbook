# Chapter 4 Audit — 함수는 입력을 출력으로 보내는 규칙

- **Audit target commit:** migration baseline (see Git history)
- **Audit date:** 2026-08-29
- **Verdict:** **FAIL / REVISE — RECOVERY REQUIRED**

## Evidence

The supplied independent audit cross-checked the latest Volume 1 DOCX and production MASTER. The MASTER claimed Chapters 1–4 were DRAFT COMPLETE, but the actual textbook DOCX ends after the Chapter 3 production record. Chapter 4 body, F005, and F1X02 are absent from the actual artifact.

## Scientific errors

No Chapter 4 physical claim can be audited as completed because the body is missing. The chapter must remain a mathematical preparation chapter and must not be promoted to a Planck-S² physical proof.

## Mathematical errors / required content

The recovered body must explicitly state:

- a function assigns **exactly one** target value to each domain element;
- a function need not be one-to-one;
- one input simultaneously assigned to two different outputs is not a function;
- domain and target/codomain are distinct roles;
- target/codomain and the actual image/range need not be identical;
- outputs may be numbers, points, colors, directions, etc.;
- the chapter prepares the notation $f:X\to Y$, $x\mapsto f(x)$ and later $n:S^2\to S^2$.

## Educational errors

The missing body means the intended progression from S² to map language is broken. Recovery must restore the long-form educational sequence rather than replacing it with a short wiki summary.

## Figure errors

- **F005:** missing in latest DOCX media.
- **F1X02:** missing in latest DOCX media.
- Both require actual assets plus the three-part caption boundary: 볼 것 / 뜻하는 것 / 뜻하지 않는 것.

## Source issues

The production MASTER was ahead of the real artifact and therefore cannot be used as the current progress source of truth. `STATUS.md` now records the corrected status.

## Required fixes

1. Recover the complete Chapter 4 body from a trustworthy saved working copy, if one exists; otherwise draft it anew only in `volume-1/04-function.md`.
2. Restore F005 and F1X02 as real assets.
3. Re-audit the chapter after recovery.
4. Only then change Chapter 4 to DRAFT COMPLETE.
5. **Do not start Chapter 5 before recovery and audit are complete.**

## Final status

**RECOVERY REQUIRED / OPEN.**
