# MacBook 코딩 10가지 팁 — 상세 가이드 작성 플랜

## TL;DR

> **Quick Summary**: MacBook에서 코딩 생산성을 극대화하는 10가지 방법을 한국어 상세 가이드로 작성. Mac 환경 최적화 + AI 도구(VS Code, Open Code, Open Spec, Gemini/Claude/ChatGPT) 워크플로우를 균형 있게 다룸.
> 
> **Deliverables**:
> - `README.md` — 프로젝트 루트에 10가지 팁 상세 가이드 (5,000~10,000 단어)
> 
> **Estimated Effort**: Medium
> **Parallel Execution**: YES — 4 waves (Wave 2에서 3개 병렬 작성)
> **Critical Path**: git init → 스켈레톤 → 콘텐츠 병렬 작성 → 통합 → QA

---

## Context

### Original Request
MacBook에서 코딩을 잘하는 10가지 방법을 정리. 사용 도구: VS Code, Open Code, Open Spec. 연동 AI 모델: Gemini, Claude, ChatGPT.

### Interview Summary
**Key Discussions**:
- **독자**: 본인 개인 레퍼런스 (캐주얼하지만 정보성 있는 톤)
- **깊이**: 팁당 1페이지 이상 상세 가이드 (구체적 설정법, 명령어, 예제 포함)
- **언어**: 한국어 (기술 용어는 영어 유지)
- **형식**: 단일 README.md 파일, 프로젝트 루트
- **AI 모델**: Gemini, Claude, ChatGPT 3개 (Anthropic은 Claude와 중복이므로 제외)
- **초점**: Mac 환경 최적화 + AI 코딩 워크플로우 균형

**Research Findings**:
- 프로젝트에 OpenSpec, OpenCode (Claude/Gemini/Codex 설정), VS Code 설정이 이미 존재
- 프로젝트에 아직 콘텐츠 없음 — 이것이 첫 번째 산출물
- Git 저장소 미초기화 상태 (`git init` 필요)
- 프로젝트에 bun/node 설정 있음 → 코드 예제는 TypeScript/Bash 사용

### Metis Review
**Identified Gaps** (addressed):
- Mac 하드웨어 타입 미확인 → Apple Silicon(M시리즈) 가정 (2026년 기준 합리적)
- macOS 버전 미확인 → 최신 macOS 가정
- 코드 예제 언어 미확인 → TypeScript/Bash 사용 (프로젝트 설정 기반)
- TOC 필요 여부 미확인 → 필수 포함 (10개 섹션 가이드에 네비게이션 필수)
- 스크린샷 처리 방법 미확인 → 텍스트 전용 (유지보수 용이)
- Open Code/Open Spec 명령어 정확성 → 프로젝트 파일에서 검증 필요
- 섹션별 분량 기준 → 300~800 단어로 설정
- 단일 파일 병렬 쓰기 충돌 → 순차 처리로 해결

---

## Work Objectives

### Core Objective
MacBook에서 코딩 생산성을 극대화하는 10가지 실용 팁을 한국어 상세 가이드로 작성하여 `README.md`에 저장한다.

### Concrete Deliverables
- `/Users/chance/workspace/mac-tips/README.md` — 10가지 팁 상세 가이드 (한국어, 5,000~10,000 단어)
- Git 저장소 초기화 및 깔끔한 커밋 히스토리

### Definition of Done
- [x] README.md 파일이 프로젝트 루트에 존재
- [x] 정확히 10개의 `##` 레벨 토픽 섹션 포함
- [x] 목차(TOC)와 앵커 링크 포함
- [x] 모든 코드 블록에 언어 태그 존재 (미태그 코드 블록 0개)
- [x] 전체 단어 수 5,000~10,000
- [x] 각 섹션에 최소 1개 코드 블록 포함
- [x] Mac 키보드 표기법 사용 (⌘⌥⌃⇧), Windows 표기 없음
- [x] 자연스러운 한국어 (기술 용어는 영어 유지)

### Must Have
- 10개 토픽 모두 상세 콘텐츠 포함
- 각 섹션에 실행 가능한 명령어/설정 예제
- 목차와 섹션 간 크로스 레퍼런스
- "마지막 업데이트" 날짜 헤더
- 일관된 섹션 템플릿 구조 (소개 → 서브섹션 → 실용 예제 → 💡 팁)

### Must NOT Have (Guardrails)
- **Open Code/Open Spec 기능 날조 금지** — 프로젝트 파일에서 검증된 명령어만 사용
- **Windows 키보드 표기 금지** — Ctrl+, Alt+, Cmd+ 대신 ⌘⌥⌃⇧ 사용
- **VS Code 확장 10개 초과 금지** — 실제 워크플로우에 필요한 것만 엄선
- **Homebrew 도구 10개 초과 금지** — 핵심 CLI 도구만 추천
- **키보드 단축키 20개 초과 금지** — 코딩 관련 생산성 단축키만
- **영어 본문 금지** — 기술 용어와 코드 외에는 한국어로 작성
- **스크린샷/이미지 참조 금지** — 텍스트 전용 가이드
- **특정 프로그래밍 언어 튜토리얼 금지** — 도구/환경 활용법에 집중
- **형식적/학술적 한국어 톤 금지** — 개인 레퍼런스에 맞는 캐주얼하지만 정보성 있는 톤

---

## Verification Strategy (MANDATORY)

> **ZERO HUMAN INTERVENTION** — ALL verification is agent-executed. No exceptions.

### Test Decision
- **Infrastructure exists**: NO (writing task — 단위 테스트 해당 없음)
- **Automated tests**: None (콘텐츠 검증은 QA 시나리오로 대체)
- **Framework**: N/A

### QA Policy
모든 태스크는 agent-executed QA 시나리오를 포함. 콘텐츠 작성 태스크의 경우:
- **구조 검증**: grep/wc 명령어로 섹션 수, 코드 블록 태그, 단어 수 확인
- **정확성 검증**: 언급된 명령어/도구의 실존 여부 확인
- **형식 검증**: Mac 표기법, 마크다운 문법 확인
- Evidence: `.sisyphus/evidence/task-{N}-{scenario-slug}.txt`

---

## Execution Strategy

### Parallel Execution Waves

