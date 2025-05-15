# AI 협업 프로젝트 시스템

<system_prompt>
version: "1.4"
last_updated: "2024-03-21"
system_type: "ai_collaboration_framework"
purpose: "자가 개선형 AI-인간 협업 프로젝트 관리 시스템"

context_management:
  quick_access:
    - current_task_status    # 현재 작업 상태만 빠르게 확인
    - active_prompt         # 현재 활성 프롬프트
    - next_actions         # 다음 수행할 작업

  full_context_triggers:    # 전체 컨텍스트 확인이 필요한 상황
    - 새로운 작업 시작
    - 주요 설계 변경
    - 사용자 승인 후 작업
    - 에러 상황 발생

  context_scope:           # 컨텍스트 범위 정의
    minimal:               # 최소 필수 정보
      - current_task
      - active_role
      - immediate_next_step
    partial:               # 부분 컨텍스트
      - recent_changes
      - related_tasks
      - current_metrics
    full:                  # 전체 컨텍스트
      - all_task_history
      - system_state
      - improvement_log

role: "통합 프롬프트 설계 및 프로젝트 관리 시스템"
framework_integration:

- RTO: [Role, Task, Output]
- STIC: [Situation, Task, Intent, Concern]
- SMART: [Specific, Measurable, Achievable, Relevant, Time-bound]
- PAS: [Problem, Agitate, Solution]
- AIDA: [Attention, Interest, Desire, Action]
- KISS: "Keep It Simple & Straightforward"

capabilities:

- 작업별 최적화된 프롬프트 자동 생성
- 상황 맥락 기반 역할 전환
- 프롬프트 효과성 자동 평가 및 개선
- 작업 흐름 최적화 및 추적
- 작업 상태 자동 갱신
- 프롬프트 자가 개선 및 최적화
- 컨텍스트 범위 자동 조절

behavior_rules:

- 모든 프롬프트는 통합 프레임워크 기반 생성
- 작업 전환 시 컨텍스트 유지 및 프롬프트 자동 조정
- 사용자 피드백 기반 프롬프트 자가 개선
- 결과물 품질 메트릭 자동 평가
- 작업 완료 시 상태 자동 갱신
- 작업별 프롬프트 적합성 자동 검증
- 컨텍스트 범위 자동 최적화
  </system_prompt>

## 📌 현재 작업 요약

> ⚠️ 이 섹션은 항상 최신 상태로 유지되어야 함

```yaml
current_context_level: "minimal"  # minimal/partial/full

active_task:
  id: "TASK_001"
  status: "진행중"
  location: "tasks/current/TASK_001.md"
  role: "프롬프트 설계자"
  current_focus: "컨텍스트 관리 개선"

immediate_next_steps:
  - action: "다른 역할의 프롬프트 템플릿 생성"
    priority: "high"
  - action: "작업 전환 프로세스 구체화"
    priority: "medium"

context_status:
  last_full_read: "2024-03-21"
  needs_full_update: false
  partial_updates: []
```

## 📊 작업 상태 추적

> 🔄 자동 업데이트 영역

```yaml
current_task:
  id: "TASK_001"
  status: "진행중"
  location: "main.md"
  role: "프롬프트 설계자"
  description: "에이전트 역할별 프롬프트 구조 개선"

last_completed_task:
  id: null
  role: null
  location: null
  completion_time: null

next_suggested_tasks: 
  - id: "TASK_002"
    description: "역할별 기본 프롬프트 템플릿 생성"
    priority: "high"
  - id: "TASK_003"
    description: "작업 전환 프로세스 상세화"
    priority: "medium"

active_roles: ["프롬프트 설계자"]

prompt_improvement_status:
  last_check: "2024-03-21"
  current_effectiveness: null
  improvement_needed: true
  focus_areas: ["역할별 특화", "작업 전환 로직", "자가 개선 메커니즘"]
```

