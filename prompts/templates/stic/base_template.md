# STIC (Situation-Task-Intent-Concern) 기본 템플릿

<template_meta>
version: "1.0"
framework: "STIC"
purpose: "상황 기반 작업 의도 및 고려사항 정의"
</template_meta>

## 기본 구조

```yaml
Situation:
  context: "[현재 상황 설명]"
  background: "[배경 정보]"
  resources: "[가용 자원]"
  constraints: "[제약 조건]"

Task:
  description: "[수행할 작업]"
  scope: "[작업 범위]"
  timeline: "[시간 계획]"
  dependencies: "[의존성]"

Intent:
  objective: "[목적]"
  expected_outcome: "[기대 결과]"
  success_criteria: "[성공 기준]"
  impact: "[영향도]"

Concern:
  risks: "[위험 요소]"
  challenges: "[도전 과제]"
  mitigation: "[대응 방안]"
  monitoring: "[모니터링 계획]"
```

## 사용 지침

1. Situation 분석
   - 현재 상황의 명확한 이해
   - 관련 배경 정보 수집
   - 가용 자원 및 제약 조건 파악

2. Task 정의
   - 구체적인 작업 내용 명시
   - 명확한 범위 설정
   - 시간 계획 수립

3. Intent 명확화
   - 작업의 궁극적 목적 정의
   - 구체적인 성공 기준 설정
   - 기대 효과 명시

4. Concern 관리
   - 잠재적 위험 식별
   - 구체적 대응 방안 수립
   - 모니터링 계획 수립 