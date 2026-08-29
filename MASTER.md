# Production MASTER

## 1. 프로젝트 목적

「Planck-S²를 처음부터 이해하는 책」은 Planck-S² Quantum Particle Hypothesis를 옹호하는 홍보물이 아니라, **어떤 수학·물리 명제가 무엇을 지지하며 어디부터가 OPEN인지 추적하는 교육·감사 교과서 시리즈**다. archive integrity의 PASS는 물리 이론의 PASS와 동일하지 않다.

전체 Planck-S² 전자 가설의 현재 최상위 라벨은 **WORKING HYPOTHESIS**다.

## 2. 6권 전체 구성

| Volume | Title | Goal |
|---|---|---|
| 1 | 구 위의 화살표에서 위상수학까지 | 입자/차원/구면/함수/장에서 시작해 $S^2\to S^2$, degree, configuration space, path, loop, homotopy, $\pi_1$, $\mathbb Z_2$까지 연결 |
| 2 | 360° 회전에서 FR 양자화까지 | 회전 loop, generator, universal cover, FR character, half-integer sector의 조건부 연결 |
| 3 | Soliton, Moduli 그리고 양자 모양 | $Q=1$ soliton, moduli, zero mode, collective coordinate, rotor state counting |
| 4 | 작은 진동에서 Casimir 에너지까지 | Hessian, eigenmode, branch tracking, one-loop, regularization, heat kernel, renormalization |
| 5 | Planck-S² 적대적 감사 — Gate A에서 Gate H까지 | Gate A–H와 판정 강등·수리의 논리 추적 |
| 6 | 그래서 Planck-S²는 지금 어디까지 왔는가 | 현재 증명상태와 실제 전자 bridge, falsifiable prediction까지의 미해결 연결을 통합 |

현재 진행상태는 오직 [`STATUS.md`](STATUS.md)를 기준으로 한다.

## 3. Source freeze

교과서 제작 기준선은 **C02까지의 frozen production baseline**이다.

- C_LIFT 및 이후 새 연구 파일은 기존 기준선에 자동 소급 병합하지 않는다.
- 새 연구는 해당 권의 SCIENTIFIC/SOURCE AUDIT 단계에서 별도로 확인한다.
- 기존 판정을 실제로 바꾸는 경우에만 해당 장과 [`sources/proof-status.md`](sources/proof-status.md)를 갱신한다.

## 4. 증명상태 라벨

| Label | Editorial rule |
|---|---|
| PROVED | 명시 범위를 넘겨 확대하지 않는다. |
| PROVED UNDER ASSUMPTIONS | 같은 장/표에서 가정 목록과 범위를 추적한다. |
| SOURCE VERIFIED | 외부/표준 결과를 Planck-S²의 새 증명처럼 쓰지 않는다. |
| NUMERICALLY VERIFIED | solver/benchmark/재현 범위를 명시한다. |
| NUMERICALLY SUPPORTED | 일반 정리나 물리 예측으로 승격하지 않는다. |
| CONDITIONAL | 조건이 사라지면 주장도 사라짐을 명시한다. |
| PRELIMINARY | 예비 계산/출력 일관성의 범위를 밝힌다. |
| OPEN | 모른다고 직접 쓴다. |
| FALSIFIED AS WRITTEN | 과거 문장을 숨기지 않고 오류와 살아남은 부분을 함께 기록한다. |
| NOT YET AUDITED | 새 결과와 후속 적대적 감사 완료 여부를 분리한다. |

## 5. Source 우선순위

1. 사용자의 명시적 지시
2. 가장 최신 적대적 감사
3. 이전 적대적 감사
4. 가장 최신 일반 연구/검증 보고서
5. 이전 일반 연구보고서
6. 외부 선행문헌
7. 추론

상세 source inventory는 [`sources/source-index.md`](sources/source-index.md)에 둔다.

## 6. Gate A–H 현재 기준선

| Gate | Current status | Scope |
|---|---|---|
| A | OPEN | reference CP¹ operator의 일부 엄밀성과 별개로 final physical action/Hessian A10이 미확정 |
| B | OPEN | zero modes / collective coordinates / stabilizer / Gram determinant / Jacobian 미폐쇄 |
| C | OPEN | current n-only action의 target SO(3) model statement는 조건부 생존하지만 physical ontology/quotient/lift/3+1D matching이 미폐쇄 |
| D | OPEN | mode counting / multiplicity / branch continuation 미폐쇄 |
| E | OPEN | actual physical Hessian의 Laplace-type 여부 미확정 |
| F | OPEN | physical heat-kernel coefficients / counterterms 미확정 |
| G | OPEN | physical renormalization condition / finite $C_{ren}(\lambda)$ 미확정 |
| H | OPEN | independent cutoff/resolution/basis validation 미완성 |

## 7. 핵심 OPEN / 금지 승격

