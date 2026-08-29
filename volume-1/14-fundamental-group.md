> **STATUS: DRAFT COMPLETE · AUDIT PENDING**
>
> VOLUME 1 FINAL BATCH DRAFT MODE에서 작성한 초안이다. 작성 Chat은 PASS를 부여하지 않는다. 이 장은 fundamental group의 표준 언어만 준비하며 Planck-S²의 특정 $\pi_1$ 값은 제15장에서 조건과 함께 다룬다.

# 14장 · 기본군을 “loop의 종류표”로 이해하기

## 현재 상태

- **작성 상태:** DRAFT COMPLETE
- **감사 상태:** AUDIT PENDING
- **선행 장 사용 방식:** 제13장 초안의 homotopy 언어를 사용하되, 표준 정의와 frozen baseline을 우선한다.
- **다음 배치 대상:** 제15장 DRAFT
- **핵심 경계:** $\pi_1$는 loop의 단순 개수가 아니라 based loop들의 homotopy class와 이어붙이기 연산으로 만든 group이다.

---

## 이번 장에서 알아낼 질문

1. based loop[^v1c14-based-loop]를 homotopy로 묶으면 어떤 “종류”가 남을까?
2. homotopy class[^v1c14-homotopy-class] $[\gamma]$는 무엇을 뜻할까?
3. 두 loop를 이어붙이는 concatenation[^v1c14-concatenation]은 어떻게 정의할까?
4. 왜 constant loop가 identity가 될까?
5. reverse loop가 왜 inverse 역할을 할까?
6. group[^v1c14-group]이라는 말은 최소한 어떤 규칙을 뜻할까?
7. fundamental group[^v1c14-fundamental-group] $\pi_1(X,x_0)$은 무엇인가?
8. 왜 $\pi_1$를 “loop의 개수”라고 부르면 틀릴까?
9. basepoint를 바꾸면 무엇이 달라질 수 있을까?

---

## 앞 장에서 배운 것

제13장에서는 두 loop를 끊지 않고 연속적으로 바꿀 수 있으면 같은 homotopy class로 묶을 수 있다는 언어를 배웠다.

또 based loop를 비교할 때는 변형 중에도 basepoint $x_0$를 유지했다.

이제 같은 class에 속하는 loop들을 한 종류로 묶어 보자.

예를 들어

$$
\gamma_1\simeq\gamma_2
$$

라면 두 loop의 정확한 그림은 다르더라도 같은 class로 본다.

그 class를

$$
[\gamma]
$$

라고 쓴다.

---

## 왜 새로운 문제가 생겼을까?

loop를 class로 묶는 것만으로도 공간의 topology를 많이 알 수 있다.

하지만 더 중요한 질문이 있다.

> loop A를 한 번 돈 뒤 loop B를 이어서 돌면 어떤 새로운 loop 종류가 되는가?

즉 loop 종류 사이에도 **연산**이 있다.

이 연산까지 함께 기록하면 단순한 목록보다 훨씬 강한 구조를 얻는다.

그 구조가 fundamental group이다.

---

## 먼저 생각해 보기 · 산책 경로 장부

집 $x_0$에서 출발해 다시 집으로 돌아오는 산책 경로들을 기록한다고 하자.

경로를 아주 조금 우회하거나 모서리를 둥글게 만든 정도는 같은 종류로 묶는다.

그리고 산책 A를 끝낸 뒤 곧바로 산책 B를 하면 “A 다음 B”라는 새 산책 경로가 생긴다.

장부에는 다음 두 가지를 함께 적을 수 있다.

1. 어떤 산책들이 같은 종류인가?
2. 두 종류를 연달아 하면 어떤 종류가 되는가?

fundamental group은 이와 비슷한 역할을 한다.

### 비유의 한계

일반적인 group에서는 순서가 중요할 수 있다.

$$
[\gamma_1][\gamma_2]
$$

와

$$
[\gamma_2][\gamma_1]
$$

가 항상 같은 것은 아니다.

따라서 fundamental group을 평범한 정수 덧셈과 항상 같은 구조라고 생각하면 안 된다.

---

## 실제 수학에서는 · based loop

공간 $X$의 한 점 $x_0$를 정하자.

based loop는

$$
\gamma:[0,1]\to X,
\qquad \gamma(0)=\gamma(1)=x_0
$$

