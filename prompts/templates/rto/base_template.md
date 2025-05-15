# RTO (Role-Task-Output) 기본 템플릿

<template_meta>
version: "1.0"
framework: "RTO"
purpose: "역할 기반 작업 정의 및 산출물 명세"
</template_meta>

## 기본 구조

```yaml
Role:
  title: "[역할 제목]"
  expertise: "[전문 분야]"
  responsibility: "[주요 책임]"
  authority: "[권한 범위]"

Task:
  objective: "[작업 목표]"
  scope: "[작업 범위]"
  constraints: "[제약 사항]"
  dependencies: "[의존성]"

Output:
  deliverables: "[산출물 목록]"
  quality_criteria: "[품질 기준]"
  format: "[형식]"
  acceptance_criteria: "[승인 기준]"
```

## 사용 지침

1. Role 정의
   - 명확한 역할 책임과 권한 정의
   - 필요한 전문성 명시
   - 다른 역할과의 관계 설정

2. Task 명세
   - 구체적이고 측정 가능한 목표 설정
   - 명확한 작업 범위 정의
   - 제약사항과 의존성 명시

3. Output 정의
   - 구체적인 산출물 형식 지정
   - 명확한 품질 기준 설정
   - 검증 가능한 승인 기준 제시 