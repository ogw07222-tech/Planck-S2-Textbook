> **STATUS: DRAFT COMPLETE · AUDIT PENDING**
>
> 작성 Chat은 PASS를 부여하지 않는다. deck transformation의 표준 topology와 wavefunction sign choice를 분리한다.

# 9장 · cover의 두 층을 잇는 규칙 — deck transformation

## 현재 상태
- **작성 상태:** DRAFT COMPLETE
- **감사 상태:** AUDIT PENDING
- **핵심 경계:** $\mathbb Z_2$ deck topology $\neq$ quantum phase $-1$.

---

## 이번 장의 질문
1. cover를 base에 그대로 내려보내면서 cover 위의 점들을 바꾸는 symmetry는 무엇일까?
2. deck transformation[^v2c09-deck]이란 무엇인가?
3. $\mathbb Z_2$ cover에서는 왜 identity와 nontrivial transformation 두 개가 나타날까?
4. nontrivial base loop를 lift했을 때 endpoint는 deck transformation과 어떻게 연결될까?
5. 왜 이 단계에서도 wavefunction sign은 아직 정해지지 않을까?

---

## 앞 장 복습

universal cover

$$
p:\widetilde X\to X
$$

에서 base loop를 lift하면

$$
\widetilde\gamma(0)=\tilde x,
\qquad
\widetilde\gamma(1)=\tilde x'
$$

처럼 서로 다른 cover point에 도착할 수 있었다.

그런데 $\tilde x$와 $\tilde x'$는 base에서는 같은 점으로 projection될 수 있다.

이 둘을 서로 바꾸는 cover symmetry가 핵심이다.

---

## 먼저 생각해 보기 · 같은 건물의 두 복사본

완전히 같은 구조의 두 층 A와 B가 있고, 각 방이 아래 지도에서는 같은 방 번호로 표시된다고 상상하자.

A층 101호와 B층 101호를 서로 교환해도 지도에 표시되는 위치는 여전히 ‘101호’다.

이처럼 cover 위에서는 점을 바꾸지만 base projection은 바꾸지 않는 변환을 생각할 수 있다.

### 비유의 한계

실제 cover가 물리적으로 두 건물 층이라는 뜻은 아니다. 특히 Planck-S²에서 cover sheet를 실제 internal space의 물질 층으로 해석하면 안 된다.

---

## deck transformation의 정의

covering map $p:\widetilde X\to X$가 있을 때 cover 위의 homeomorphism[^v2c09-homeomorphism]

$$
g:\widetilde X\to\widetilde X
$$

가

$$
p\circ g=p
$$

를 만족하면 $g$를 deck transformation이라고 부른다.

즉 cover 위에서는 점을 옮기지만 base에서 보면 같은 점에 내려간다.

---

## Z₂ deck group

fundamental group이 $\mathbb Z_2$이고 universal cover가 regular하게 대응하는 전형적 상황에서는 deck group도

$$
\{e,g\}\cong\mathbb Z_2
$$

처럼 두 원소를 가진다.

- $e$: 아무것도 바꾸지 않는 identity deck transformation
- $g$: 두 lift endpoint를 교환하는 nontrivial transformation

그리고

$$
g^2=e.
$$

한 번 sheet를 바꾸고 다시 한 번 바꾸면 원래로 돌아온다는 구조다.

---

## loop lifting과 endpoint

nontrivial base loop $\gamma$를 $\tilde x$에서 lift했다고 하자.

그 endpoint가

$$
\widetilde\gamma(1)=g\tilde x
$$

로 갈 수 있다.

같은 nontrivial loop class를 한 번 더 이어붙이면 두 번째 lift가

$$
g\tilde x\to g^2\tilde x=\tilde x
$$

로 돌아온다.

이것이 $\mathbb Z_2$ topology를 cover endpoint로 읽는 방법이다.

---

## 왜 아직 −1이 아닌가

여기까지 얻은 것은

$$
\tilde x\longrightarrow g\tilde x
$$

이라는 **point transformation**이다.

하지만 quantum wavefunction $\Psi$가 있을 때