인 loop다.

$x_0$가 basepoint[^v1c14-basepoint]다.

fundamental group에서는 이 basepoint를 공유하는 loop들을 비교한다.

---

## homotopy class [γ]

두 based loop가 basepoint를 유지하는 homotopy로 서로 바뀔 수 있으면 같은 class로 묶는다.

그 class를

$$
[\gamma]
$$

라고 쓴다.

중요한 점은 $[\gamma]$가 loop 그림 하나를 뜻하는 것이 아니라는 것이다.

> **서로 homotopic한 모든 based loop를 한꺼번에 묶은 equivalence class[^v1c14-equivalence-class]**

다.

---

## 두 loop를 이어붙이기 · concatenation

두 based loop $\gamma_1,\gamma_2$가 같은 $x_0$를 기준점으로 가진다고 하자.

먼저 $\gamma_1$을 돌고, 그 다음 $\gamma_2$를 돌면 하나의 새 loop를 만들 수 있다.

이를

$$
\gamma_1*\gamma_2
$$

처럼 쓴다.

parameter를 반씩 나누어 쓰면 개념적으로

$$
(\gamma_1*\gamma_2)(t)=
\begin{cases}
\gamma_1(2t), & 0\le t\le\frac12,\\
\gamma_2(2t-1), & \frac12\le t\le1
\end{cases}
$$

처럼 생각할 수 있다.

class에서는

$$
[\gamma_1]\,[\gamma_2]=[\gamma_1*\gamma_2]
$$

라고 쓴다.

---

## constant loop = identity

basepoint $x_0$에서 계속 머무는 constant loop를 $c$라고 하자.

$$
c(t)=x_0.
$$

어떤 loop $\gamma$ 앞이나 뒤에 $c$를 붙여도 homotopy class는 원래 $[\gamma]$와 같다.

따라서

$$
[c][\gamma]=[\gamma][c]=[\gamma]
$$

가 된다.

이런 역할을 하는 원소를 identity[^v1c14-identity]라고 부른다.

---

## reverse loop = inverse

loop $\gamma$를 반대 방향으로 따라가는 loop를

$$
\gamma^{-1}(t)=\gamma(1-t)
$$

처럼 쓸 수 있다.

$\gamma$를 갔다가 바로 반대로 돌아오면 전체 loop는 constant loop와 같은 class로 줄일 수 있다.

그래서

$$
[\gamma][\gamma^{-1}]=[c]
$$

이고, $[\gamma^{-1}]$는 $[\gamma]$의 inverse[^v1c14-inverse] 역할을 한다.

---

## associativity는 왜 class에서 말할까?

세 loop를 이어붙일 때

$$
(\gamma_1*\gamma_2)*\gamma_3
$$

와

$$
\gamma_1*(\gamma_2*\gamma_3)
$$

는 parameter를 나누는 방식이 달라 path 함수로서 완전히 같은 모양은 아닐 수 있다.

하지만 둘은 자연스럽게 reparameterization해서 서로 homotopic하다.

따라서 homotopy class에서는

$$
([\gamma_1][\gamma_2])[\gamma_3]
=
[\gamma_1]([\gamma_2][\gamma_3])
$$

가 성립한다.

이 성질을 associativity[^v1c14-associativity]라고 한다.

---

## group이라는 말의 최소 의미

어떤 원소들의 모음과 결합 규칙이 있고 다음 네 가지가 성립하면 group이라고 부른다.

1. 두 원소를 결합하면 다시 같은 종류의 원소가 나온다.
2. 결합 순서를 괄호로 묶는 방식에 대해 associativity가 성립한다.
3. 아무것도 바꾸지 않는 identity가 있다.
4. 각 원소에는 그것을 되돌리는 inverse가 있다.

fundamental group에서는

- 원소: based loop의 homotopy class
- 연산: loop concatenation
- identity: constant loop class
- inverse: reverse loop class

가 된다.

---

## fundamental group π₁(X,x₀)

이제 정의를 한 줄로 모을 수 있다.

$$
\pi_1(X,x_0)
=
\{\text{based loops at }x_0\}/\text{homotopy}
$$

라고 생각하고, 여기에 concatenation을 연산으로 둔다.

즉 $\pi_1(X,x_0)$는

