# Chapter 14 Audit — 기본군을 “loop의 종류표”로 이해하기

- **Audit date:** 2026-08-29
- **Canonical file:** `volume-1/14-fundamental-group.md`
- **Verdict:** **PASS — CHAPTER 15 DEPENDENCY ACCEPTED**

## 1. 표준 수학 감사

**PASS.**

- based loop와 basepoint를 정확히 구분한다.
- `[γ]`를 raw loop 하나가 아니라 based-loop homotopy class로 설명한다.
- concatenation을 piecewise formula로 제시한다.
- constant-loop class를 identity, reverse-loop class를 inverse로 설명한다.
- raw path concatenation의 괄호 방식은 함수 수준에서 엄밀히 동일하지 않을 수 있으나 homotopy class에서 associativity가 성립한다는 정밀성 경계를 둔다.
- `π₁(X,x₀)`를 based-loop homotopy classes + concatenation의 group으로 정의한다.
- `π₁ = loop의 개수`라는 오해를 명시적으로 차단한다.

Allen Hatcher의 *Algebraic Topology* Chapter 1의 fundamental-group 정의와 일치한다.

## 2. Basepoint 정밀성 감사

**PASS.**

path-connected 공간에서 서로 다른 basepoint의 fundamental group들이 연결 path 선택을 통해 isomorphic하다는 점과, 그 구체적 identification이 일반적으로 선택에 의존한다는 주의를 각주로 제공한다.

## 3. Planck-S² 경계 감사

**PASS.**

- 이 장은 `π₁(Map₁)=Z₂`를 새로 증명하지 않고 제15장으로 넘긴다.
- ideal mapping space와 actual physical configuration space를 구분한다.
- quotient/completion에 따라 fundamental group이 달라질 수 있다는 경계를 유지한다.
- FR phase 및 spin-1/2을 fundamental group 정의만으로 유도하지 않는다.

## 4. 각주 감사

**PASS.**

based loop, homotopy class, concatenation, group, fundamental group, basepoint, equivalence class, identity, inverse, associativity, path-connected, isomorphism 및 basepoint 정밀성 각주가 장별 ID로 정상 구성되어 있다.

## 5. 비차단 메모

본문은 `[γ][γ^{-1}]=[c]`를 대표식으로 쓴다. reverse loop가 양쪽 inverse라는 표준 사실까지 포함하는 것으로 읽을 수 있으며, 초급 설명 수준에서 blocker가 아니다.

## Final ruling

**PASS.** 제15장의 `Z₂` 결과를 읽기 위한 표준 수학 기반으로 적절하다.