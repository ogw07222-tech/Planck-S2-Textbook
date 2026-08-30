> **STATUS: DRAFT COMPLETE · AUDIT PENDING**
>
> 작성 Chat은 PASS를 부여하지 않는다. topology/FR이 줄 수 있는 sector 제약과 physical $j=1/2$ ground-state 결론을 분리한다.

# 14장 · 왜 아직 spin-1/2 증명이 아닌가 — sector, j=1/2, ground state의 차이

## 현재 상태
- **작성 상태:** DRAFT COMPLETE
- **감사 상태:** AUDIT PENDING
- **핵심 경계:** half-integer sector = **CONDITIONAL**, complete spin-$1/2$ = **OPEN**, $j=1/2$ ground = **OPEN**.

---

## 이번 장의 질문
1. “half-integer sector가 허용된다”와 “입자가 spin-1/2이다”는 왜 다른가?
2. representation label $j=1/2$을 허용하는 것과 실제로 선택하는 것은 왜 다른가?
3. ground state[^v2c14-ground-state]는 topology가 아니라 왜 dynamics의 문제인가?
4. physical Hilbert space[^v2c14-hilbert], Hamiltonian[^v2c14-hamiltonian], domain[^v2c14-domain]이 왜 필요할까?
5. 과거 “2-state → 1 qubit” 주장은 왜 이 장에서 다시 경계해야 할까?

---

## 세 단계를 처음부터 분리하자

이 장의 핵심은 다음 세 문장을 절대로 한 문장으로 합치지 않는 것이다.

### A. half-integer sector 허용

FR-odd 조건이 physical하게 성립하면

$$
j=\frac12,\frac32,\frac52,\ldots
$$

같은 half-integer sector가 허용될 수 있다.

현재 판정: **CONDITIONAL**.

### B. j=1/2 representation 선택

half-integer들 중 실제 state가 $j=1/2$ representation에 놓이는가?

현재 판정: **OPEN**.

### C. j=1/2이 physical ground state

모든 허용 state의 energy를 비교했을 때 $j=1/2$이 가장 낮은가?

현재 판정: **OPEN**.

---

## 먼저 생각해 보기 · 입장 가능한 반과 1등 학생

어떤 대회에서 “A반 학생만 참가 가능”이라는 규칙이 있다고 하자.

이 규칙은 참가 가능한 **범위**를 정한다.

하지만

- A반에서 누가 실제 출전할지,
- 누가 가장 점수가 높을지,
- 누가 우승할지

는 별도 정보다.

FR-odd가 half-integer sector를 허용한다는 것도 비슷하다.

### 비유의 한계

representation sector는 실제 학교 반이 아니고, quantum state selection은 단순한 인간의 선택도 아니다. 실제 selection은 Hamiltonian, symmetry, boundary condition, dynamics에 의해 결정된다.

---

## topology가 해 준 일

이상적인 unquotiented branch에서 topology와 FR-odd condition을 결합하면 integer-$j$와 half-integer-$j$ 사이를 구분하는 selection rule의 후보가 생긴다.

즉 topology는 가능한 representation들의 **종류를 제한**하는 데 도움을 줄 수 있다.

하지만 topology는 일반적으로 각 representation의 energy를 계산하지 않는다.

---

## j=1/2을 선택하려면 무엇이 필요한가

$j=1/2$을 actual physical state로 고르려면 적어도 어떤 quantum Hilbert space에서 rotation representation이 어떻게 분해되는지 알아야 한다.

또 physical Hamiltonian

$$
H
$$

이 그 공간에서 어떻게 작용하는지 알아야 한다.

그리고 eigenvalue problem

$$
H\Psi=E\Psi
$$

을 풀어 각 sector의 energy를 비교해야 한다.

이 정보 없이

> “half-integer니까 가장 작은 $j=1/2$이겠지”

라고 말하는 것은 수학적·물리적 비약이다.

---

## ground state는 무엇인가

ground state는 허용되는 quantum states 가운데 가장 낮은 energy를 갖는 state 또는 ground eigenspace를 뜻한다.

따라서 “ground”라는 단어 자체가 Hamiltonian과 spectrum을 필요로 한다.

단순 topology만으로는

$$
E_{1/2}<E_{3/2}<E_{5/2}<\cdots
$$

같은 ordering을 자동으로 만들 수 없다.

---

## physical Hilbert space와 domain이 왜 중요할까

Hamiltonian은 아무 함수에나 무조건 작용하는 기호가 아니다.

- 어떤 wavefunctions가 state space에 들어가는가?
- 어떤 boundary/FR condition을 만족해야 하는가?
- operator의 self-adjoint domain은 무엇인가?
- target symmetry와 spatial symmetry가 quantum level에서 어떻게 lift되는가?

가 정해져야 spectrum 문제를 정확히 말할 수 있다.

canonical C02에서는 physical Hilbert realization, quantum lift, external rotation matching이 여전히 OPEN이다.

---

## complete spin-1/2이라는 말에는 더 많은 것이 필요하다

실제 spin-$1/2$ particle을 말하려면 단순한 $2\pi$ sign 외에도 arbitrary-axis rotations 아래 full representation이 일관되게 정의돼야 한다.

