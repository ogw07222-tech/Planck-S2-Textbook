# Audits

장별 감사 파일은 canonical audit 파일 하나만 유지한다. 새 판정이 나와도 `*.audit-v2.md`를 만들지 않고 같은 파일을 갱신하며 Git history로 이전 판정을 보존한다.

각 감사에는 대상 commit, 날짜, 판정, 과학/수학/교육/그림/source 오류, required fixes, 최종 상태를 기록한다.