```
Wave 0 (Pre-requisite):
└── Task 0: Git 저장소 초기화 [quick]

Wave 1 (After Wave 0 — 스켈레톤):
└── Task 1: README.md 스켈레톤 생성 (TOC + 10개 섹션 헤더 + 템플릿) [quick]

Wave 2 (After Wave 1 — 콘텐츠 병렬 작성):
├── Task 2: Topics 1,2,7,10 — Mac 환경 그룹 [writing]
├── Task 3: Topics 3,4,5 — AI 도구 그룹 [writing]
└── Task 4: Topics 6,8,9 — AI 실전 활용 그룹 [writing]
⚠️ 동일 파일 병렬 쓰기 충돌 → Task 2→3→4 순차 실행

Wave 3 (After Wave 2 — 통합 & 폴리시):
└── Task 5: 통합, 크로스 레퍼런스, 일관성 검토 [unspecified-low]

Wave 4 (After Wave 3 — QA):
└── Task 6: 수용 기준 검증 및 수정 [quick]

Wave FINAL (After ALL tasks — 최종 검증):
├── Task F1: 플랜 준수 감사 [oracle]
├── Task F2: 마크다운 품질 리뷰 [unspecified-high]
├── Task F3: 콘텐츠 QA [unspecified-high]
└── Task F4: 범위 충실도 검사 [deep]
→ 결과 제시 → 사용자 명시적 확인 대기

Critical Path: Task 0 → Task 1 → Task 2 → Task 3 → Task 4 → Task 5 → Task 6 → F1-F4 → user okay
Parallel Speedup: Wave 2 내 순차이므로 속도 이점 제한적. Wave FINAL에서 4개 병렬 검증으로 보완.
Max Concurrent: 4 (Wave FINAL)
```

### Dependency Matrix

| Task | Depends On | Blocks | Wave |
|------|-----------|--------|------|
| 0 | — | 1 | 0 |
| 1 | 0 | 2, 3, 4 | 1 |
| 2 | 1 | 3 (파일 충돌) | 2 |
| 3 | 1, 2 (파일 충돌) | 4 (파일 충돌) | 2 |
| 4 | 1, 3 (파일 충돌) | 5 | 2 |
| 5 | 2, 3, 4 | 6 | 3 |
| 6 | 5 | F1-F4 | 4 |
| F1-F4 | 6 | — (사용자 확인) | FINAL |

### Agent Dispatch Summary

- **Wave 0**: **1** — T0 → `quick` + `git-master`
- **Wave 1**: **1** — T1 → `quick`
- **Wave 2**: **3** (순차) — T2 → `writing`, T3 → `writing`, T4 → `writing`
- **Wave 3**: **1** — T5 → `unspecified-low`
- **Wave 4**: **1** — T6 → `quick` + `git-master`
- **FINAL**: **4** (병렬) — F1 → `oracle`, F2 → `unspecified-high`, F3 → `unspecified-high`, F4 → `deep`

---

## TODOs

- [x] 0. Git 저장소 초기화

  **What to do**:
  - `/Users/chance/workspace/mac-tips`에서 `git init` 실행
  - `.gitignore` 파일 생성: `node_modules/`, `.DS_Store`, `.sisyphus/evidence/` 포함
  - 초기 커밋 없이 저장소만 초기화

  **Must NOT do**:
  - 원격 저장소 추가 금지
  - 초기 커밋 생성 금지 (Task 1에서 스켈레톤과 함께 커밋)

  **Recommended Agent Profile**:
  - **Category**: `quick`
  - **Skills**: [`git-master`]
    - `git-master`: Git 초기화 및 설정 전문

  **Parallelization**:
  - **Can Run In Parallel**: NO
  - **Parallel Group**: Wave 0 (단독)
  - **Blocks**: Task 1
  - **Blocked By**: None

  **References**:
  - 프로젝트 루트: `/Users/chance/workspace/mac-tips/`
  - 기존 `.opencode/.gitignore` 참고 가능

  **Acceptance Criteria**:

  **QA Scenarios:**

  ```
  Scenario: Git 저장소 초기화 확인
    Tool: Bash
    Preconditions: /Users/chance/workspace/mac-tips 디렉토리 존재
    Steps:
      1. `git init` 실행
      2. `git status` 실행 — "On branch main" 또는 "On branch master" 메시지 확인
      3. `.gitignore` 파일 생성 확인: `test -f .gitignore && echo "PASS"`
      4. `.gitignore`에 `node_modules/`, `.DS_Store` 포함 확인: `grep "node_modules" .gitignore`
    Expected Result: Git 저장소 초기화됨, .gitignore 존재
    Failure Indicators: `git status` 실행 시 "not a git repository" 에러
    Evidence: .sisyphus/evidence/task-0-git-init.txt
  ```

  **Commit**: NO (Task 1에서 함께 커밋)

---

