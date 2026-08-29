> **STATUS: DRAFT COMPLETE · AUDIT PENDING**
>
> VOLUME 1 FINAL BATCH DRAFT MODE에서 작성한 역사/감사 초안이다. 작성 Chat은 PASS를 부여하지 않으며, 과거 문장의 현재 판정은 frozen baseline과 `sources/proof-status.md`를 따른다.

# 16장 · v0.1에서 v0.3 직전까지: 왜 여기까지 왔나

## 현재 상태

- **작성 상태:** DRAFT COMPLETE
- **감사 상태:** AUDIT PENDING
- **역할:** 제1권에서 배운 개념이 초기 Planck-S² 연구에서 어떤 순서로 등장했는지 추적
- **새 증명:** 없음
- **핵심 경계:** 연구가 한 방향으로 좁혀졌다는 사실은 그 방향이 실제 전자 이론으로 증명됐다는 뜻이 아니다.

---

## 이번 장에서 알아낼 질문

1. 처음의 “입자에 더 깊은 내부 자유도가 있을 수 있는가?”라는 넓은 질문이 왜 $S^2\to S^2$로 좁혀졌을까?
2. 왜 2차원과 $S^2$가 후보 언어로 선택됐을까?
3. 왜 한 점의 방향보다 field 전체와 degree가 중요해졌을까?
4. 왜 $Q=1$ sector가 연구 대상으로 선택됐을까?
5. configuration과 configuration space가 왜 필요해졌을까?
6. 왜 path, loop, homotopy, $\pi_1$까지 질문이 확장됐을까?
7. 당시 문서의 직관 가운데 현재 살아남은 것과 강등된 것은 무엇일까?
8. 왜 $\mathbb Z_2$ 구조를 얻어도 아직 electron proof라고 부를 수 없을까?

---

## 이 장을 읽는 법

이 장에서는 세 시간을 구분한다.

### 1. 당시 연구자가 생각했던 것

어떤 방향을 시험해 볼 가치가 있다고 본 연구 직관이다.

### 2. 당시 문서가 실제로 주장한 것

G01, G02, G03 등 당시 보고서에 적힌 구체적 claim이다.

### 3. 현재 판정

후속 A01, C02와 canonical proof ledger까지 반영한 오늘의 상태다.

이 세 층을 섞으면 과거 아이디어가 현재 검증된 사실처럼 보일 수 있으므로 반드시 분리한다.

---

## 먼저 생각해 보기 · 과학 수사와 디버깅

복잡한 프로그램에 오류가 있다고 하자.

처음에는 가능한 원인이 아주 많다.

- 입력 문제일 수도 있고,
- 메모리 문제일 수도 있고,
- 알고리즘 문제일 수도 있고,
- 인터페이스 문제일 수도 있다.

검사를 하면서 가능성을 하나씩 줄인다.

Planck-S² 초기 연구도 비슷했다.

처음에는 내부 자유도의 종류가 넓게 열려 있었지만, 구체적으로 계산할 수 있는 후보를 고르고 그 후보가 어떤 수학 구조를 갖는지 따라가면서 질문이 좁아졌다.

### 비유의 한계

디버깅에서 원인을 좁혔다고 해서 마지막 후보가 반드시 정답인 것은 아니다.

마찬가지로 연구 경로가 $S^2\to S^2$와 topology 쪽으로 좁혀졌다는 사실만으로 그 모델이 실제 전자라는 뜻은 아니다.

---

## 1단계 · 출발점은 “입자란 무엇인가?”였다

G01의 출발 질문은 매우 넓었다.

표준 입자물리에서 전자는 기본입자로 다뤄지지만, 그 사실을 “더 깊은 내부 자유도는 절대로 존재할 수 없다”는 존재론적 증명으로 과장하면 안 된다는 문제의식이 있었다.

여기서 후보 질문이 생겼다.

> 외부에서는 point-like하게 기술되는 입자가 더 근본적인 층에서는 어떤 내부/경계 자유도를 가질 수 있는가?

