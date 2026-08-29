# Planck-S2 Textbook

이 저장소는 「Planck-S²를 처음부터 이해하는 책」 6권 교과서 프로젝트의 **canonical working source**다.

- 전체 Planck-S² 전자 가설의 현재 상태는 **WORKING HYPOTHESIS**다.
- **Markdown이 유일한 작업 원본(single source of truth)** 이다.
- DOCX/PDF는 앞으로 출판·배포 산출물로만 생성한다.
- `MASTER.md`는 안정적인 제작 규칙·source freeze·증명상태 기준선을 관리한다.
- `STATUS.md`는 현재 제작 진행상태를 **한 곳에서만** 관리한다.
- `volume-*`는 권별 본문/outline Markdown을 관리한다.
- `audits/`는 장별 적대적 감사 기록을 관리한다.
- `figures/`는 실제 그림 asset과 figure registry를 관리한다.
- `sources/`는 source inventory와 현재 proof-status ledger를 관리한다.
- source freeze는 **C02까지의 frozen production baseline**을 사용한다. C_LIFT 및 이후 새 연구는 자동 소급 병합하지 않는다.

> Legacy DOCX는 migration source일 뿐 canonical source가 아니다. 버전 파일(`-1`, `-2`, `-final` 등)을 새로 만들지 않고 Git commit history로 변경 이력을 보존한다.