> **기준점 $x_0$에서 출발해 돌아오는 loop들을 homotopy로 종류별로 묶고, 그 종류들을 이어붙이는 법까지 기록한 group**

이다.

---

## π₁는 loop의 개수가 아니다

이 장에서 가장 중요한 오해 방지다.

한 공간에는 실제 loop 함수가 무한히 많이 있을 수 있다.

하지만 그중 수많은 loop가 같은 homotopy class에 들어갈 수 있다.

따라서

> $\pi_1$의 원소 수 = 원래 loop 그림의 개수

가 아니다.

$\pi_1$가 분류하는 것은 **loop 자체 하나하나가 아니라 loop homotopy class**다.

---

## fundamental group은 무엇을 감지할까?

fundamental group은 공간 안에서 loop가 어떻게 걸릴 수 있는지를 통해 “구멍 구조”의 일부를 감지한다.

예를 들어 어떤 공간에서는 모든 loop가 constant loop로 줄어 하나의 class만 남을 수 있다.

다른 공간에서는 줄일 수 없는 loop class들이 남을 수 있다.

하지만 fundamental group이 공간의 모든 위상 정보를 완전히 기록하는 만능 도구는 아니다. 서로 다른 공간이 같은 fundamental group을 가질 수도 있다.

---

## basepoint를 바꾸면 어떻게 될까?

$\pi_1(X,x_0)$ 표기에 $x_0$가 들어가는 이유가 있다.

based loop는 어느 점을 기준으로 시작하고 끝나는지를 정하기 때문이다.

공간이 path-connected[^v1c14-path-connected]라면 서로 다른 basepoint를 잇는 path를 선택해서 fundamental group들 사이의 isomorphism[^v1c14-isomorphism]을 만들 수 있다.

하지만 그 identification은 일반적으로 선택한 연결 path에 의존할 수 있어 완전히 자동적인 하나의 동일시라고 생각하면 안 된다.[^v1c14-basepoint-precision]

---

## Planck-S²에서는

앞 장들의 ideal 후보 공간을

$$
\mathcal C_1=\mathrm{Map}_1(S^2,S^2)
$$

라고 썼다.

그렇다면 자연스럽게

$$
\pi_1(\mathcal C_1,n_0)
$$

를 물어볼 수 있다.

이 표현은 “degree-one mapping space에서 based loop들의 homotopy class group은 무엇인가?”라는 질문이다.

하지만 이 장에서는 그 답을 아직 넣지 않는다.

제15장에서 frozen baseline의 조건부 결과

$$
\pi_1(\mathrm{Map}_1(S^2,S^2))\cong\mathbb Z_2
$$

를 정확한 가정 범위와 함께 소개한다.

---

## 당시 연구에서는 무엇을 얻었나

G02/G03는 degree-one mapping space의 loop 구조를 조사하면서 fundamental group을 핵심 질문으로 끌어올렸다.

중요한 변화는

> “loop 하나가 어떻게 생겼나?”

에서

> “모든 loop 종류가 어떤 group 구조를 이루나?”

로 질문이 확장된 것이다.

---

## 후속 감사에서는 무엇이 바뀌었나

A01과 C02 이후에는 $\pi_1$ 값을 말할 때 **어느 공간의 fundamental group인지**를 반드시 명시한다.

ideal/unquotiented $\mathrm{Map}_1$의 수학 결과와 actual physical configuration space의 $\pi_1$는 같은 명제가 아니다.

특히 quotient나 completion이 달라지면 fundamental group도 달라질 수 있다.

따라서 제15장에서도 ideal result와 physical application을 분리한다.

---

## 현재 판정

| 주장/항목 | 상태 | 정확한 범위 |
|---|---|---|
| based loop / homotopy class / concatenation의 표준 정의 | **SOURCE VERIFIED** | 표준 위상수학 |
| loop homotopy classes가 concatenation으로 fundamental group을 이룸 | **SOURCE VERIFIED** | 표준 위상수학 |
| constant loop = identity, reverse loop = inverse | **SOURCE VERIFIED** | 표준 fundamental-group 구조 |
| $\pi_1$가 loop의 단순 개수가 아님 | **SOURCE VERIFIED** | class와 raw loop 구분 |
| actual physical Planck-S² configuration space의 $\pi_1$ | **OPEN** | physical-space 동일성 미확정 |
| 전체 Planck-S² | **WORKING HYPOTHESIS** | 전체 이론 미완성 |