현재 살아남는 것은 **이 질문을 연구 질문으로 던질 수 있다는 것**이지, 실제 전자 내부구조가 발견됐다는 결론이 아니다.

실제 electron 내부 $S^2$ 구조는 계속 **OPEN**이다.

---

## 2단계 · 왜 2차원과 S²가 등장했나

초기 문서에서는 내부/경계 후보를 2차원으로 두는 아이디어가 등장했다.

제1권 2~3장에서 배운 것처럼

- 2차원이라는 말은 intrinsic dimension을 뜻해야 하고,
- $S^2$는 속이 찬 공 $B^3$가 아니라 2차원 구면이며,
- 3차원에 그려진다고 해서 intrinsic dimension이 3이 되는 것은 아니다.

이 구분이 중요한 이유는 Planck-S²의 후보 공간을 수학적으로 정확히 읽기 위해서다.

하지만 “2차원 $S^2$가 실제 전자 내부에 존재한다”는 물리적 주장은 현재 **OPEN**이다.

---

## 3단계 · 내부 자유도를 field로 쓰기

G02에서는 후보 내부 자유도를 더 구체적으로

$$
n:S^2_{\rm domain}\to S^2_{\rm target}
$$

라는 unit-vector field 형태로 다루는 방향이 중심이 되었다.

이 선택으로 질문이 훨씬 명확해졌다.

- domain의 어디에서 값을 읽는가?
- target에서 어떤 방향값을 얻는가?
- field 전체는 어떤 map인가?

제5~6장이 바로 이 언어를 초보자 수준에서 준비했다.

현재 판정에서는 이 $n$-field 선택 자체가 **PROJECT MODEL CHOICE / CONDITIONAL**이며, 실제 전자의 physical field임은 **OPEN**이다.

---

## 4단계 · field 전체를 정수 Q로 분류하기

$S^2\to S^2$ map을 쓰면 degree를 정의할 수 있다.

$$
Q=\deg(n)\in\mathbb Z.
$$

이것이 G02 이후 연구에서 중요한 이유는 무수히 많은 field 모양을 전역적 topological sector로 나눌 수 있기 때문이다.

프로젝트는 그중

$$
Q=1
$$

sector를 중심 후보로 선택했다.

여기서 현재 반드시 구분한다.

- degree의 표준 수학: **SOURCE VERIFIED**
- $Q=1$ sector를 후보로 고르는 것: **CONDITIONAL · PROJECT MODEL CHOICE**
- 실제 electron이 $Q=1$ physical sector라는 주장: **OPEN**

---

## 5단계 · Q=1에 너무 많은 뜻을 붙이면 안 됐다

초기 연구 흐름에서는 topology와 정보량, charge, particle identity를 연결하려는 직관이 여러 방향으로 등장했다.

후속 감사가 특히 강하게 막은 비약이 있다.

### $Q=1=1$ bit

현재 판정:

> **FALSIFIED AS WRITTEN**

$Q$는 degree이고 bit는 정보량이다. 숫자가 같다고 같은 물리량이 아니다.

### $Q=1=$ charge $-e$

현재 판정:

> **OPEN**

전자기 $U(1)$ coupling과 실제 전하 observable로의 bridge가 아직 없다.

### $Q=1=$ electron identity

현재 판정:

> **OPEN**

spin, statistics, mass, QED, observables 등 필요한 연결이 아직 남아 있다.

이것이 제8장의 핵심 경계였다.

---

## 6단계 · 한 field 전체를 configuration으로 보기

degree만 알면 field의 모든 세부 모양이 정해지는 것은 아니다.

같은 $Q=1$ sector 안에도 서로 다른 많은 field configuration이 있을 수 있다.

그래서 연구의 단위가

> 한 점의 $n(x)$

에서

> full field $n(\cdot)$ 하나, 즉 configuration 하나

로 이동한다.