$$
\Psi(g\tilde x)
$$

가 $\Psi(\tilde x)$와 어떤 관계를 가져야 하는지는 아직 정하지 않았다.

가능한 규칙 중에는

$$
\Psi(g\tilde x)=+\Psi(\tilde x)
$$

도 있고

$$
\Psi(g\tilde x)=-\Psi(\tilde x)
$$

도 있을 수 있다.

이 규칙을 정리하는 것이 다음 장의 **character/representation**이다.

---

## topology와 quantum rule을 분리하기

표로 구분하자.

| 층 | 질문 |
|---|---|
| topology | nontrivial loop가 cover endpoint를 어떻게 바꾸는가? |
| deck group | endpoint 교환 transformation은 어떤 group을 이루는가? |
| quantum character | 그 transformation 아래 wavefunction이 어떻게 변하는가? |

따라서

> $\mathbb Z_2$ deck group 존재
>
> $\neq$
>
> wavefunction sign $-1$ 선택

이다.

---

## Planck-S²에서는

G04의 FR construction은 ideal configuration-space topology 위에서 cover와 character를 사용한다.

A01의 감사도 $\pi_1=\mathbb Z_2$에서 1-dimensional unitary character 두 개가 가능하다는 수학 구조를 assumption 범위에서 생존시킨다.

하지만 실제 physical configuration space와 cover/lift가 올바르게 정의됐는지는 physical bridge에 속한다.

C02는 quotient branch에서 standard loop 자체가 사라질 수 있음을 보여 주므로, deck transformation language를 physical electron에 적용하려면 먼저 어느 branch가 맞는지 정해야 한다.

---

## 현재 판정

| 주장 | 상태 | 범위 |
|---|---|---|
| deck transformation 표준 정의 | **SOURCE VERIFIED** | covering-space theory |
| $\mathbb Z_2$ cover에서 $g^2=e$ | **SOURCE VERIFIED** | standard group/cover structure |
| topology가 $-1$ phase를 자동 선택 | **FALSIFIED AS AN INFERENCE** | 추가 character 필요 |
| Planck-S² FR-odd physical choice | **CONDITIONAL** | G04/A01/C02 범위 |
| actual physical configuration space | **OPEN** | canonical ledger |

---

## 자주 하는 오해

> **“sheet가 두 개니 wavefunction은 ± 두 상태다.”**

아니다. sheet count와 quantum-state dimension은 별개다.

> **“nontrivial deck transformation은 이름부터 −1이다.”**

아니다. $g$는 cover point를 바꾸는 transformation이고, $\Psi$에 어떤 수를 곱할지는 representation을 통해 정한다.

---

## 다음 장이 필요한 이유

이제 정확한 질문을 할 수 있다.

> $g$가 wavefunction에 작용할 때 $+1$을 줄 것인가, $-1$을 줄 것인가?

이 규칙을 **FR character**로 정리한다.

---

## 한 문장 기억

> **deck transformation은 cover endpoint를 바꾸는 topology의 symmetry이고, 그 아래 wavefunction에 +1/−1을 붙이는 것은 다음 단계의 character 선택이다.**

---

## 확인문제
1. deck transformation의 핵심 식은?
2. $g^2=e$는 무엇을 뜻하는가?
3. 왜 $g$ 자체를 $-1$ phase라고 부르면 안 되는가?

## 정답
1. $p\circ g=p$.
2. nontrivial sheet exchange를 두 번 하면 identity가 된다는 뜻.
3. $g$는 공간의 transformation이고 $-1$은 wavefunction representation에서 나오는 수이기 때문이다.

---

## 근거 자료
- Allen Hatcher, *Algebraic Topology*, covering transformations/deck transformations — **SOURCE VERIFIED**.
- **G04**: cover/deck language와 FR sector.
- **A01/C02**: physical application scope.

[^v2c09-deck]: covering space를 자기 자신으로 바꾸면서 base projection은 그대로 유지하는 symmetry transformation.
[^v2c09-homeomorphism]: 공간을 찢거나 붙이지 않고 연속적으로 일대일 대응시키며 역변환도 연속인 map.
