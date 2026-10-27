## 🛠️ Tech Stacks

### AI / ML

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![XGBoost](https://img.shields.io/badge/XGBoost-189AB4?style=flat-square)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white)

- **Python**: 데이터 전처리, 모델 학습·평가, AI 에이전트 로직 구현
- **XGBoost·회귀 모델**: 뇌 체적 데이터 기반 예측 및 기준 모델 비교
- **LLM 응용**: 단계별 프롬프트 구성, JSON 응답 파싱, 생성 결과 정규화
- **에이전트 파이프라인**: 입력 검증부터 시나리오·케이스·절차·요약 생성까지 단계 분리

### Agent Engineering

- **요구사항 추적**: `source_requirement_ids`를 통한 생성 결과와 원본 요구사항 연결
- **커버리지 보정**: 기능 요구사항에 대응하는 시나리오 누락 확인 및 보완
- **구조화된 출력**: 시나리오·테스트 케이스·시험 절차를 JSON 목록으로 관리
- **병렬 요청**: 공통 LLM 클라이언트와 병렬 호출 유틸리티 활용
- **오류 대응**: 응답 파싱 실패 시 기본 생성 로직 적용 및 경고 기록
- **워크플로우 연동**: 공통 상태 객체를 통한 입력 전달 및 에이전트 결과 저장

### Tools

![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=flat-square&logo=jupyter&logoColor=white)
![pytest](https://img.shields.io/badge/pytest-0A9EDC?style=flat-square&logo=pytest&logoColor=white)

- **Git·GitHub**: 코드 버전 관리 및 팀 프로젝트 협업
- **Jupyter Notebook**: 데이터 분석 및 모델 실험
- **pytest**: 학습용 프로젝트의 코드 동작 검증

---

## 🚀 Projects

### 🤖 ALPLED — AI-DLC Platform for sLLM Enterprise Documentation

**멀티 에이전트 기반 AI-DLC 문서 생성 자동화 플랫폼**

> RFP·회의록 → 요구사항·설계·테스트 등 6종 SW 개발 산출물 생성

개발 과정에서 반복되는 문서 작성 업무를 자동화하고,
산출물 간 연결과 정합성을 관리하는 팀 프로젝트입니다.

### 담당 역할 — 통합시험 시나리오 생성 에이전트 개발

요구사항 정의서와 인터페이스 참조 정보를 입력받아
시험 시나리오, 테스트 케이스, 단계별 시험 절차를 생성하는
`TestScenarioGenerationAgent`를 개발했습니다.

#### 1. 입력 검증 및 전처리

- 산출물 코드가 `TS`인지 확인하여 실행 대상 검증
- `udt_yn` 값에 따라 신규 생성과 기존 산출물 수정 흐름 분리
- 신규 생성에 필요한 요구사항·인터페이스 참조 목록 확인
- 기능 요구사항 필터링 및 LLM 전달용 입력 압축
- 필수 입력 누락 시 오류 코드와 실패 상태 반환

#### 2. 단계별 생성 파이프라인

한 번의 응답에 전체 문서를 맡기지 않고,
생성 대상을 단계별로 나누어 처리했습니다.

1. 기능 요구사항 기반 시험 시나리오 생성
2. 요구사항 ID 기준 시나리오 누락 확인 및 보완
3. 시나리오별 테스트 케이스 생성
4. 시험 절차의 기본 단계 생성
5. 인터페이스 정보를 참조한 단계별 상세 정보 생성
6. 최종 절차를 기준으로 케이스 설명 요약 생성

상세 절차를 확정한 뒤 요약을 생성하여,
요약과 최종 시험 절차가 어긋나는 문제를 줄이도록 구성했습니다.

#### 3. 요구사항 추적 및 누락 보완

- `source_requirement_ids`로 원본 요구사항과 시나리오 연결
- 시나리오에 연결된 요구사항 ID 집합과 입력 요구사항 비교
- 연결되지 않은 요구사항은 기본 시나리오를 추가하여 보완
- 보완 결과를 `TS_REQUIREMENT_COVERAGE_REPAIRED` 경고로 기록
- 테스트 케이스에도 요구사항 ID를 전달하여 추적 정보 유지

이 보정은 요구사항 ID의 연결 누락을 다루며,
생성된 시험 내용의 충분성은 별도 검토 대상으로 구분합니다.

#### 4. 테스트 케이스 및 시험 절차 구조화

- 시나리오·테스트 케이스·절차별 식별자 구성
- 테스트 케이스 유형과 입력 필드 정규화
- 요구사항 ID를 기준으로 인터페이스 참조 정보 연결
- 시험 절차에 다음 항목 구성
  - 처리내용
  - 시험항목
  - 사전조건
  - 입력값
  - 예상결과
  - 화면 ID
- 실제 시험을 수행하기 전 `test_result`는 `None`으로 유지

시험 문서 생성과 실제 테스트 실행 결과를 구분하도록 구성했습니다.

#### 5. LLM 응답 처리 및 오류 대응

- 공통 `LLMClient`를 통한 모델 호출
- `send_parallel`을 활용한 단계 내 독립 요청 병렬 처리
- JSON 응답 파싱 및 목록·객체 형태 정규화
- 입력값·예상결과 등 필드의 자료형 보정
- 호출 실패 또는 응답 파싱 실패 시 기본 생성 로직 적용
- 일부 실패 경로에서 원본 응답 저장 및 경고에 경로 기록

기본값으로 보완된 결과를 경고 정보와 함께 전달하여
후속 검토에서 확인할 수 있도록 했습니다.

#### 6. 기존 산출물 수정 흐름

- 기존 통합 산출물에 시나리오 작성 규칙 적용
- 시나리오·테스트 케이스·시험 절차별 정제
- 누락된 케이스 또는 절차 생성
- 수정된 최종 절차를 기준으로 설명 요약 재생성
- 결과를 신규 생성과 동일한 출력 구조로 반환

#### 7. 공통 워크플로우 연동

- `WorkflowState`에서 문서 병합 에이전트의 결과 참조
- `agent_outputs`에 TS 에이전트 결과 저장
- 성공·실패 상태, 경고, 오류를 구분하여 반환
- 디버그 설정 시 전처리 입력 등 추가 정보 제공

### 출력 데이터 구조

| 출력 필드 | 내용 |
|---|---|
| `scenario_json_list` | 요구사항 기반 시험 시나리오 |
| `test_case_json_list` | 시나리오별 테스트 케이스 |
| `step_json_list` | 케이스별 시험 절차 |
| `step_detail_json_list` | 입력값·예상결과·화면 ID 등 상세 정보 |
| `warnings` | 누락 보완·기본값 적용 등 검토 정보 |
| `errors` | 처리 실패 관련 오류 정보 |

### 관련 구현

| 파일 | 역할 |
|---|---|
| `agent.py` | 신규 생성·수정 분기 및 전체 실행 흐름 |
| `prompts.py` | 단계별 프롬프트 및 입력 압축 |
| `scenario_generator.py` | 시나리오 생성·정제 및 요구사항 누락 보완 |
| `testcase_generator.py` | 테스트 케이스 생성·정규화 및 설명 요약 |
| `step_generator.py` | 시험 절차·상세 정보 생성 및 인터페이스 연결 |

### 팀 프로젝트 기술 구성

| 영역 | 기술 |
|---|---|
| AI 워크플로우 | LangGraph, 멀티 에이전트 |
| 모델·추론 | Qwen 계열 모델, 파인튜닝, vLLM |
| 검색 | Qdrant, 임베딩 기반 RAG |
| API·웹 | FastAPI, Django |
| 데이터베이스 | MySQL, SQLAlchemy |

*위 표는 팀 프로젝트 전체 기술 구성입니다.
개인 담당 영역은 통합시험 시나리오 생성 에이전트이며,
전체 아키텍처·RAG·파인튜닝 개발과는 구분합니다.*

🔗 [Repository](https://github.com/junhaj27-jpg/jun)
· [Agent Code](https://github.com/junhaj27-jpg/jun/tree/HEAD/ALPLED-CORE/agents/test_scenario)