- actual physical configuration space = ideal/unquotiented $\mathrm{Map}_1(S^2,S^2)$: **OPEN**
- $\pi_1(\mathrm{Map}_1(S^2,S^2))\cong\mathbb Z_2$: **PROVED UNDER ASSUMPTIONS**
- FR-odd $2\pi\to-1$: **CONDITIONAL**
- 완전한 spin-1/2 / $j=1/2$ ground: **OPEN**
- $Q=1=1$ bit: **FALSIFIED AS WRITTEN**
- $Q=1=$ charge $-e$: **OPEN**
- physical Gate A / A10 action & Hessian: **OPEN**
- physical $C_{ren}(\lambda)$ / final $H_2$ ground: **OPEN**
- external 3+1D Lorentz, Dirac, QED, Fermi statistics, mass, radius, form factor, g-factor, 독립적 falsifiable prediction: **OPEN**

상세 현재 proof ledger는 [`sources/proof-status.md`](sources/proof-status.md)를 기준으로 한다.

## 8. 교과서 작성 원칙

전문용어는 가능한 한 다음 순서를 따른다.

**왜 필요한가 → 직관 → 비유 → 그림 → 비유의 한계 → 실제 정의 → 최소 수학 → Planck-S² 적용 → 현재 증명상태 → 말할 수 있는 것 → 말할 수 없는 것 → 오해 방지 → 확인문제**

- 초보 독자를 위한 장문 교재의 설명 밀도를 유지한다.
- 오류를 발견해도 migration 단계에서 원문을 몰래 고치지 않는다. 원문은 보존하고 `TODO` 또는 audit note를 추가한다.
- 장별 canonical 파일은 하나만 둔다. `04-function-v2.md`, `final.md` 같은 파일을 만들지 않는다.
- 감사도 장별 canonical audit 파일 하나만 유지하고 Git history로 판정 변화를 보존한다.

## 9. 오해 방지 규칙

| Source statement | Forbidden equivalence |
|---|---|
| $Q=1$ | $\neq$ 1 bit |
| $Q=1$ | $\neq$ charge $-e$ |
| $2\pi\to-1$ 가능 | $\neq$ 완전한 spin-1/2 |
| half-integer sector | $\neq$ $j=1/2$ ground |
| CP¹ reference result | $\neq$ physical Planck-S² result |
| $H_0$ signal | $\neq$ $H_2$ ground state |
| Casimir minimum | $\neq$ quantum ground state |
| numerical convergence | $\neq$ renormalization |
| specific mode convergence | $\neq$ total mode sum convergence |
| archive integrity PASS | $\neq$ hypothesis PASS |

## 10. 전체 개념 의존관계

| Track | Dependency chain |
|---|---|
| A. 기초 언어 | 점/대상 → 차원 → 원·구면 → $S^1/S^2$ → 함수 → domain/target → field → $S^2\to S^2$ |
| B. 위상 언어 | degree $Q$ → configuration → configuration space → path → loop → homotopy → $\pi_1$ → $\mathbb Z_2$ |
| C. 회전/양자화 | SO(3) → 2π/4π rotation path → generator proof → universal cover → deck transformation → FR character → SU(2) double cover → half-integer representation |
| D. 동역학/모양 | energy → action → CP¹ → $Q=1$ soliton → Möbius moduli → $\lambda/\mu$ → zero mode → collective coordinate → rotor state counting |
| E. moduli 양자화 | $L^2$ metric → moduli metric → Laplace–Beltrami → $H_0$ → self-adjoint domain/FR line bundle → $H_1/H_2$ |
| F. fluctuation/one-loop | fluctuation → Hessian → eigenmode → zero-point energy → Casimir → branch identity → regularization → heat kernel → counterterms → renormalization |
| G. EFT/검증 | derivative expansion → power counting → A10.11f → Gate A–H → physical $C_{ren}$ → $H_2$ eigenproblem → ground state |
| H. 실제 전자 bridge | physical completion → external 3+1D rotations/Lorentz → charge $-e$/U(1) → Dirac/QED → exchange/Fermi statistics → observables → falsifiable prediction |

## 11. 권별 목표

각 권의 상세 목표와 chapter outline은 해당 `volume-*/README.md` 및 장별 Markdown에서 관리한다. 현재 진행상태 문자열은 여기에서 중복하지 않는다.

## 12. 그림 registry

그림의 존재/감사/asset 상태는 오직 [`figures/registry.md`](figures/registry.md)에서 관리한다. 실제 존재를 확인하지 않은 그림은 `CREATED`로 올리지 않는다.

## 13. 현재 작업 규칙

- Markdown = 연구/교과서 작업 원본
- Git = 버전관리
- DOCX/PDF = 배포·출판 산출물
- 현재 상태 = `STATUS.md` 한 곳에서만 관리
- source status = `sources/proof-status.md`
- figure status = `figures/registry.md`
- 제4장 실제 본문과 F005/F1X02가 복구·감사되기 전에는 **제5장 본문을 시작하지 않는다.**
