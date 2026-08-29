# Chapter 13 Audit — 고무줄처럼 줄일 수 있는가: homotopy

- **Audit date:** 2026-08-29
- **Canonical file:** `volume-1/13-homotopy.md`
- **Verdict:** **PASS — CHAPTER 14 DEPENDENCY ACCEPTED**

## 1. 표준 수학 감사

**PASS.**

- path와 homotopy를 서로 다른 층의 map으로 구분한다.
- `H:[0,1]×[0,1]→X`에서 `t`는 각 path 위의 parameter, `s`는 path 자체의 변형 parameter로 설명한다.
- based-loop homotopy에서 `H(s,0)=H(s,1)=x₀`를 유지하는 조건을 fundamental group 준비와 연결한다.
- constant loop, contractible, noncontractible, homotopy class의 역할이 표준 위상수학과 일치한다.
- `endpoint equality ≠ contractibility` 경계를 유지한다.

Allen Hatcher의 *Algebraic Topology* Chapter 1의 path homotopy / fundamental-group 준비와 양립한다.

## 2. 교육·비유 감사

**PASS.**

고무줄/기둥 비유는 contractibility 직관을 제공하지만, 실제 Planck-S² configuration space에 물리적 기둥이나 장애물이 존재한다는 뜻이 아니라고 본문과 그림에서 모두 제한한다.

## 3. Planck-S² 경계 감사

**PASS.**

- ideal `Map₁(S²,S²)` 안의 homotopy 질문과 actual physical configuration-space topology를 분리한다.
- physical space와 ideal Map₁의 동일성은 계속 **OPEN**이다.
- 특정 `2π` rotation loop의 nontriviality/generator 판정을 앞당기지 않는다.
- FR phase와 spin-1/2을 이 장에서 유도하지 않는다.
- 전체 Planck-S²는 **WORKING HYPOTHESIS** 경계를 유지한다.

## 4. Figure F017

**PASS.**

실제 asset이 존재하며, contractible/noncontractible 직관과 함께 `실제 Planck-S² configuration space 모양 아님`, `nontriviality는 공간 topology와 허용 homotopy 조건에 의존` 경계를 그림 내부에 직접 표시한다.

## 5. 각주 감사

**PASS.**

`homotopy`, `constant loop`, `contractible`, `noncontractible`, `based loop`에 장별 고유 footnote ID가 있으며 본문 정의를 보조하고 proof-status를 각주로 숨기지 않는다.

## 6. 비차단 메모

`contractible`은 이 장에서 fundamental-group 문맥에 맞춰 basepoint를 고정한 null-homotopy로 설명된다. 이후 자유 homotopy를 별도로 소개할 경우 두 문맥을 구분하면 된다. 현재 장에서는 문제가 없다.

## Final ruling

**PASS.** 과학적·수학적 blocker 없음.