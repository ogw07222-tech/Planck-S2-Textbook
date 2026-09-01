# Volume 2 Chapter 1 Independent Audit

- Canonical chapter: `volume-2/01-so3-physical-rotation.md`
- Primary figure: `figures/volume-2/F2X01.svg`
- Audit scope: mathematics, physics, proof-status boundaries, sources, pedagogy, SVG geometry, rendered visual QA
- Verdict: **REVISE — SCIENTIFIC CONTENT PASS, F2X01 VISUAL/SEMANTIC BLOCKER**

## 1. Executive verdict

제1장 본문의 표준 SO(3) 수학, Planck-S²의 proof-status 경계, Gate C 경계, FR/spin-1/2 비승격 규칙은 독립 감사에서 살아남았다.

차단 사유는 본문이 아니라 **F2X01의 시각 표현**이다. 이 장의 핵심 교육 명제가 `endpoint equality ≠ path contractibility`인데, 현재 그림의 가운데 패널에서 “360° 회전”을 나타내는 파란 경로가 열린 말굽형 곡선이며 방향 화살표도 없다. 독자는 이것을 완전한 360° 회전이 아니라 일부 각도 회전으로 읽을 수 있다. 오른쪽의 닫힌 loop는 실제로 닫혀 있으나 cubic Bézier 접합부가 뾰족하여 오른쪽 끝에 눈에 띄는 cusp가 생긴다. 위상적으로 loop에 smoothness가 필수는 아니지만, 이 장에서 cusp/특수점은 설명 대상이 아니므로 그림이 불필요한 구조를 암시한다.

따라서 **본문은 과학·수학상 PASS 수준이지만, 그림 수정 전 장 전체 PASS는 보류한다.**

---

## 2. Mathematics audit

### PASS — SO(3) definition

본문의

`SO(3)={R∈R^{3×3}: R^T R=I, det R=1}`

정의와 “3차원 orientation-preserving proper rotations” 설명은 표준 정의와 일치한다.

### PASS — path vs endpoint

`R_z(0)=R_z(2π)=I`에서 fixed-axis 2π path가 SO(3)의 loop가 된다는 설명은 정확하다.

또한 다음 구분도 정확하다.

- endpoint equality: `R(2π)=R(0)`
- loop triviality: `[γ_{2π}]=e`

두 명제는 동치가 아니다.

### PASS — π1(SO(3))

표준 결과

`π1(SO(3)) ≅ Z2`

와 이에 따른

- 360° fixed-axis loop: noncontractible
- 같은 loop의 double traversal인 720° loop: contractible

설명은 외부 표준 source와 일치한다.

### PASS — same π1 does not imply same space

`SO(3)`와 `Map_1(S²,S²)`가 모두 Z2 fundamental group을 가질 수 있어도 두 공간 자체를 동일시할 수 없다는 설명은 정확하다.

### MINOR PRECISION NOTE — orientation language

“SO(3)의 한 점 = 특정 3차원 orientation/rotation 상태”는 기준 frame에 대한 rigid rotation이라는 문맥에서는 적절하다. 다만 물체 자체가 비자명한 회전 대칭을 가지면 physically distinguishable orientation space는 `SO(3)/H` 꼴이 될 수 있다. 이 장은 화살표가 있는 비대칭 상자를 예로 들고 있고 이후 quotient 경고도 있으므로 현재 문장은 오답은 아니다. 재작성 필수 사항은 아니다.

---

## 3. Physics / Planck-S² boundary audit

### PASS — three-layer separation

본문은 다음 세 층을 명확히 분리한다.

1. standard rotation group `SO(3)`
2. ideal/smooth/unquotiented `Map_1(S²,S²)`
3. actual physical electron configuration space

이 구분은 canonical proof ledger와 일치한다.

### PASS — ideal mapping-space claims

다음 두 주장은 정확히 assumption-scoped로 유지된다.

- `π1(Map_1(S²,S²)) ≅ Z2`: **PROVED UNDER ASSUMPTIONS**
- smooth unquotiented `Map_1`에서 standard spatial 2π rotation loop가 Z2 generator: **PROVED UNDER ASSUMPTIONS**