- [x] 1. README.md 스켈레톤 생성 (TOC + 섹션 구조 + 템플릿)

  **What to do**:
  - `/Users/chance/workspace/mac-tips/README.md` 생성
  - 제목: `# MacBook에서 코딩을 잘하는 10가지 방법`
  - "마지막 업데이트: 2026년 3월" 표기
  - 간단한 소개 문단 (2~3문장)
  - 목차 (TOC): 10개 토픽에 대한 앵커 링크
  - 10개 `##` 섹션 헤더 생성 (각 토픽별):
    1. `## 1. Mac 개발 환경 기초 세팅`
    2. `## 2. VS Code Mac 최적화`
    3. `## 3. Open Code 완전 정복`
    4. `## 4. Open Spec 스펙 기반 개발`
    5. `## 5. AI 모델 전략적 선택법`
    6. `## 6. AI 프롬프트 엔지니어링 for 코딩`
    7. `## 7. Mac 키보드 & 생산성 해킹`
    8. `## 8. Git 워크플로우 + AI 연동`
    9. `## 9. 디버깅 & 문제 해결에 AI 활용`
    10. `## 10. Mac 개발 환경 유지보수`
  - 각 섹션 내부에 일관된 템플릿 구조:
    - 소개 문단 영역
    - 2~3개 `###` 서브섹션 헤더 (토픽에 맞게)
    - `<!-- CONTENT: Topic N -->` 플레이스홀더 마커
    - `> 💡 **팁:**` 콜아웃 영역
  - 마지막에 간단한 "마치며" 섹션 헤더

  **Must NOT do**:
  - 실제 콘텐츠 작성 금지 — 구조와 플레이스홀더만
  - 이미지/스크린샷 참조 금지

  **Recommended Agent Profile**:
  - **Category**: `quick`
  - **Skills**: []
    - 단순 파일 생성 작업이므로 특별한 스킬 불필요

  **Parallelization**:
  - **Can Run In Parallel**: NO
  - **Parallel Group**: Wave 1 (단독)
  - **Blocks**: Tasks 2, 3, 4
  - **Blocked By**: Task 0

  **References**:
  **Pattern References**:
  - GitHub의 일반적인 README.md 구조 참고 (title → TOC → sections)

  **Acceptance Criteria**:

  **QA Scenarios:**

  ```
  Scenario: 스켈레톤 구조 검증
    Tool: Bash
    Preconditions: Task 0 완료 (git init됨)
    Steps:
      1. `test -f /Users/chance/workspace/mac-tips/README.md` — 파일 존재 확인
      2. `grep -c "^## " README.md` — 10개 이상 (10 토픽 + 마치며)
      3. `grep -c "<!-- CONTENT" README.md` — 정확히 10 (각 토픽별 플레이스홀더)
      4. `grep "마지막 업데이트" README.md` — 날짜 포함 확인
      5. `grep -c "^### " README.md` — 20개 이상 (각 토픽 2~3개 서브섹션)
      6. `grep "목차" README.md` 또는 `grep "Table of Contents" README.md` — TOC 존재
    Expected Result: 파일 존재, 10개 토픽 섹션, 10개 플레이스홀더, TOC 포함
    Failure Indicators: 섹션 수 10 미만, 플레이스홀더 누락, TOC 없음
    Evidence: .sisyphus/evidence/task-1-skeleton-verify.txt

  Scenario: 마크다운 형식 검증
    Tool: Bash
    Preconditions: README.md 생성됨
    Steps:
      1. `awk '/^```$/{c++} END{print c+0}' README.md` — 0 (미태그 코드 블록 없음, 스켈레톤에는 코드 블록 자체가 없어야 함). 참고: macOS 기본 grep은 `-P` 미지원이므로 awk 사용.
      2. 헤딩 레벨 확인: `#` → `##` → `###` 순서 (레벨 점프 없음)
    Expected Result: 깨끗한 마크다운 구조
    Evidence: .sisyphus/evidence/task-1-markdown-verify.txt
  ```

  **Commit**: YES
  - Message: `docs: add README skeleton with TOC and section structure`
  - Files: `README.md`, `.gitignore`
  - Pre-commit: `grep -c "^## " README.md` (10+ 확인)

---

- [x] 2. 콘텐츠 작성 — Topics 1, 2, 7, 10 (Mac 환경 그룹)

  **What to do**:
  README.md의 해당 섹션 플레이스홀더를 실제 한국어 콘텐츠로 교체.

  **Topic 1 — Mac 개발 환경 기초 세팅** (300~800 단어):
  - Homebrew 설치: `/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"`
  - Apple Silicon 경로: `/opt/homebrew` 설명
  - 필수 CLI 도구 (최대 10개): git, node, bun, python, fzf, ripgrep, jq, bat, eza, fd
  - Zsh + Oh My Zsh 설정
  - 유용한 alias 예제 (3~5개)
  - 터미널 앱 추천 (iTerm2 또는 Warp)

  **Topic 2 — VS Code Mac 최적화** (300~800 단어):
  - `settings.json` 핵심 설정 (5~8개, 코드 블록으로)
  - 필수 확장 프로그램 (최대 10개, 한국어 설명)
  - Mac 전용 단축키 (⌘⌥⌃⇧ 표기): ⌘P, ⌘⇧P, ⌘B, ⌘J 등
  - 워크스페이스 설정 팁

  **Topic 7 — Mac 키보드 & 생산성 해킹** (300~800 단어):
  - 윈도우 관리: Rectangle 또는 Raycast
  - 런처: Alfred 또는 Raycast
  - 코딩 관련 단축키 15~20개 (⌘⌥⌃⇧ 표기)
  - 한영 전환 팁
  - Mission Control / Spaces 활용

  **Topic 10 — Mac 개발 환경 유지보수** (300~800 단어):
  - `brew update && brew upgrade && brew cleanup` 루틴
  - VS Code 설정 동기화 (Settings Sync)
  - dotfiles 백업 전략 (git으로 관리)
  - 디스크 정리 팁
  - macOS 업데이트 시 개발 환경 대응

  **각 섹션 공통 요구사항**:
  - 300~800 단어
  - 최소 1개 코드 블록 (언어 태그 필수)
  - `> 💡 **팁:**` 콜아웃으로 마무리
  - 자연스러운 한국어 (캐주얼하지만 정보성 있는 톤)
  - `<!-- CONTENT: Topic N -->` 플레이스홀더 제거

  **Must NOT do**:
  - Homebrew 도구 10개 초과 나열 금지
  - VS Code 확장 10개 초과 나열 금지
  - 키보드 단축키 20개 초과 나열 금지
  - Windows 표기법(Ctrl+, Alt+, Cmd+) 사용 금지
  - 스크린샷/이미지 참조 금지
  - 폐기된(deprecated) 도구/설정 언급 금지

  **Recommended Agent Profile**:
  - **Category**: `writing`
    - Reason: 기술 문서 콘텐츠 작성 작업
  - **Skills**: []
  - **Skills Evaluated but Omitted**:
    - `frontend-ui-ux`: 이 작업은 UI가 아닌 문서 작성

  **Parallelization**:
  - **Can Run In Parallel**: NO (동일 파일 편집 충돌)
  - **Parallel Group**: Wave 2 (Task 2 → 3 → 4 순차)
  - **Blocks**: Task 3 (파일 충돌), Task 5 (콘텐츠 완성)
  - **Blocked By**: Task 1

  **References**:
  **Pattern References**:
  - Task 1에서 생성한 README.md 스켈레톤 구조를 따를 것
  - 각 섹션의 `###` 서브섹션 헤더를 유지하면서 콘텐츠 추가

  **Acceptance Criteria**:

  **QA Scenarios:**

  ```
  Scenario: Topic 1,2,7,10 콘텐츠 존재 확인
    Tool: Bash
    Preconditions: Task 1 완료 (스켈레톤 존재)
    Steps:
      1. `grep "<!-- CONTENT: Topic 1 -->" README.md` — 결과 없어야 함 (플레이스홀더 제거됨)
      2. `grep "<!-- CONTENT: Topic 2 -->" README.md` — 결과 없어야 함
      3. `grep "<!-- CONTENT: Topic 7 -->" README.md` — 결과 없어야 함
      4. `grep "<!-- CONTENT: Topic 10 -->" README.md` — 결과 없어야 함
      5. `grep "Homebrew" README.md` — 결과 있어야 함 (Topic 1 콘텐츠 존재)
      6. `grep "settings.json" README.md` — 결과 있어야 함 (Topic 2 콘텐츠 존재)
    Expected Result: 4개 토픽의 플레이스홀더 모두 제거, 실제 콘텐츠 존재
    Failure Indicators: 플레이스홀더가 남아있음, 핵심 키워드 부재
    Evidence: .sisyphus/evidence/task-2-content-verify.txt

  Scenario: Mac 표기법 및 코드 블록 검증
    Tool: Bash
    Preconditions: 콘텐츠 작성 완료
    Steps:
      1. `grep -c "Ctrl+" README.md` — 0이어야 함
      2. `grep -c "Cmd+" README.md` — 0이어야 함
      3. `grep "⌘" README.md` — 결과 있어야 함 (Mac 표기 사용 중)
      4. `awk '/^```$/{c++} END{print c+0}' README.md` — 0이어야 함 (모든 코드 블록 태그됨). macOS 호환 명령어.
    Expected Result: Windows 표기 없음, Mac 표기 사용, 코드 블록 모두 태그됨
    Evidence: .sisyphus/evidence/task-2-format-verify.txt
  ```

  **Commit**: NO (Task 5에서 통합 후 함께 커밋)

