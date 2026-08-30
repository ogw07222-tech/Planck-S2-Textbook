# Volume 2 — 360° 회전에서 FR 양자화까지

구성공간의 비자명 loop를 실제 3차원 회전, universal cover, deck transformation, Finkelstein–Rubinstein(FR) character, SU(2) representation으로 연결한다. 단, **half-integer sector 가능성**과 **complete spin-1/2 / j=1/2 ground / electron identity**를 끝까지 분리한다.

제1권 final independent audit가 PASS되어 Volume 2 DRAFT production이 승인되었다. 각 장의 scientific PASS는 계속 독립 감사에서만 부여한다.

현재 진행상태는 오직 [`../STATUS.md`](../STATUS.md)를 기준으로 한다. 이 README는 목차와 범위만 관리하며 live PASS 상태를 중복 기록하지 않는다.

## 확정 목차

| File | Unit |
|---|---|
| `01-so3-physical-rotation.md` | 제1장 · SO(3)과 물리적 회전 — 왜 360°가 단순해 보이지만 위상적으로는 문제가 생기는가 |
| `02-so3-three-axis.md` | 제2장 · 세 축으로 돌린다는 것 — 3차원 회전과 SO(3) |
| `03-360-720.md` | 제3장 · 360°와 720° — 같은 끝점, 다른 회전 경로 |
| `04-spatial-action.md` | 제4장 · 회전은 장을 어떻게 바꾸는가 — spatial action과 precomposition |
| `05-rotation-loop.md` | 제5장 · 회전 orbit는 왜 loop가 되는가 — configuration space 안의 2π 경로 |
| `06-evaluation-fibration.md` | 제6장 · evaluation fibration — mapping space의 topology를 읽는 계단 |
| `07-generator-proof-repair.md` | 제7장 · generator를 정말 찾았는가 — G03의 논리 빈틈과 A01의 수리 |
| `08-universal-cover.md` | 제8장 · loop를 펼쳐 올리기 — universal cover |
| `09-deck-transformation.md` | 제9장 · cover의 두 층을 잇는 규칙 — deck transformation |
| `10-fr-character.md` | 제10장 · FR character — 위상적 loop에 +1/-1 규칙을 붙이는 법 |
| `11-2pi-minus-one.md` | 제11장 · 2π→−1, 4π→+1 — 정확히 무엇이 조건부로 따라오는가 |
| `12-so3-su2.md` | 제12장 · SO(3)와 SU(2) — 왜 double cover가 나타나는가 |
| `13-half-integer-sector.md` | 제13장 · half-integer representation — j=1/2, 3/2, 5/2, ... |
| `14-not-yet-spin-half.md` | 제14장 · 왜 아직 spin-1/2 증명이 아닌가 — sector, j=1/2, ground state의 차이 |
| `15-gate-c-fork.md` | 제15장 · Gate C의 갈림길 — unquotiented space와 quotient space |
| `16-closing.md` | Closing · 제2권 마무리 — topology에서 양자 상태 공간으로, 그리고 제3권으로 |

## Canonical scientific boundary

- standard SO(3)/SU(2), covering-space, representation-theory 사실은 외부 표준 source와 구분해 **SOURCE VERIFIED**로 사용한다.
- ideal smooth/unquotiented $\pi_1(\mathrm{Map}_1(S^2,S^2))\cong\mathbb Z_2$: **PROVED UNDER ASSUMPTIONS**.
- 같은 ideal smooth/unquotiented setting의 $2\pi$ spatial-rotation loop가 $\mathbb Z_2$ generator: **PROVED UNDER ASSUMPTIONS**.
- actual physical configuration space $=$ ideal/unquotiented $\mathrm{Map}_1$: **OPEN**.
- Gate C overall: **OPEN**.
- FR-odd $2\pi\to-1$, $4\pi\to+1$: **CONDITIONAL**.
- half-integer rotation sector: **CONDITIONAL**.
- complete spin-1/2 / $j=1/2$ ground: **OPEN**.
- $Q=1=1$ bit: **FALSIFIED AS WRITTEN**.
- $Q=1=$ charge $-e$: **OPEN**.
- 전체 Planck-S²: **WORKING HYPOTHESIS**.

## Primary project sources

제2권의 frozen production baseline에서 핵심 project sources는 G03, G04, A01, C01, C02다. 현재 판정에서는 후속 적대적 감사 A01/C02를 우선하며, C_LIFT 등 frozen baseline 이후 자료는 자동 소급 병합하지 않는다.