### PASS — physical identification remains OPEN

`actual physical configuration space = ideal/unquotiented Map_1`을 **OPEN**으로 유지한다.

### PASS — Gate C

current unreduced n-only CP¹ branch의 constant target SO(3) global Noether symmetry라는 좁은 model-level statement와, project-level Gate C overall **OPEN**을 혼동하지 않는다.

### PASS — no premature FR/spin claim

본문은 다음을 정확히 유지한다.

- FR-odd `2π→−1`: **CONDITIONAL**
- half-integer sector: **CONDITIONAL**
- complete spin-1/2 / `j=1/2` ground: **OPEN**
- whole Planck-S²: **WORKING HYPOTHESIS**

`Z2 ≠ -1 phase itself` 경고도 적절하다.

---

## 4. Source audit

### PASS — MathWorld cross-check

MathWorld의 Rotation Group / Special Orthogonal Group 자료는 orthogonal matrix + determinant 1 정의와 SO(3)가 3차원 rotation group이라는 설명을 지지한다.

### PASS — John Baez Lecture 5 cross-check

John Baez, *Lie Theory Through Examples*, Lecture 5는 명시적으로

- `π1(SO(3)) = Z/2Z`
- 한 번의 360° loop는 noncontractible
- 두 번, 즉 720° traversal은 contractible

이라는 설명을 제공한다.

따라서 이 장의 standard SO(3) SOURCE VERIFIED 표시는 독립 외부 교차검증을 통과한다.

### PASS — project proof ledger

`G03/A01/C02`에서 가져온 mapping-space generator, physical Map₁ OPEN, Gate C OPEN, FR conditional 경계는 현재 `sources/proof-status.md`와 일치한다.

---

## 5. Pedagogy audit

### PASS

제1권의 path → loop → homotopy → π1 → Z2를 짧게 복습한 뒤 SO(3)로 이동하는 순서는 자연스럽다.

“사진 한 장 vs 동영상 전체”, belt/plate trick 비유도 각각의 한계를 바로 명시하고 있어 비유가 proof를 대체하지 않는다.

### PASS — misconception control

특히 다음 오해를 명시적으로 차단한다.

- 360° 뒤 모습 동일 ⇒ path trivial
- SO(3) 360° nontrivial ⇒ 모든 physical configuration space에서 nontrivial
- Z2 ⇒ 자동 -1 phase
- Map₁ generator theorem ⇒ actual electron theorem
- target SO(3) ⇒ external spatial SO(3)

---

## 6. F2X01 SVG geometry audit

### PASS — exact straightness / alignment

SVG 원문 좌표를 검사했다.

- 왼쪽 vertical axis: `(235,190) → (235,385)` — **정확한 직선**
- 가운데 vertical axis: `(640,190) → (640,385)` — **정확한 직선**
- 왼쪽 orientation arrow shaft: `(235,285) → (325,285)` — **정확한 수평선**
- 가운데 orientation arrow shaft: `(640,285) → (730,285)` — **정확한 수평선**
- 두 orientation 도형의 세로축 길이와 화살표 길이는 동일하다.
- 세 panel의 중심 x좌표는 `235, 640, 1045`이고 간격은 각각 `405 px`로 동일하다.
- 세 panel 크기는 모두 `360×420 px`로 동일하다.
- basepoint dot `(930,300)`은 purple loop의 시작/끝 좌표와 정확히 일치한다.
- 텍스트가 panel 경계 밖으로 잘리거나 겹치는 현상은 1280×760 및 2× 렌더에서 발견되지 않았다.

즉 사용자가 요청한 “직선이어야 하는데 미세하게 굽은 선” 문제는 axis/arrow에서는 발견되지 않았다.

### REVISE BLOCKER A — 360° indicator is visually open and directionless

가운데 파란 path:

`M545,320 C515,220 560,170 640,170 C720,170 765,220 735,320`

은 시작 `(545,320)`과 끝 `(735,320)`이 다른 **open cubic Bézier curve**다.