---

- [x] 3. 콘텐츠 작성 — Topics 3, 4, 5 (AI 도구 그룹)

  **What to do**:
  README.md의 해당 섹션 플레이스홀더를 실제 한국어 콘텐츠로 교체.

  **Topic 3 — Open Code 완전 정복** (300~800 단어):
  - Open Code란 무엇인가 (간단 소개)
  - 설치 및 기본 설정
  - 핵심 슬래시 커맨드 — **반드시 프로젝트 `.opencode/` 디렉토리에서 실제 존재하는 커맨드만 기술**:
    - `/opsx-propose`, `/opsx-apply`, `/opsx-archive`, `/opsx-explore` (`.opencode/command/` 확인)
  - 에이전트 타입 설명 (explore, librarian 등)
  - 실전 워크플로우 예시 (구체적 시나리오)

  **Topic 4 — Open Spec 스펙 기반 개발** (300~800 단어):
  - Open Spec이란 (spec-driven 개발의 장점)
  - 4단계 워크플로우: 탐색(explore) → 제안(propose) → 구현(apply) → 아카이브(archive)
  - 각 단계 예시 명령어 — **반드시 프로젝트 `openspec/` 디렉토리 및 `.opencode/command/` 에서 검증**
  - `openspec/config.yaml` 설정 설명
  - 스펙 기반 개발의 실전 이점

  **Topic 5 — AI 모델 전략적 선택법** (300~800 단어):
  - 3개 모델 비교표: Gemini vs Claude vs ChatGPT
    - 강점/약점
    - 코딩 작업별 추천 (코드 생성, 디버깅, 리팩토링, 아키텍처)
    - 비용/속도 고려사항
  - 상황별 모델 선택 가이드 (간단한 플로우차트 형태)
  - 실전 조합 전략 (여러 모델 함께 활용하는 법)

  **각 섹션 공통 요구사항**: (Task 2와 동일)

  **Must NOT do**:
  - **Open Code/Open Spec 기능 날조 절대 금지** — 프로젝트 파일에서 검증된 것만 기술
  - AI 모델 벤치마크 수치 날조 금지 — 일반적인 특성 비교만
  - 미확인 슬래시 커맨드 기술 금지

  **Recommended Agent Profile**:
  - **Category**: `writing`
    - Reason: 기술 문서 콘텐츠 작성 + 프로젝트 파일 참조 필요
  - **Skills**: []

  **Parallelization**:
  - **Can Run In Parallel**: NO (동일 파일 편집 충돌)
  - **Parallel Group**: Wave 2 (Task 2 → 3 → 4 순차)
  - **Blocks**: Task 4 (파일 충돌), Task 5 (콘텐츠 완성)
  - **Blocked By**: Task 1, Task 2 (파일 충돌)

  **References**:
  **Pattern References**:
  - Task 1에서 생성한 README.md 스켈레톤 구조를 따를 것

  **API/Type References** (CRITICAL — Open Code 커맨드 검증):
  - `.opencode/command/opsx-explore.md` — explore 커맨드 정의
  - `.opencode/command/opsx-propose.md` — propose 커맨드 정의
  - `.opencode/command/opsx-apply.md` — apply 커맨드 정의
  - `.opencode/command/opsx-archive.md` — archive 커맨드 정의
  - `openspec/config.yaml` — Open Spec 설정 구조

  **WHY Each Reference Matters**:
  - `.opencode/command/*.md`: Open Code 슬래시 커맨드의 실제 정의를 확인하여 날조 방지. 각 파일에서 커맨드 이름, 설명, 사용법을 추출할 것.
  - `openspec/config.yaml`: Open Spec의 실제 설정 구조를 보여줌. `schema: spec-driven` 등의 실제 값을 가이드에 반영.

  **Acceptance Criteria**:

  **QA Scenarios:**

  ```
  Scenario: Topic 3,4,5 콘텐츠 존재 확인
    Tool: Bash
    Preconditions: Task 2 완료
    Steps:
      1. `grep "<!-- CONTENT: Topic 3 -->" README.md` — 결과 없어야 함
      2. `grep "<!-- CONTENT: Topic 4 -->" README.md` — 결과 없어야 함
      3. `grep "<!-- CONTENT: Topic 5 -->" README.md` — 결과 없어야 함
      4. `grep "Open Code" README.md` — 결과 있어야 함 (Topic 3)
      5. `grep "Open Spec" README.md` — 결과 있어야 함 (Topic 4)
      6. `grep "Gemini" README.md && grep "Claude" README.md && grep "ChatGPT" README.md` — 3개 모델 모두 언급
    Expected Result: 3개 토픽 플레이스홀더 제거, 실제 콘텐츠 존재, 3개 AI 모델 모두 언급
    Evidence: .sisyphus/evidence/task-3-content-verify.txt

  Scenario: Open Code 커맨드 정확성 검증
    Tool: Bash
    Preconditions: 콘텐츠 작성 완료
    Steps:
      1. README.md에서 언급된 Open Code 슬래시 커맨드 목록 추출
      2. `.opencode/command/` 디렉토리의 실제 파일 목록과 대조
      3. README.md에 언급되었지만 실제 존재하지 않는 커맨드가 있으면 FAIL
    Expected Result: README.md의 모든 Open Code 커맨드가 프로젝트 파일에 실존
    Failure Indicators: 존재하지 않는 커맨드 언급
    Evidence: .sisyphus/evidence/task-3-command-verify.txt
  ```

  **Commit**: NO (Task 5에서 통합 후 함께 커밋)

