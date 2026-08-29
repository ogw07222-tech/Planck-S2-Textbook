# Chapter 12 Audit — 출발점으로 돌아오기: loop

- **Audit date:** 2026-08-29
- **Canonical file:** `volume-1/12-loop.md`
- **Verdict:** **PASS — CHAPTER 13 DRAFT APPROVED**

## 1. Standard loop definition audit

**PASS.**

The chapter defines a loop as a path

$$
\gamma:[0,1]\to\mathcal C
$$

with

$$
\gamma(0)=\gamma(1)=n_0.
$$

This agrees with the standard algebraic-topology definition. Allen Hatcher, *Algebraic Topology*, §1.1 likewise defines loops as paths whose starting and ending point is the same and calls that common point the basepoint.

## 2. Endpoint equality versus triviality

**PASS.**

The chapter correctly separates

$$
\gamma(0)=\gamma(1)
$$

from the stronger statement that the loop is contractible to a constant loop. This is the key conceptual bridge to homotopy and is stated repeatedly without prematurely classifying any specific Planck-S² loop.

## 3. Basepoint / homotopy preparation

**PASS.**

`basepoint`, `contractible`, and `homotopy` are introduced only as forward references. The chapter does not attempt to define the full fundamental group before the scheduled later chapters.

## 4. Physical-time boundary

**PASS.**

The chapter carries forward the Chapter 11 distinction between a mathematical path parameter and actual physical time evolution. It does not claim that an electron physically executes a loop merely because a loop exists in a mathematical configuration space.

## 5. Planck-S² / FR boundary audit

**PASS.**

The chapter explicitly refuses to infer any of the following from the generic loop definition alone:

- a specific $2\pi$ spatial-rotation loop is nontrivial;
- it is the $\mathbb Z_2$ generator;
- it automatically produces an FR phase $-1$;
- the ideal loop theorem automatically holds in the actual physical electron configuration space.

The frozen baseline is preserved: ideal mapping-space results remain assumption-scoped, actual physical configuration space remains **OPEN**, and FR-odd $2\pi\to-1$ remains **CONDITIONAL**.

## 6. C02 quotient warning

**PASS.**

The chapter correctly notes that target quotient choices can alter the interpretation/topology of the standard spatial rotation loop. It does not generalize the ideal unquotiented result to all physical completions.

## 7. Footnote audit

**PASS.**

The notes for `loop`, `endpoint equality`, `triviality`, `closed path`, `basepoint`, `contractible`, and `time evolution` are concise and do not hide the scientific caveats.

## 8. Figure audit — F016

**PASS.**

F016 clearly shows a closed configuration-space path and states that endpoint equality does not determine contractibility. It also explicitly says it is not a diagram of a specific $2\pi$ rotation loop, a $\mathbb Z_2$ generator, or an FR verdict.

## 9. Final ruling

| Area | Verdict |
|---|---|
| Standard loop definition | **PASS** |
| Endpoint vs contractibility | **PASS** |
| Basepoint/homotopy preparation | **PASS** |
| Physical-time distinction | **PASS** |
| $2\pi$ / $\mathbb Z_2$ / FR boundaries | **PASS** |
| C02 quotient caveat | **PASS** |
| Footnotes | **PASS** |
| F016 | **PASS** |

### Overall

**PASS.**

Chapter 13 may now be drafted. Chapter 14 remains blocked until Chapter 13 receives an independent audit PASS.