또 `marker-end`가 없어 회전 방향도 표시되지 않는다.

본문과 캡션은 “360° 회전 후”를 설명하지만 시각적으로는 완전한 한 바퀴가 아니라 약 3/4 원형의 열린 아치처럼 보인다.

이 그림은 핵심 개념의 첫 시각화이므로 단순 장식 문제가 아니다.

#### Required fix

가운데 panel은 다음 중 하나로 바꾼다.

- full circular/elliptic rotation arrow + arrowhead를 사용하여 실제 “한 바퀴”를 명확히 표시, 또는
- 현재 열린 arc를 유지하려면 “회전 방향 schematic”이라고 명시하고 360° 완료를 별도의 full-turn symbol로 표시.

첫 번째가 교육적으로 더 명확하다.

### REVISE BLOCKER B — closed loop has unintended cusps

오른쪽 purple loop:

`M930,300 C960,205 1130,205 1160,300 C1130,395 960,395 930,300 Z`

은 위상적으로는 닫혀 있으나 `(1160,300)`에서 두 cubic segment의 tangent가 불연속이어서 **눈에 띄는 오른쪽 cusp**가 생긴다. 시작/종료점 `(930,300)`에서도 tangent가 매끄럽게 이어지지 않지만 basepoint dot가 이를 가리고 있다.

loop의 continuous-ness만 필요하므로 수학적으로 거짓 그림은 아니다. 그러나 이 장은 singular point나 piecewise-smooth loop를 가르치는 장이 아니므로, 뾰족한 점이 특별한 topology를 뜻하는 것처럼 보일 이유가 없다.

#### Required fix

가장 단순한 수정은 purple path를

`<ellipse cx="1045" cy="300" rx="115" ry="72" .../>`

같은 smooth closed curve로 바꾸고 왼쪽 basepoint dot를 그대로 올리는 것이다.

또는 cubic Bézier control points를 조정해 join에서 C1 tangent continuity를 맞춘다.

### OPTIONAL MINOR IMPROVEMENT — traversal direction

오른쪽 loop에 작은 arrowhead 하나를 추가하면 “path를 따라 한 번 돈다”는 의미가 더 명확하다. contractibility 자체에는 orientation이 필수는 아니므로 blocker는 아니다.

---

## 7. Workflow consistency note

장 끝 production record의

`DO NOT START: Volume 2 Chapter 2 before Chapter 1 independent audit PASS`

문구는 현재 저장소 상태와 맞지 않는다. 사용자의 후속 지시로 제2권 전체 초안이 이미 작성되었기 때문이다.

이것은 과학적 오류가 아니라 stale workflow text다. 다음 안전한 편집 때

- “Chapter 2 production” blocker를 삭제하고
- “Chapter 2 independent audit before Chapter 1 PASS” 또는 현재 1장씩 감사 정책에 맞는 문구

로 정리하는 것이 좋다.

---

## 8. Required revision checklist

1. F2X01 가운데 360° 표시를 full-turn circular arrow로 교체하거나 동일 수준으로 명료화.
2. F2X01 오른쪽 closed loop의 cusp 제거; smooth ellipse/curve 권장.
3. 수정 SVG를 실제 렌더하여 1× 및 확대 렌더에서 다시 검사.
4. 본문 과학 내용과 proof-status는 현재 그대로 유지.
5. stale Chapter-2 production blocker 문구는 기회가 될 때 정리.

---

## 9. Final verdict

**REVISE — SCIENTIFIC CONTENT PASS, F2X01 VISUAL/SEMANTIC BLOCKER**

본문 자체에서는 현재 차단할 수학·물리·source/proof-status 오류를 찾지 못했다.

그러나 제2권은 회전 topology를 그림으로 배우는 권이고, F2X01은 첫 핵심 시각 자료다. 360° indicator의 열린 모양과 closed-loop cusp를 그대로 PASS하면 이후 그림 감사 기준과 충돌한다.

**Chapter 1 re-audit required after F2X01 revision. Chapter 2 independent audit should wait until Chapter 1 PASS.**