최소한 다음 구분이 필요하다.

- rotation group action
- quantum Hilbert-space representation
- $j=1/2$ block의 존재와 physical selection
- Hamiltonian/dynamics
- external 3+1D rotation과의 matching

현재 이 chain은 Planck-S²에서 모두 닫히지 않았다.

따라서

> **complete spin-1/2: OPEN.**

---

## 과거 2-state → 1 qubit 오류를 짧게 복습

프로젝트의 과거 G06에는 $j=1/2$ rotor의 상태수를 단순히 $2j+1=2$로 세어 “전체 상태수 2 → 1 qubit”로 연결한 주장이 있었다.

후속 A01/C02 감사에서는 full spherical rotor fixed-$j$ block에 left/right labels가 함께 있어 dimension이

$$
(2j+1)^2
$$

이 될 수 있고, $j=1/2$이면 4-state라는 점을 지적했다.

따라서 과거 문장

> $j=1/2$ rotor 전체 상태수 $=2\Rightarrow1$ qubit

은 **FALSIFIED AS WRITTEN**이다.

또 더 근본적으로

$$
Q=1=1\text{ bit}
$$

도 **FALSIFIED AS WRITTEN**이다.

이 상세 rotor counting은 제3권에서 더 깊게 다룬다.

---

## 현재 판정표

| 단계 | 현재 판정 | 필요한 추가 구조 |
|---|---|---|
| FR-odd 조건 아래 half-integer sector | **CONDITIONAL** | physical space/lift/rotation branch |
| $j=1/2$ representation의 actual selection | **OPEN** | full Hilbert decomposition/physical state selection |
| $j=1/2$ ground state | **OPEN** | Hamiltonian, domain, complete spectrum |
| complete spin-$1/2$ | **OPEN** | full 3D rotation representation + physical matching |
| G06 2-state→1-qubit 전체-state 주장 | **FALSIFIED AS WRITTEN** | 제3권 state-count audit |
| $Q=1=1$ bit | **FALSIFIED AS WRITTEN** | degree와 정보량은 다른 양 |
| 전체 Planck-S² | **WORKING HYPOTHESIS** | 전체 bridge 미완성 |

---

## 이것으로 말할 수 있는 것
- half-integer sector와 $j=1/2$은 같은 말이 아니다.
- representation label과 energy ordering은 서로 다른 문제다.
- ground-state claim에는 Hamiltonian과 spectrum이 필요하다.

## 이것으로 말할 수 없는 것
- $2\pi\to-1$만으로 electron의 complete spin-$1/2$이 증명됐다고 할 수 없다.
- 가장 작은 half-integer라는 이유로 $j=1/2$이 ground라고 할 수 없다.
- $j=1/2$ representation dimension만 보고 full physical state count를 확정할 수 없다.

---

## 다음 장이 필요한 이유

지금까지의 FR chain은 대부분 **unquotiented ideal configuration-space branch**를 기준으로 설명했다.

하지만 physical state에서 target rotations를 실제 자유도로 볼 것인가, redundancy로 quotient할 것인가는 topology 자체를 바꿀 수 있다.

제2권 마지막 핵심 장에서 Gate C의 두 갈림길을 본다.

---

## 한 문장 기억

> **topology/FR은 조건부로 half-integer sector를 제한할 수 있지만, $j=1/2$ 선택과 $j=1/2$ ground state는 별도의 Hilbert-space와 dynamics 문제다.**

---

## 확인문제
1. A/B/C 세 단계를 각각 말해 보라.
2. 왜 topology만으로 ground state를 고를 수 없는가?
3. G06의 2-state 주장이 왜 제3권 감사 대상으로 남는가?

## 정답
1. A half-integer 허용, B $j=1/2$ actual selection, C $j=1/2$ ground.
2. energy ordering을 계산할 Hamiltonian과 spectrum이 필요하기 때문이다.
3. rotor Hilbert block의 multiplicity를 단순 $2j+1$로 세면 안 되고 physical Hilbert realization도 아직 미완성이기 때문이다.

---

## 근거 자료
- **G04**: half-integer sector/FR project construction.
- **G06**: 과거 state-count/1-qubit 주장.
- **A01**: $j=1/2$ 선택 OPEN, G06 state-count 반증.
- **C02**: FR-odd rotor 4-state assumption-scoped 결과와 full physical Hilbert OPEN.

[^v2c14-ground-state]: 주어진 Hamiltonian의 허용 state들 가운데 가장 낮은 energy를 갖는 state 또는 eigenspace.
[^v2c14-hilbert]: quantum states를 벡터로 다루기 위한 inner-product가 있는 완비 벡터공간. 어떤 함수들이 실제 state인지 정하는 물리적 구조가 필요하다.
[^v2c14-hamiltonian]: quantum system의 energy와 time evolution을 결정하는 operator.
[^v2c14-domain]: operator가 실제로 작용하도록 허용된 state들의 집합. 무한차원 quantum operator에서는 domain 선택이 self-adjointness와 spectrum에 중요하다.