---

- [x] 4. 콘텐츠 작성 — Topics 6, 8, 9 (AI 실전 활용 그룹)

  **What to do**:
  README.md의 해당 섹션 플레이스홀더를 실제 한국어 콘텐츠로 교체.

  **Topic 6 — AI 프롬프트 엔지니어링 for 코딩** (300~800 단어):
  - 코딩 전용 프롬프트 패턴 5~7개:
    - 버그 수정 프롬프트
    - 리팩토링 프롬프트
    - 코드 설명 프롬프트
    - 테스트 생성 프롬프트
    - 아키텍처 설계 프롬프트
  - Before/After 예시: 모호한 프롬프트 vs 구체적 프롬프트
  - 각 패턴별 템플릿 형식

  **Topic 8 — Git 워크플로우 + AI 연동** (300~800 단어):
  - AI 기반 커밋 메시지 작성 (Conventional Commits 형식)
  - AI 코드 리뷰 워크플로우
  - AI를 활용한 머지 충돌 해결
  - 브랜치 네이밍 + AI
  - Git hooks + AI 통합 팁

  **Topic 9 — 디버깅 & 문제 해결에 AI 활용** (300~800 단어):
  - 에러 메시지 → AI 워크플로우 (복붙 패턴)
  - 로그 분석에 AI 활용
  - AI와의 러버덕 디버깅
  - 스택 트레이스 해석
  - 성능 디버깅 프롬프트

  **각 섹션 공통 요구사항**: (Task 2와 동일)

  **Must NOT do**:
  - 프롬프트 엔지니어링 이론서 작성 금지 — 실용 패턴만
  - 모든 Git 브랜치 전략 설명 금지 — AI 연동 부분만
  - 디버깅 도구 10개 이상 나열 금지

  **Recommended Agent Profile**:
  - **Category**: `writing`
    - Reason: 기술 문서 콘텐츠 작성 작업
  - **Skills**: []

  **Parallelization**:
  - **Can Run In Parallel**: NO (동일 파일 편집 충돌)
  - **Parallel Group**: Wave 2 (Task 2 → 3 → 4 순차)
  - **Blocks**: Task 5 (콘텐츠 완성)
  - **Blocked By**: Task 1, Task 3 (파일 충돌)

  **References**:
  **Pattern References**:
  - Task 1에서 생성한 README.md 스켈레톤 구조를 따를 것

  **Acceptance Criteria**:

  **QA Scenarios:**

  ```
  Scenario: Topic 6,8,9 콘텐츠 존재 확인
    Tool: Bash
    Preconditions: Task 3 완료
    Steps:
      1. `grep "<!-- CONTENT: Topic 6 -->" README.md` — 결과 없어야 함
      2. `grep "<!-- CONTENT: Topic 8 -->" README.md` — 결과 없어야 함
      3. `grep "<!-- CONTENT: Topic 9 -->" README.md` — 결과 없어야 함
      4. `grep "프롬프트" README.md` — 결과 있어야 함 (Topic 6)
      5. `grep -i "git" README.md` — 결과 있어야 함 (Topic 8)
      6. `grep "디버깅" README.md` — 결과 있어야 함 (Topic 9)
    Expected Result: 3개 토픽 플레이스홀더 제거, 실제 콘텐츠 존재
    Evidence: .sisyphus/evidence/task-4-content-verify.txt

  Scenario: 프롬프트 패턴 예시 품질 확인
    Tool: Bash
    Preconditions: Topic 6 콘텐츠 작성 완료
    Steps:
      1. Topic 6 섹션 내 코드 블록 수 확인 — 최소 3개 (프롬프트 템플릿)
      2. Before/After 패턴 존재 확인: "Before" 또는 "모호한" 과 "After" 또는 "구체적" 키워드 검색
    Expected Result: 코드 블록 3개 이상, Before/After 비교 예시 존재
    Evidence: .sisyphus/evidence/task-4-prompt-quality.txt
  ```

  **Commit**: NO (Task 5에서 통합 후 함께 커밋)

---

