# Chapter 5 Audit — 장(field)은 공간의 모든 점에 값을 붙인다

- **Audit target:** `volume-1/05-field.md` on `main`
- **Audit date:** 2026-08-29
- **Verdict:** **PASS — CHAPTER 6 DRAFT APPROVED**

## Scope

이번 감사는 제5장 canonical Markdown, F006/F1X03 실제 SVG asset, `STATUS.md`, `figures/registry.md`, frozen source ledger, 그리고 장에서 인용한 외부 표준 자료를 교차검토했다.

## Mathematical audit

**PASS.**

다음 핵심 개념이 정확히 분리되어 있다.

- field 전체와 한 점의 field value를 구분한다.
- scalar field를 `phi:M->R`의 형태로 설명한다.
- vector/direction field와 unit-vector field를 구분한다.
- `|n(x)|=1`은 길이 조건이며 모든 방향이 같다는 뜻이 아님을 명시한다.
- `n(x) in S^2`는 한 점에서의 값이고 `n`은 장 전체라는 구분을 유지한다.
- 일반적인 tangent vector field가 각 `T_xM`의 벡터를 고르는 section이라는 더 엄밀한 주의를 넣고, 이를 Planck-S² internal direction field와 자동 동일시하지 않는다.

초보자용으로 “field를 공간의 각 점을 입력으로 받아 값을 출력하는 함수”라고 먼저 설명하지만, 곧바로 tangent-bundle 예외/정밀화를 넣었기 때문에 과도한 일반화로 판정하지 않는다.

## Scientific / interpretation audit

**PASS.**

프로젝트 모델과 물리적 실재 주장을 분리한다.

- G02의 `n:S^2_domain -> S^2_internal`은 **CONDITIONAL · PROJECT MODEL CHOICE**로 취급한다.
- n-only baseline의 selection axiom은 조건부 분류정리의 가정으로 제한한다.
- 실제 전자에 physical n-field가 존재한다는 주장은 **OPEN**으로 유지한다.
- 전체 Planck-S²는 **WORKING HYPOTHESIS**로 유지한다.
- “구 위의 화살표”를 실제 전자 표면의 물질 바늘이나 관측된 내부구조로 묘사하지 않는다.

## Figure audit

### F006 — PASS

실제 asset `figures/volume-1/F006.svg`를 확인했다.

- scalar / vector-direction / unit-vector field의 세 패널이 구분되어 있다.
- unit-vector panel은 `|n(x)|=1`을 명시한다.
- 구는 domain의 예시일 뿐이며 실제 물질 표면이 아님을 asset 자체에도 명시한다.
- 본문에 `[이 그림에서 볼 것] / [이 그림이 뜻하는 것] / [이 그림이 뜻하지 않는 것]` 3단 경계가 존재한다.

### F1X03 — PASS

실제 asset `figures/volume-1/F1X03.svg`를 확인했다.

- 온도 지도는 scalar field, 바람 지도는 direction/vector field의 교육용 비교로 적절하다.
- 실제 기상자료가 아님을 표시한다.
- unit-vector field에서는 길이를 1로 고정해 방향만 남길 수 있다는 경계를 명시한다.
- 본문에 3단 그림 해석 경계가 존재한다.

## External source audit

**SOURCE VERIFIED.**

- OpenStax *Calculus Volume 3* §6.1은 vector field를 각 점에 벡터를 배정하는 구조로 설명하고, unit vector field를 각 벡터의 magnitude가 1인 field로 정의한다.
- MIT OCW *Calculus*, Chapter 15는 2D/3D vector field를 각 점에 벡터를 배정하는 것으로 정의한다.
- MIT OCW *An Introduction to Vector Calculus*는 위치에 따라 달라지는 temperature를 scalar quantity/function의 예로 사용한다.

이 외부 source들은 표준 field 언어만 뒷받침하며 Planck-S²의 물리 가설을 검증하는 증거로 확대되지 않았다.

## Educational audit

**PASS.**

4장 function/map에서 5장 field로 이어지는 의존관계가 자연스럽다. 날씨 지도 비유 뒤에 비유의 한계를 명시하고, 한 점의 값과 장 전체를 반복해서 분리하며, 다음 6장의 domain/target 두 S² 구분으로 연결한다.

## Minor notes

- F006의 구형 domain 위 화살표는 일반 독자가 tangent vector field로 오해할 수 있으나, 본문이 tangent field와 internal direction field의 차이를 명시하므로 blocker가 아니다.
- `direction field`라는 표현은 문맥에 따라 여러 뜻으로 쓰일 수 있으므로 이 책에서는 현재처럼 “방향 정보를 배정하는 직관적 표현”으로 제한하는 것이 적절하다.

## Final status

**PASS.**

- Chapter 5: `DRAFT COMPLETE / PASS`
- Previous audit state `AUDIT PENDING`: **CLOSED**
- Chapter 6 draft: **APPROVED**

제6장 제작 시에도 `domain S^2`와 `target/internal S^2`를 역할상 명확히 분리하고, 두 구가 실제 공간에 두 물체로 존재한다는 식의 해석을 금지한다.