> **AUDIT NOTE:** 제14장은 fundamental group의 정의만 세운다. $\pi_1(\mathrm{Map}_1)=\mathbb Z_2$의 프로젝트 적용 범위는 제15장 독립 감사에서 별도로 검증해야 한다.

---

## 이것으로 말할 수 있는 것

- fundamental group의 원소는 based loop 자체가 아니라 homotopy class다.
- loop concatenation이 group operation을 만든다.
- constant loop class는 identity다.
- reverse loop class는 inverse다.
- fundamental group은 공간의 loop obstruction을 감지하는 위상 도구다.

---

## 이것으로 말할 수 없는 것

- $\pi_1$를 loop의 총 개수라고 말할 수 없다.
- 모든 fundamental group이 숫자 덧셈처럼 commutative라고 말할 수 없다.
- ideal mapping space의 $\pi_1$를 actual electron configuration space에 자동 이식할 수 없다.
- fundamental group만으로 FR phase나 spin-1/2을 얻었다고 말할 수 없다.

---

## 자주 하는 오해

### 오해 1 · “π₁는 loop가 몇 개인지 세는 숫자다.”

아니다. $\pi_1$는 loop homotopy class들과 그 group operation이다.

### 오해 2 · “두 loop를 이어붙이는 것은 그냥 길이 더하기다.”

아니다. loop 함수 자체를 순서대로 따라가는 새로운 loop를 만드는 연산이다.

### 오해 3 · “identity loop는 특별한 큰 원이다.”

아니다. constant loop의 homotopy class다.

### 오해 4 · “inverse는 숫자에 마이너스를 붙이는 것이다.”

일반 fundamental group에서 inverse는 loop를 반대 방향으로 따라가는 class다.

### 오해 5 · “fundamental group을 알면 공간의 모든 것을 안다.”

아니다. 중요한 위상 불변량이지만 공간의 모든 정보를 담지는 않는다.

---

## 다음 장이 필요한 이유

이제 fundamental group이 무엇인지 알았다.

그러면 Planck-S²의 ideal degree-one mapping space에서 실제로 어떤 group이 나오는지 물을 수 있다.

frozen baseline의 핵심 결과는

$$
\mathbb Z_2
$$

다.

하지만 이 결과는 반드시 가정과 물리적 한계를 함께 읽어야 한다.

---

## 한 문장 기억

> **fundamental group은 based loop들을 homotopy 종류로 묶고 이어붙이기 연산을 준 group이지, loop의 단순 개수를 세는 숫자가 아니다.**

---

## 용어 카드

| 용어 | 이 장에서의 뜻 |
|---|---|
| based loop | 같은 basepoint에서 출발하고 돌아오는 loop |
| homotopy class $[\gamma]$ | 서로 homotopic한 based loop들을 한 부류로 묶은 것 |
| concatenation $*$ | 두 loop를 순서대로 이어붙이는 연산 |
| identity | 다른 원소와 결합해도 바꾸지 않는 원소; constant loop class |
| inverse | 원래 원소와 결합하면 identity가 되는 원소; reverse loop class |
| group | 연산, associativity, identity, inverse를 갖는 구조 |
| fundamental group $\pi_1(X,x_0)$ | based loop homotopy classes와 concatenation으로 만든 group |

---

## 확인문제

### 1번
$[\gamma]$는 loop 하나인가, 아니면 무엇인가?

### 2번
$\gamma_1*\gamma_2$는 무엇을 뜻하는가?

### 3번
constant loop가 identity 역할을 하는 이유를 설명하라.

### 4번
reverse loop는 어떤 group 역할을 하는가?

### 5번
왜 concatenation의 associativity를 homotopy class 수준에서 말하는 것이 자연스러운가?

### 6번
$\pi_1(X,x_0)$가 loop의 개수와 다른 이유는 무엇인가?

### 7번
fundamental group이 공간의 모든 topology를 완전히 결정하는가?

### 8번
actual physical configuration space의 $\pi_1$를 현재 ideal Map₁ 결과와 자동 동일시할 수 있는가?

---

## 정답과 설명

### 1번
서로 homotopic한 based loop들을 모두 묶은 homotopy class다.