- [x] 5. 통합, 크로스 레퍼런스, 일관성 검토

  **What to do**:
  - 전체 README.md 검토 및 일관성 보장:
    (a) 10개 섹션 전체의 한국어 톤 일관성 확인 (캐주얼-정보성, 본인 참고용)
    (b) 모든 섹션의 포맷 일관성 (동일 헤딩 레벨, 코드 블록 스타일, 콜아웃 형식)
    (c) 관련 섹션 간 크로스 레퍼런스 앵커 링크 추가:
      - Topic 3 (Open Code) ↔ Topic 8 (Git + AI)
      - Topic 5 (AI 모델) ↔ Topic 6 (프롬프트)
      - Topic 6 (프롬프트) ↔ Topic 9 (디버깅)
      - Topic 1 (환경 세팅) ↔ Topic 10 (유지보수)
    (d) TOC 앵커 링크가 실제 헤딩과 일치하는지 확인
    (e) 섹션 간 중복 콘텐츠 없는지 확인
    (f) 모든 `##` 섹션에 적절한 소개 문단 존재 확인
    (g) "마치며" 결론 문단 추가 (2~3문장)
    (h) 남아있는 `<!-- CONTENT -->` 플레이스홀더 마커 모두 제거
    (i) 전체 문서의 흐름이 자연스러운지 확인

  **Must NOT do**:
  - 콘텐츠 대폭 변경 금지 — 톤/형식/링크 조정만
  - 새로운 섹션 추가 금지
  - 범위 밖 콘텐츠 추가 금지

  **Recommended Agent Profile**:
  - **Category**: `unspecified-low`
    - Reason: 구조적 검토 및 경미한 편집 작업
  - **Skills**: []

  **Parallelization**:
  - **Can Run In Parallel**: NO
  - **Parallel Group**: Wave 3 (단독)
  - **Blocks**: Task 6
  - **Blocked By**: Tasks 2, 3, 4

  **References**:
  - 플랜의 "Must Have" / "Must NOT Have" 섹션 — 준수 확인
  - Task 1의 스켈레톤 구조 — TOC 앵커 링크 대조

  **Acceptance Criteria**:

  **QA Scenarios:**

  ```
  Scenario: 플레이스홀더 완전 제거 확인
    Tool: Bash
    Preconditions: Tasks 2, 3, 4 모두 완료
    Steps:
      1. `grep -c "<!-- CONTENT" README.md` — 0이어야 함
      2. `grep -c "^## " README.md` — 10~12 (10 토픽 + 마치며 등)
    Expected Result: 플레이스홀더 0개, 섹션 수 안정적
    Evidence: .sisyphus/evidence/task-5-integration-verify.txt

  Scenario: 크로스 레퍼런스 링크 유효성
    Tool: Bash
    Preconditions: 크로스 레퍼런스 추가 완료
    Steps:
      1. README.md 내의 모든 `](#` 형태 앵커 링크 추출
      2. 각 앵커의 대상 헤딩이 실제 존재하는지 확인
    Expected Result: 모든 앵커 링크가 유효한 헤딩을 가리킴
    Failure Indicators: 깨진 앵커 링크 존재
    Evidence: .sisyphus/evidence/task-5-links-verify.txt

  Scenario: 톤 및 형식 일관성
    Tool: Bash
    Preconditions: 통합 완료
    Steps:
      1. 각 `##` 섹션에 `> 💡` 콜아웃 존재 확인: `grep -c "💡" README.md` — 10이어야 함
      2. Windows 표기 없음: `grep -c "Ctrl+" README.md` — 0
      3. `grep -c "Cmd+" README.md` — 0
    Expected Result: 10개 섹션 모두 💡 콜아웃 포함, Windows 표기 없음
    Evidence: .sisyphus/evidence/task-5-consistency-verify.txt
  ```

  **Commit**: YES
  - Message: `docs: add complete guide content for all 10 Mac coding tips`
  - Files: `README.md`
  - Pre-commit: `wc -w README.md` (5000-10000 범위 확인)

---

- [x] 6. 수용 기준 검증 및 최종 수정

  **What to do**:
  모든 수용 기준 검증 명령어 실행:
  1. `test -f README.md` — 파일 존재
  2. `grep -c "^## " README.md` — 10개 이상 섹션
  3. `awk '/^```$/{c++} END{print c+0}' README.md` — 0 (미태그 코드 블록 없음, macOS 호환)
  4. `wc -w README.md` — 5,000~10,000 단어
  5. `grep -c "Ctrl+" README.md` — 0 (Windows 표기 없음)
  6. `grep -c "Cmd+" README.md` — 0 (Windows 표기 없음)
  7. `grep -c "<!-- CONTENT" README.md` — 0 (플레이스홀더 없음)
  8. Korean 콘텐츠가 주요 언어인지 확인
  실패 항목 발견 시 즉시 수정. 모든 검증 통과 후 최종 커밋 (수정 있을 경우에만).

  **Must NOT do**:
  - 콘텐츠 대폭 변경 금지 — QA 수정만
  - 새로운 콘텐츠 추가 금지

  **Recommended Agent Profile**:
  - **Category**: `quick`
    - Reason: 검증 명령어 실행 및 경미한 수정
  - **Skills**: [`git-master`]
    - `git-master`: 최종 커밋 관리

  **Parallelization**:
  - **Can Run In Parallel**: NO
  - **Parallel Group**: Wave 4 (단독)
  - **Blocks**: F1-F4 (Final Verification)
  - **Blocked By**: Task 5

  **References**:
  - 플랜의 "Success Criteria" 섹션 — 모든 검증 명령어 포함
  - 플랜의 "Must Have" / "Must NOT Have" — 최종 대조

  **Acceptance Criteria**:

  **QA Scenarios:**

  ```
  Scenario: 전체 수용 기준 통과
    Tool: Bash
    Preconditions: Task 5 완료
    Steps:
      1. `test -f README.md && echo "AC-1: PASS"` — 파일 존재
      2. `count=$(grep -c "^## " README.md); [ $count -ge 10 ] && echo "AC-2: PASS ($count sections)" || echo "AC-2: FAIL ($count sections)"`
      3. `count=$(awk '/^```$/{c++} END{print c+0}' README.md); [ "$count" -eq 0 ] && echo "AC-3: PASS" || echo "AC-3: FAIL ($count untagged blocks)"` (macOS 호환 — grep -cP 대신 awk 사용)
      4. `words=$(wc -w < README.md); [ $words -ge 5000 ] && [ $words -le 10000 ] && echo "AC-4: PASS ($words words)" || echo "AC-4: FAIL ($words words)"`
      5. `count=$(grep -c "Ctrl+" README.md || true); [ $count -eq 0 ] && echo "AC-5: PASS" || echo "AC-5: FAIL ($count occurrences)"`
      6. `count=$(grep -c "Cmd+" README.md || true); [ $count -eq 0 ] && echo "AC-6: PASS" || echo "AC-6: FAIL ($count occurrences)"`
      7. `count=$(grep -c "<!-- CONTENT" README.md || true); [ $count -eq 0 ] && echo "AC-7: PASS" || echo "AC-7: FAIL ($count placeholders)"`
    Expected Result: 모든 AC-1 ~ AC-7 PASS
    Failure Indicators: 하나라도 FAIL
    Evidence: .sisyphus/evidence/task-6-acceptance-results.txt

  Scenario: Git 히스토리 검증
    Tool: Bash
    Preconditions: 최종 커밋 완료
    Steps:
      1. `git log --oneline` — 2~3개 깔끔한 커밋 메시지 확인
      2. `git status` — working tree clean
    Expected Result: 2~3개 커밋, 깨끗한 working tree
    Evidence: .sisyphus/evidence/task-6-git-history.txt
  ```

  **Commit**: YES (수정 있을 경우에만)
  - Message: `docs: polish formatting and fix QA issues`
  - Files: `README.md`

---

## Final Verification Wave (MANDATORY — after ALL implementation tasks)

> 4 review agents run in PARALLEL. ALL must APPROVE. Present consolidated results to user and get explicit "okay" before completing.

- [x] F1. **플랜 준수 감사** — `oracle`

  **What to do**:
  플랜을 처음부터 끝까지 읽고 "Must Have" 항목 각각에 대해 구현 존재 여부 확인. "Must NOT Have" 항목에 대해 코드베이스에서 금지 패턴 검색 — 발견 시 file:line과 함께 거부. `.sisyphus/evidence/` 내 증거 파일 존재 확인. 산출물과 플랜 비교.

  **Recommended Agent Profile**:
  - **Category**: `unspecified-high`
    - Reason: 플랜 전체를 읽고 README.md 와 대조하는 분석 작업

  **QA Scenarios:**

  ```
  Scenario: Must Have 항목 전수 검증
    Tool: Bash
    Preconditions: Task 6 완료, README.md 최종 상태
    Steps:
      1. 플랜 파일 `.sisyphus/plans/mac-coding-tips.md`에서 "Must Have" 섹션의 항목 추출
      2. 각 항목에 대해 README.md에서 해당 구현 존재 확인:
         - "10개 토픽 모두 상세 콘텐츠" → `grep -c "^## " README.md` — 10 이상
         - "각 섹션에 실행 가능한 명령어/설정 예제" → 각 `##` 섹션 내 코드 블록 존재 확인
         - "목차와 섹션 간 크로스 레퍼런스" → `grep -c "](#" README.md` — 10 이상
         - "마지막 업데이트 날짜 헤더" → `grep "마지막 업데이트" README.md`
         - "일관된 섹션 템플릿 구조" → 각 섹션에 `> 💡` 콜아웃 존재 확인
      3. "Must NOT Have" 항목에 대해 금지 패턴 검색:
         - `grep -c "Ctrl+" README.md` — 0이어야 함
         - `grep -c "Cmd+" README.md` — 0이어야 함
         - `awk '/^```$/{c++} END{print c+0}' README.md` — 0이어야 함
      4. `.sisyphus/evidence/` 디렉토리 내 증거 파일 존재 확인: `ls .sisyphus/evidence/ | wc -l` — 10 이상
    Expected Result: Must Have 모두 충족, Must NOT Have 모두 부재, 증거 파일 존재
    Failure Indicators: Must Have 항목 누락 또는 Must NOT Have 패턴 발견
    Evidence: .sisyphus/evidence/f1-plan-compliance.txt
  ```

  Output: `Must Have [N/N] | Must NOT Have [N/N] | Tasks [N/N] | VERDICT: APPROVE/REJECT`

---

- [x] F2. **마크다운 품질 리뷰** — `unspecified-high`

  **What to do**:
  모든 마크다운 문법 검증: 헤딩 레벨 점프 없음, 코드 블록 모두 닫힘, 리스트 형식 일관성, 링크 유효성. AI 슬롭 패턴 확인: 과도한 주석, 불필요한 추상화, 일반적 변수명.

  **Recommended Agent Profile**:
  - **Category**: `unspecified-high`
    - Reason: 마크다운 구조 분석 및 품질 검토

  **QA Scenarios:**

  ```
  Scenario: 마크다운 구조 검증
    Tool: Bash
    Preconditions: README.md 최종 상태
    Steps:
      1. 헤딩 레벨 점프 확인: README.md 전체에서 `#` 다음에 `###`이 바로 오는 경우 검색 (## 레벨을 건너뛰는 경우)
         - `awk '/^#/{print NR": "$0}' README.md` 로 전체 헤딩 목록 추출 후 레벨 순서 확인
      2. 코드 블록 닫힘 확인: 열린 코드 블록(```)과 닫힌 코드 블록의 개수가 짝수인지 확인
         - `grep -c '^\x60\x60\x60' README.md` — 짝수여야 함 (열고 닫기)
      3. 리스트 형식 일관성: `-` 또는 `*` 또는 숫자 리스트가 혼재하지 않는지 확인
      4. 앵커 링크 유효성: README.md 내 `](#` 패턴의 링크 대상이 실제 헤딩과 일치하는지 확인
      5. AI 슬롭 패턴 검색: "물론", "알겠습니다", "도움이 되셨길" 등의 AI 대화체 잔존 여부
         - `grep -ci "물론\|알겠습니다\|도움이" README.md` — 0이어야 함
    Expected Result: 헤딩 레벨 순서 정상, 코드 블록 짝수, 리스트 일관적, 링크 유효, AI 대화체 없음
    Failure Indicators: 헤딩 레벨 점프, 열린 코드 블록, 깨진 링크
    Evidence: .sisyphus/evidence/f2-markdown-quality.txt
  ```

  Output: `Markdown Lint [PASS/FAIL] | Format [N clean/N issues] | VERDICT`

---

- [x] F3. **콘텐츠 QA** — `unspecified-high`

  **What to do**:
  10개 섹션 각각에 대해: (1) 300단어 이상인지, (2) 코드 블록 1개 이상 포함, (3) 💡 팁 존재, (4) Mac 표기법 사용, (5) 언급된 도구/명령어 실존 여부 검증. 크로스 레퍼런스 링크 작동 확인.

  **Recommended Agent Profile**:
  - **Category**: `unspecified-high`
    - Reason: 10개 섹션 각각의 콘텐츠 품질을 개별 검증

  **QA Scenarios:**

  ```
  Scenario: 섹션별 분량 및 구성요소 검증
    Tool: Bash
    Preconditions: README.md 최종 상태
    Steps:
      1. README.md를 `## ` 구분자로 10개 섹션으로 분리
      2. 각 섹션에 대해:
         - `wc -w` 로 단어 수 확인 — 300 이상
         - 코드 블록 (```) 존재 확인 — 1개 이상
         - `💡` 콜아웃 존재 확인
         - `⌘` 또는 `⌥` 또는 `⌃` 중 하나 이상 존재 확인 (Topic 7 등 해당 섹션)
      3. 분석 결과를 테이블 형태로 정리:
         `Section | Words | CodeBlocks | Tip | MacNotation | PASS/FAIL`
    Expected Result: 10개 섹션 모두 300단어 이상, 코드 블록 1개 이상, 💡 콜아웃 포함
    Failure Indicators: 300단어 미만 섹션, 코드 블록 없는 섹션, 💡 누락
    Evidence: .sisyphus/evidence/f3-content-qa.txt

  Scenario: 도구/명령어 실존 여부 검증
    Tool: Bash
    Preconditions: README.md 최종 상태
    Steps:
      1. README.md에서 언급된 Open Code 슬래시 커맨드 추출
      2. `.opencode/command/` 디렉토리의 실제 파일과 대조
      3. README.md에서 언급된 Homebrew 패키지 이름 추출
      4. 주요 패키지 (`brew info <package>`)로 실존 확인 (git, node, bun, fzf, ripgrep, jq, bat, eza, fd)
    Expected Result: 모든 커맨드/패키지가 실존
    Failure Indicators: 존재하지 않는 커맨드 또는 패키지 발견
    Evidence: .sisyphus/evidence/f3-commands-verify.txt
  ```

  Output: `Sections [N/N pass] | Commands Verified [N/N] | Links [N/N] | VERDICT`

---

- [x] F4. **범위 충실도 검사** — `deep`

  **What to do**:
  각 태스크(Task 0~6)에 대해: 플랜의 "What to do" 읽기, 실제 결과물 대조. 1:1 매칭 확인 — 스펙에 있는 모든 것이 구현됨 (누락 없음), 스펙 밖의 것이 추가되지 않음 (범위 증가 없음). "Must NOT do" 준수 확인.

  **Recommended Agent Profile**:
  - **Category**: `deep`
    - Reason: 플랜 전체와 결과물의 정밀 1:1 대조 분석

  **QA Scenarios:**

  ```
  Scenario: 태스크별 스펙-구현 1:1 대조
    Tool: Bash + Read
    Preconditions: 모든 구현 태스크 완료
    Steps:
      1. `.sisyphus/plans/mac-coding-tips.md` 읽기 — 각 Task의 "What to do" 섹션 추출
      2. Task 0: `git status` — Git 저장소 초기화 확인, `.gitignore` 존재 확인
      3. Task 1: README.md 구조 확인 — TOC 존재, 10개 `##` 헤더 존재
      4. Task 2: Topics 1,2,7,10 콘텐츠 — Homebrew, VS Code, 키보드, 유지보수 내용 확인
      5. Task 3: Topics 3,4,5 콘텐츠 — Open Code, Open Spec, AI 모델 비교 내용 확인
      6. Task 4: Topics 6,8,9 콘텐츠 — 프롬프트, Git+AI, 디버깅 내용 확인
      7. Task 5: 크로스 레퍼런스 링크 존재, 💡 콜아웃 10개, 플레이스홀더 0개
      8. Task 6: 모든 AC-1~AC-7 PASS 확인
      9. "Must NOT do" 준수 검증:
         - VS Code 확장 수 세기 — 10개 이하인지
         - 키보드 단축키 수 세기 — 20개 이하인지
         - `grep -c "Ctrl+\|Alt+" README.md` — 0이어야 함
    Expected Result: 모든 태스크의 스펙이 1:1 구현됨, 범위 증가 없음
    Failure Indicators: 스펙에 명시된 항목 누락, 스펙 밖 추가 콘텐츠, Must NOT do 위반
    Evidence: .sisyphus/evidence/f4-scope-fidelity.txt

  Scenario: 범위 초과(scope creep) 탐지
    Tool: Bash + Read
    Preconditions: README.md 최종 상태
    Steps:
      1. README.md의 `##` 섹션이 정확히 플랜의 10개 토픽 + 마치며인지 확인
      2. 플랜에 없는 추가 `##` 섹션이 있으면 FAIL
      3. 각 섹션 내 서브토픽이 플랜의 "What to do"에 명시된 범위 내인지 확인
      4. 비해당 프로그래밍 언어 튜토리얼, 하드웨어 리뷰 등 금지된 콘텐츠 검색
    Expected Result: 플랜과 1:1 매칭, 범위 초과 없음
    Failure Indicators: 미계획 섹션 발견, 금지 콘텐츠 발견
    Evidence: .sisyphus/evidence/f4-scope-creep.txt
  ```

  Output: `Tasks [N/N compliant] | Scope [CLEAN/N issues] | Unaccounted [CLEAN/N files] | VERDICT`

---

## Commit Strategy

```
git init  (Wave 0 — 사전 단계)

Commit 1: "docs: add README skeleton with TOC and section structure"
  - README.md (스켈레톤만)
  - Pre-commit: grep -c "^## " README.md (10+ 확인)

Commit 2: "docs: add complete guide content for all 10 Mac coding tips"
  - README.md (전체 콘텐츠)
  - Pre-commit: wc -w README.md (5000-10000 확인)

Commit 3 (QA 수정 있을 경우에만): "docs: polish formatting and fix QA issues"
  - README.md
```

---

## Success Criteria

### Verification Commands
```bash
# 파일 존재
test -f README.md && echo "PASS" || echo "FAIL"

# 토픽 섹션 수 (10개 이상)
grep -c "^## " README.md

# 미태그 코드 블록 없음 (0이어야 함)
awk '/^```$/{c++} END{print c+0}' README.md

# 단어 수 범위 (5000-10000)
wc -w README.md

# Windows 키보드 표기 없음 (각각 0이어야 함)
grep -c "Ctrl+" README.md
grep -c "Cmd+" README.md

# 플레이스홀더 마커 잔여 없음 (0이어야 함)
grep -c "<!-- CONTENT" README.md
```

### Final Checklist
- [x] 모든 "Must Have" 항목 존재
- [x] 모든 "Must NOT Have" 항목 부재
- [x] 10개 섹션 모두 300~800 단어 범위
- [x] Git 히스토리 깔끔 (2-3 커밋)