제9장에서 우리는

$$
x\neq n(x)\neq n(\cdot)
$$

의 역할을 분리했다.

---

## 7단계 · 가능한 configuration 전체를 공간으로 보기

다음 단계는 configuration들을 전부 모으는 것이다.

ideal 후보 언어로

$$
\mathcal C_1=\mathrm{Map}_1(S^2,S^2)
$$

를 생각할 수 있다.

여기서 configuration 하나가 $\mathcal C_1$의 “점 하나”가 된다.

이 생각 덕분에

- path,
- loop,
- homotopy,
- fundamental group

을 질문할 수 있게 되었다.

하지만 후속 감사에서 가장 중요한 경계도 여기 생겼다.

> **actual physical configuration space = ideal/unquotiented Map₁: OPEN**

completion, finite-energy, quotient, EFT-valid subset, ontology가 아직 닫히지 않았다.

---

## 8단계 · path와 loop를 묻기

G03으로 가는 연구 흐름에서는 configuration space 안에서 field 전체가 연속적으로 변하는 family를 생각했다.

$$
\gamma:[0,1]\to\mathcal C_1.
$$

시작과 끝이 같으면 loop가 된다.

$$
\gamma(0)=\gamma(1).
$$

이때 중요한 질문은 “끝에서 같은 configuration으로 돌아왔는가?”만이 아니었다.

> 그 loop가 어떤 homotopy class에 속하는가?

가 핵심이 되었다.

---

## 9단계 · topology와 π₁ 질문으로 좁혀지기

loop들을 homotopy class로 묶고 concatenation하면 fundamental group을 만들 수 있다.

초기 mapping-space 연구에서 결국 다음 구조가 핵심 대상이 되었다.

$$
\pi_1(\mathrm{Map}_1(S^2,S^2)).
$$

현재 frozen baseline에서는

$$
\pi_1(\mathrm{Map}_1(S^2,S^2))\cong\mathbb Z_2
$$

가 **PROVED UNDER ASSUMPTIONS**로 살아남는다.

하지만 이 statement는 ideal smooth/unquotiented mapping-space setting의 결과다.

actual physical electron configuration space의 $\pi_1$가 $\mathbb Z_2$라고 확정한 것은 아니다.

---

## 당시 주장 / 현재 판정 표

| 당시 연구에서 등장한 생각 또는 주장 | 현재 판정 | 현재 읽는 법 |
|---|---|---|
| 전자 후보에 2D/$S^2$ 내부 자유도를 둘 수 있다 | **OPEN / MODEL HYPOTHESIS** | 후보 질문이지 관측 사실 아님 |
| $n:S^2\to S^2$를 기본 후보장으로 사용 | **CONDITIONAL · PROJECT MODEL CHOICE** | 모델 선택 |
| degree $Q$로 map을 분류 | **SOURCE VERIFIED** | 표준 수학 |
| $Q=1$ sector를 중심 후보로 선택 | **CONDITIONAL · PROJECT MODEL CHOICE** | electron identity와 별개 |
| $Q=1=1$ bit | **FALSIFIED AS WRITTEN** | degree와 information 분리 |
| $Q=1=$ charge $-e$ | **OPEN** | electromagnetic bridge 미유도 |
| ideal $\mathrm{Map}_1$를 연구 | **SOURCE VERIFIED AS PROJECT HISTORY** | 수학적 후보 공간 |
| actual physical space = ideal Map₁ | **OPEN** | quotient/completion/ontology 미폐쇄 |
| $\pi_1(\mathrm{Map}_1)\cong\mathbb Z_2$ | **PROVED UNDER ASSUMPTIONS** | ideal smooth/unquotiented 범위 |
| FR-odd $2\pi\to-1$ | **CONDITIONAL** | 제2권 이후의 추가 구조 필요 |
| 완전한 spin-$1/2$ / electron identity | **OPEN** | 아직 미도출 |

---

