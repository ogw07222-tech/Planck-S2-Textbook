# Chapter 4 Audit — 함수는 입력을 출력으로 보내는 규칙

- **Audit basis:** `Planck-S2_교과서_제1권_구위의화살표에서위상수학까지-7.docx`
- **Audit date:** 2026-08-29
- **Verdict:** **PASS — RECOVERY CLOSED · CHAPTER 5 DRAFT APPROVED**

## Evidence

독립 감사에서 최신 제1권 복구본을 확인했다. 제4장 본문은 실제 artifact의 후반부에 존재하며, 이전에 누락되었던 F005와 F1X02도 실제 그림으로 삽입되어 있다.

- 제4장 본문: 존재 확인
- F005: 존재 확인
- F1X02: 존재 확인
- 제5장 본문: 아직 시작하지 않음

## Mathematical audit

다음 필수 조건을 모두 충족한다.

- 함수는 domain의 각 원소에 target의 **정확히 하나**의 값을 대응시킨다고 명시한다.
- 함수는 반드시 일대일일 필요가 없으며 many-to-one이 허용됨을 설명한다.
- 한 입력에 서로 다른 두 출력이 동시에 정해지면 보통의 함수가 아님을 명시한다.
- domain과 target/codomain을 구분한다.
- target/codomain과 실제 image를 구분한다.
- 출력은 숫자뿐 아니라 점·색·방향 등이 될 수 있음을 제시한다.
- $f:X\to Y$, $x\mapsto f(x)$ 표기를 설명한다.
- 이후 $n:S^2\to S^2$ 표기를 읽기 위한 준비로 범위를 제한한다.

**판정: PASS.**

## Figure audit

### F005

PASS.

- domain $X$의 각 입력에 정확히 하나의 출력이 대응된다.
- 서로 다른 두 입력이 같은 $y_2$로 가는 many-to-one 예가 들어 있어 “함수=일대일” 오해를 방지한다.
- target의 사용되지 않는 점을 보여 image와 target이 같을 필요가 없음을 시각화한다.
- `이 그림에서 볼 것 / 이 그림이 뜻하는 것 / 이 그림이 뜻하지 않는 것` 3단 경계를 갖춘다.

### F1X02

PASS.

- 숫자→숫자
- 점→색
- 점→방향

의 세 map 예가 실제 그림으로 들어 있다. 또한 점→방향 그림을 실제 전자의 내부 방향장 관측으로 오해하지 않도록 제한문을 포함한다.

## Scientific / interpretation audit

PASS.

제4장은 표준 함수·사상 언어를 설명하는 수학 준비 장으로 유지된다. $n:S^2\to S^2$ 표기를 사용한다는 사실만으로 실제 전자의 내부 $S^2$가 존재한다고 주장하지 않는다.

- 함수/사상 언어: **SOURCE VERIFIED**
- G02의 $n:S^2_{domain}\to S^2_{internal}$ 사용: **PROJECT MODEL CHOICE**
- 실제 전자의 physical internal field 여부: **OPEN**
- Planck-S² 전체: **WORKING HYPOTHESIS**

## Educational audit

PASS.

3장 $S^2$ → 4장 function/map → 5장 field로 이어지는 개념 의존관계가 복구되었다. 자판기 비유의 한계도 명시되어 있으며, 짧은 wiki 요약이 아니라 장문 교과서 구조가 유지된다.

## Previous blockers

| Blocker | Previous status | Current status |
|---|---|---|
| Chapter 4 body missing | OPEN / FAIL | **CLOSED** |
| F005 missing | OPEN / FAIL | **CLOSED** |
| F1X02 missing | OPEN / FAIL | **CLOSED** |
| unique-output rule missing | REQUIRED | **SATISFIED** |
| many-to-one clarification | REQUIRED | **SATISFIED** |
| domain/target/image distinction | REQUIRED | **SATISFIED** |

## Final status

**PASS — Chapter 4 DRAFT COMPLETE.**

제4장 복구 blocker는 닫혔다. `STATUS.md`는 Chapter 4 `DRAFT COMPLETE / PASS`로 갱신한다.

**다음 허용 작업: Chapter 5 DRAFT.**

**Chapter 6는 Chapter 5의 독립 감사 PASS 전까지 시작하지 않는다.**