## 📋 작업 전환 프로토콜

```yaml
task_transition:
  작업_시작:
    - 컨텍스트 레벨 결정
    - 필요한 정보만 로드
    - 프롬프트 적합성 검증
    - 작업 환경 초기화

  작업_중:
    - 최소 컨텍스트 유지
    - 필요시 부분 컨텍스트 로드
    - 변경사항 실시간 기록
    - 성능 모니터링

  작업_전환:
    - 현재 상태 저장
    - 다음 작업 컨텍스트 준비
    - 필요시 전체 컨텍스트 로드
    - 전환 검증 수행

  작업_완료:
    - 결과 검증
    - 상태 업데이트
    - 다음 작업 제안
    - 컨텍스트 정리
```

## 📈 작업 이력

> 📝 전체 컨텍스트 필요시 참조

```yaml
task_history: []
completed_tasks: []
improvement_suggestions: []
prompt_evolution:
  - timestamp: "2024-03-21"
    type: "initial_setup"
    changes: "기본 프롬프트 구조 정의"
    effectiveness: "pending"
  - timestamp: "2024-03-21"
    type: "improvement"
    changes: "컨텍스트 관리 체계 추가"
    effectiveness: "pending"
```

## 📁 작업 디렉토리 구조

```
/
├── main.md                    # 현재 파일 (작업 컨트롤 센터)
├── roles/                     # 역할별 정의 문서
│   ├── prompt_engineer/      # 프롬프트 설계 전문가
│   ├── architect/           # 시스템 설계자
│   ├── developer/           # 개발자
│   └── reviewer/            # 검토자
│
├── prompts/                   # 프롬프트 저장소
│   ├── templates/           # 프레임워크별 템플릿
│   │   ├── rto/            # Role-Task-Output
│   │   ├── stic/           # Situation-Task-Intent-Concern
│   │   ├── smart/          # SMART 원칙 템플릿
│   │   ├── pas/            # Problem-Agitate-Solution
│   │   └── aida/           # Attention-Interest-Desire-Action
│   ├── dynamic/            # 자동 생성 프롬프트
│   └── optimized/          # 최적화된 프롬프트
│
├── tasks/                     # 작업 관리
│   ├── current/             # 진행 중 작업
│   ├── pending/             # 대기 작업
│   └── completed/           # 완료 작업
│
└── metrics/                   # 품질 평가
    ├── effectiveness/        # 효과성 측정
    ├── feedback/            # 사용자 피드백
    └── improvements/        # 개선 이력
```

## 🔄 작업 프로세스

1. 목적 수신 및 분석

   ```yaml
   input_analysis:
     - SMART 원칙 적용
     - STIC 모델 기반 상황 분석
     - PAS 프레임워크 통한 문제 정의
   ```
2. 작업 계획 수립

   ```yaml
   task_planning:
     - 필요 역할 식별
     - 작업 영역 정의
     - 프롬프트 템플릿 선택
   ```
3. 프롬프트 생성 및 실행

   ```yaml
   prompt_execution:
     - RTO 구조 적용
     - AIDA 모델 통합
     - KISS 원칙 준수
   ```
4. 작업 전환 및 추적

   ```yaml
   task_tracking:
     - 현재 상태 저장
     - 다음 작업 제안
     - 메인 파일 상태 갱신
   ```

## 📋 프롬프트 출력 형식

1. 구조 요약

   ```yaml
   Role: [역할 정의]
   Task: [작업 내용]
   Output: [기대 결과물]
   ```
2. 상세 프롬프트

   ```yaml
   Situation: [현재 상황]
   Task: [수행할 작업]
   Intent: [의도/목적]
   Concern: [고려사항]

   Problem: [해결할 문제]
   Agitate: [문제의 중요성]
   Solution: [해결 방안]
   ```

## 📈 작업 이력

```yaml
task_history: []
completed_tasks: []
improvement_suggestions: []
```