## 왜 U(1), spinor, FR 같은 이름은 여기서만 살짝 보이나

초기 연구사에는 electromagnetic $U(1)$, spinor[^v1c16-spinor], FR quantization[^v1c16-fr] 같은 용어가 등장한다.

하지만 제1권은 이들의 정식 이론을 가르치는 권이 아니다.

여기서는 오직 역사적 표지로만 이해한다.

- U(1): charge bridge와 관련된 별도 물리 구조
- spinor: 회전 아래 특수한 변환법칙을 갖는 양자 상태 언어
- FR: configuration-space topology를 양자화 조건과 연결하는 후속 구조

이 세 가지 모두 제1권의 $\mathbb Z_2$ 언어만으로 자동 완성되지 않는다.

---

## 현재 살아남은 가장 좁고 안전한 줄기

제1권에서 역사적으로 살아남은 가장 안전한 줄기는 다음처럼 적을 수 있다.

> 후보 $S^2\to S^2$ field 언어
> → degree 분류
> → $Q=1$ ideal mapping sector
> → configuration-space topology 질문
> → ideal/unquotiented $\pi_1\cong\mathbb Z_2$의 조건부 수학 결과

이 줄기는 실제 electron proof가 아니라 **후속 연구를 가능하게 하는 수학적 골격**이다.

---

## 무엇이 아직 OPEN인가

현재도 다음은 해결되지 않았다.

- 실제 electron에 $S^2$ internal field가 있는가?
- physical configuration space가 무엇인가?
- ideal Map₁와 physical space가 같은가?
- 특정 $2\pi$ spatial rotation loop가 physical generator인가?
- FR quantization이 실제 물리적으로 적용되는가?
- spin-$1/2$, charge $-e$, QED, Fermi statistics가 나오는가?

전체 프로젝트는 여전히 **WORKING HYPOTHESIS**다.

---

## 자주 하는 오해

### 오해 1 · “연구가 S²→S²로 좁혀졌으니 그게 정답이었나 보다.”

아니다. 계산 가능한 후보로 좁힌 것이지 자연이 그 후보를 선택한다는 증명이 아니다.

### 오해 2 · “Z₂까지 나왔으니 초기 아이디어가 전부 검증됐다.”

아니다. ideal mapping-space theorem의 조건부 생존과 physical electron bridge는 별개다.

### 오해 3 · “과거 문서에 1 bit라고 썼으니 현재도 유효하다.”

아니다. $Q=1=1$ bit는 **FALSIFIED AS WRITTEN**이다.

### 오해 4 · “charge는 topology에서 곧바로 나왔다.”

아니다. $Q=1=$ charge $-e$는 **OPEN**이다.

### 오해 5 · “FR이라는 이름이 나왔으니 2π→−1이 이미 끝났다.”

아니다. FR-odd $2\pi\to-1$은 현재도 **CONDITIONAL**이고 본격적인 연결은 제2권이다.

---

## 다음 장이 필요한 이유

이제 연구가 왜 현재의 수학 사다리까지 왔는지 알았다.

마지막으로 제1권 전체를 처음부터 다시 한 줄로 연결하고, 어디까지가 실제 도달점이며 다음 권에서 어떤 질문이 남는지 정리할 필요가 있다.

---

## 한 문장 기억

> **Planck-S² 초기 연구는 넓은 내부구조 질문에서 $S^2\to S^2$, degree, configuration-space topology로 점차 좁혀졌지만, 그 연구 경로 자체가 실제 electron을 증명하지는 않는다.**

---

## 용어 카드

| 용어 | 이 장에서의 뜻 |
|---|---|
| project history | 어떤 아이디어와 질문이 어떤 순서로 등장했는지의 기록 |
| downgrade | 후속 감사에서 claim의 범위를 더 약하거나 조건부 상태로 낮추는 것 |
| bridge | 서로 다른 수학/물리 구조를 실제 이론 안에서 연결하는 추가 유도 |
| spinor | 회전 아래 일반 벡터와 다른 방식으로 변환하는 양자 상태 언어 |
| FR quantization | configuration-space topology를 양자상태의 조건과 연결하는 후속 양자화 방법 |