### 2번
첫 loop를 따라간 뒤 두 번째 loop를 이어서 따라가는 concatenated loop다.

### 3번
constant loop를 앞이나 뒤에 이어붙여도 원래 loop와 같은 homotopy class가 남기 때문이다.

### 4번
inverse 역할을 한다.

### 5번
path 함수로서는 parameter 분할 방식이 달라질 수 있지만 그 차이는 homotopy로 없앨 수 있기 때문이다.

### 6번
무한히 많은 raw loop들이 같은 homotopy class 하나에 들어갈 수 있기 때문이다.

### 7번
아니다. fundamental group은 중요한 불변량이지만 모든 위상 정보를 담는 것은 아니다.

### 8번
아니다. actual physical configuration space와 ideal Map₁의 동일성은 **OPEN**이다.

---

## 이 장의 근거 자료

| 자료 | 역할 | 종류 |
|---|---|---|
| Allen Hatcher, *Algebraic Topology*, §1.1 | fundamental group, path homotopy, concatenation의 표준 정의 | [외부 수학] |
| G02 | degree-one mapping space의 $\pi_1$ 질문 도입 | [일반 연구] |
| G03 | evaluation-fibration 및 loop topology 연구의 배경 | [일반 연구] |
| A01 | ideal mapping-space theorem의 조건과 proof scope | [적대적 감사] |
| C02 | physical quotient/topology 경고 | [최신 적대적 감사] |
| `sources/proof-status.md` | physical configuration-space identification OPEN | [프로젝트 상태] |

---

## 제14장 제작 기록

- **Canonical file:** `volume-1/14-fundamental-group.md`
- **작성 상태:** DRAFT COMPLETE
- **감사 상태:** AUDIT PENDING
- **작성자 자체 PASS:** 부여하지 않음
- **핵심 목적:** 제15장의 $\mathbb Z_2$ 결과를 읽기 위한 표준 fundamental-group 언어 구축
- **다음 작업:** FINAL BATCH 규칙에 따른 Chapter 15 DRAFT

[^v1c14-based-loop]: 미리 정한 한 점에서 출발해 같은 점으로 돌아오는 loop다. fundamental group에서는 이 기준점을 고정해 비교한다.

[^v1c14-homotopy-class]: 서로 연속적으로 변형 가능한 대상들을 “같은 종류”로 묶은 부류다. $[\gamma]$는 loop 하나가 아니라 그 loop와 homotopic한 loop들의 class다.

[^v1c14-concatenation]: 한 loop를 끝까지 따라간 뒤 두 번째 loop를 이어 따라가는 결합 연산이다.

[^v1c14-group]: 원소들의 집합과 결합 규칙이 있고, associativity·identity·inverse 같은 규칙을 만족하는 대수적 구조다.

[^v1c14-fundamental-group]: 한 공간에서 based loop들의 homotopy class를 모으고 concatenation을 연산으로 둔 group이다. 공간의 loop형 위상 구조를 감지한다.

[^v1c14-basepoint]: based loop가 출발하고 돌아오는 기준점이다.

[^v1c14-equivalence-class]: 어떤 “같다고 보기” 규칙을 만족하는 대상들을 한 묶음으로 모은 것이다. 여기서는 homotopy로 서로 바뀌는 loop들을 한 묶음으로 본다.

[^v1c14-identity]: 다른 원소와 결합해도 그 원소를 바꾸지 않는 특별한 원소다.

[^v1c14-inverse]: 원래 원소와 결합했을 때 identity가 되게 하는 짝이다.

[^v1c14-associativity]: 세 원소를 결합할 때 어느 두 개를 먼저 묶어 계산해도 최종 결과가 같다는 규칙이다.

[^v1c14-path-connected]: 공간의 임의의 두 점을 그 공간 안의 path로 연결할 수 있다는 뜻이다.

[^v1c14-isomorphism]: 두 group이 원소 이름은 달라도 연산 구조가 완전히 같은 방식으로 대응된다는 뜻이다.

[^v1c14-basepoint-precision]: path-connected 공간의 서로 다른 basepoint에서 얻은 fundamental group들은 isomorphic하다. 다만 두 basepoint를 잇는 어떤 path를 선택했는지에 따라 구체적인 대응이 달라질 수 있어, 일반적으로 “아무 선택 없이 완전히 같은 group”이라고 쓰지는 않는다.
