# Chapter 7 Audit — 구를 몇 번 감았는가: degree Q

- **Audit date:** 2026-08-29
- **Canonical target:** `volume-1/07-degree-q.md`
- **Verdict:** **PASS — CHAPTER 8 DRAFT APPROVED**

## Scope

GitHub main의 제7장 본문, F009/F010/F011/F012/F1X04 실제 SVG asset, figure registry, canonical proof-status 경계를 독립 적대적으로 점검했다. 외부 표준 수학은 Allen Hatcher의 *Algebraic Topology* §2.2 degree/local degree 논의와 교차검증했다.

## Mathematical audit

**PASS.**

다음 핵심 내용이 표준 위상수학과 일치한다.

- 연속 map `f:S²→S²`에는 정수 degree를 붙일 수 있다.
- identity map의 degree는 `+1`이다.
- reflection의 degree는 `−1`이다.
- constant map은 degree `0`의 대표 예다.
- degree는 homotopy invariant이다.
- `S²→S²`의 homotopy class는 degree로 분류된다.
- 적절한 target point의 preimage에서 local degree를 합하면 global degree를 얻는다는 설명은 표준 local-degree 공식과 일치한다.
- degree `2`를 `+1 + +1` local contributions의 대표 그림으로 설명하는 방식은 적절한 교육적 단순화다.
- `n(x)` 한 점의 값과 `Q=deg(n)`이라는 전역적 정수를 명확히 분리했다.

본문의

`Q = (1/4π) ∫ n·(∂θ n × ∂φ n) dθ dφ`

형식은 표준 spherical parametrization과 orientation convention 아래의 pullback-area degree 공식으로 읽을 수 있다. 본문이 좌표 convention/orientation 의존성을 명시해 과도한 일반화를 피했다. 구면 극점의 좌표 특이성은 degree 자체의 특이성이 아니며, 이 장의 교육 수준에서는 blocker가 아니다.

## Scientific / interpretation audit

**PASS.**

프로젝트의 수학적 사실과 물리적 가설을 적절히 분리했다.

- standard degree theory: **SOURCE VERIFIED**
- Planck-S²에서 `Q=1` sector 선택: **CONDITIONAL · PROJECT MODEL CHOICE**
- `Q=1 = 1 bit`: **FALSIFIED AS WRITTEN**
- `Q=1 = electric charge −e`: **OPEN**
- 실제 전자가 physical `n`-field 및 `Q=1` sector를 가진다는 주장: **OPEN**
- actual physical configuration space = ideal mapping space: **OPEN**
- 전체 Planck-S²: **WORKING HYPOTHESIS**

`Q<0`을 음의 에너지/음전하/반입자로, `Q=2`를 두 입자나 2 bit로 자동 해석하는 비약도 명시적으로 차단했다.

## Figure audit

### F009 — Q=0
**PASS.** 상수 map을 degree-0의 대표 예로만 사용하고, 모든 Q=0 map이 상수라는 오해를 차단한다.

### F010 — Q=+1
**PASS.** orientation-preserving degree-one 대표 상황을 보여 주며 charge/bit/electron 동일시를 금지한다.

### F011 — Q=−1
**PASS.** orientation reversal의 부호 의미를 시각화하고 음의 에너지·전하·반입자 해석을 금지한다.

### F012 — Q=2
**PASS.** regular target point의 두 preimage와 `+1,+1` local contributions라는 local-degree 직관을 사용하며 실제 두 sheet/두 입자라는 해석을 차단한다.

### F1X04 — orientation
**PASS.** local orientation 보존/반전을 최소 직관으로 제시하며 정식 orientation 정의 전체를 그림이 대체하지 않는다고 제한한다.

모든 핵심 그림 본문에는 `[이 그림에서 볼 것] / [이 그림이 뜻하는 것] / [이 그림이 뜻하지 않는 것]` 경계가 있다.

## Educational audit

**PASS.**

제6장 `S²→S²` map 언어에서 제7장 전역 degree로 넘어가는 개념 의존관계가 자연스럽다. 특히 degree를 먼저 ‘몇 번 감김’ 비유로 소개한 뒤 orientation, local degree, homology 정의, 적분 표현으로 점진적으로 정밀화해 초보 독자용 구조를 유지한다.

## Non-blocking precision note

- spherical `(θ,φ)`는 구면 전체를 단일 regular chart로 덮지 못한다. 현재 적분식은 표준 spherical parametrization에서 좌표 특이점을 허용해 쓰는 공식으로 이해하면 된다. 이후 더 엄밀한 판에서는 ‘pullback of the target area form’ 표현을 한 줄 덧붙이면 더욱 정확해진다.

이 항목은 현재 본문의 수학적 결론을 바꾸지 않으므로 **PASS blocker가 아니다.**

## Final status

**PASS — Chapter 7 DRAFT COMPLETE. Chapter 8 DRAFT is approved.**

제8장에서는 `Q=1`이 말해 주는 것과 말해 주지 않는 것을 분리하되, 특히 `Q=1≠1 bit`, `Q=1≠charge −e`, `Q=1≠electron identity` 경계를 유지해야 한다.