---

## 확인문제

### 1번
초기 넓은 내부구조 질문이 왜 $n:S^2\to S^2$ 같은 구체적 모델로 좁혀졌는가?

### 2번
$Q=1$ sector를 선택했다는 것과 electron identity를 증명했다는 것은 같은 말인가?

### 3번
왜 configuration space가 필요했는가?

### 4번
현재 $Q=1=1$ bit의 판정은 무엇인가?

### 5번
현재 $Q=1=$ charge $-e$의 판정은 무엇인가?

### 6번
$\pi_1(\mathrm{Map}_1)\cong\mathbb Z_2$의 현재 범위는 무엇인가?

### 7번
왜 actual physical configuration space를 ideal Map₁와 자동 동일시할 수 없는가?

### 8번
이 장에서 FR을 정식으로 증명하지 않는 이유는 무엇인가?

---

## 정답과 설명

### 1번
넓은 후보군 가운데 실제로 수학적으로 정의하고 topology를 계산할 수 있는 구체적 후보를 선택해야 했기 때문이다. 선택 자체가 자연의 정답임을 뜻하지는 않는다.

### 2번
아니다. $Q=1$ 선택은 모델 선택이고 electron identity는 훨씬 강한 physical claim이다.

### 3번
가능한 full field configuration들을 한 공간의 점처럼 모아 path, loop, homotopy, fundamental group을 질문하기 위해서다.

### 4번
**FALSIFIED AS WRITTEN**이다.

### 5번
**OPEN**이다.

### 6번
ideal smooth/unquotiented mapping-space 설정의 명시 가정 아래 **PROVED UNDER ASSUMPTIONS**이다.

### 7번
finite-energy, completion, EFT-valid subset, quotient, ontology 문제가 아직 닫히지 않았기 때문이다.

### 8번
FR은 topology와 quantum-state boundary condition을 연결하는 추가 구조이며, 제1권의 표준 topology 언어만으로 자동 결론나지 않기 때문이다.

---

## 이 장의 근거 자료

| 자료 | 역할 | 종류 |
|---|---|---|
| G01 | 초기 내부구조·2D/$S^2$ 후보 질문 | [일반 연구] |
| G02 | $n:S^2\to S^2$, degree $Q=1$, mapping-space topology로의 집중 | [일반 연구] |
| G03 | loop, evaluation-fibration, rotation-generator 질문으로의 발전 | [일반 연구] |
| A01 | G01–G03의 논리 감사와 살아남은 mapping-space result 범위 | [적대적 감사] |
| C02 | physical quotient/ontology와 topology 적용 경계 | [최신 적대적 감사] |
| `sources/proof-status.md` | 현재 proof labels의 canonical ledger | [프로젝트 상태] |

---

## 제16장 제작 기록

- **Canonical file:** `volume-1/16-history-v01-v03.md`
- **새 증명:** 없음
- **작성 상태:** DRAFT COMPLETE
- **감사 상태:** AUDIT PENDING
- **작성자 자체 PASS:** 부여하지 않음
- **핵심 편집 원칙:** 당시 연구 생각 / 당시 claim / 현재 판정을 분리
- **다음 작업:** FINAL BATCH 규칙에 따른 Volume 1 Closing DRAFT

[^v1c16-spinor]: 공간을 한 바퀴 회전했을 때 일반적인 3차원 벡터와 다른 방식으로 변환할 수 있는 양자상태의 수학 언어다. 정식 정의는 제2권에서 다룬다.

[^v1c16-fr]: Finkelstein–Rubinstein 양자화의 약칭이다. configuration space의 위상적 loop 구조를 양자상태의 부호/경계조건과 연결하는 방법이며, 실제 Planck-S² 적용은 조건부 문제다.
