# 안녕하세요, 정준하입니다 👋

### “원래 그렇게 한다”는 말에서, 더 나은 방법을 찾습니다.

LLM 기반 에이전트와 데이터 분석을 활용해
실제 업무에 도움이 되는 서비스를 개발하고 있습니다.

멀티 에이전트 기반 개발 문서 자동화 플랫폼 **ALPLED**에서
**통합시험 시나리오 생성 에이전트 개발**을 담당했습니다.

또한 **NeuroAge-MAS**를 통해 뇌 체적·임상·유전체 자료의
입력 검증, 모델 비교, 연구 결과 검토와 보고서 생성을 연결하는
연구용 플랫폼을 개발하고 있습니다.

입력 데이터의 근거와 처리 과정을 확인하고,
결과를 다시 검토할 수 있는 구조를 만드는 데 관심이 있습니다.

---

## 🛠️ Tech Stacks

아래는 참여·개발 프로젝트에서 사용하는 기술 구성입니다.
프로젝트 전체 기술과 개인 담당 범위는 각 프로젝트 설명에서 구분합니다.

### Languages

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css&logoColor=white)

### AI / ML & Data

![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white)
![XGBoost](https://img.shields.io/badge/XGBoost-189AB4?style=flat-square)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white)
![SciPy](https://img.shields.io/badge/SciPy-8CAAE6?style=flat-square&logo=scipy&logoColor=white)

### Web & Backend

![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=flat-square&logo=vite&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white)

### Tools & Quality

![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![pytest](https://img.shields.io/badge/pytest-0A9EDC?style=flat-square&logo=pytest&logoColor=white)
![Ruff](https://img.shields.io/badge/Ruff-D7FF64?style=flat-square&logo=ruff&logoColor=black)

---

## 🚀 Projects

## 🤖 ALPLED
### AI-DLC Platform for sLLM Enterprise Documentation

**멀티 에이전트 기반 AI-DLC 문서 생성 자동화 플랫폼**

> RFP·회의록 → 요구사항·설계·테스트 등 6종 SW 개발 산출물 생성

개발 과정에서 반복되는 문서 작성을 자동화하고,
산출물 간 연결과 정합성을 관리하는 팀 프로젝트입니다.

### 담당 역할

**통합시험 시나리오 생성 에이전트 개발**

요구사항 정의서와 인터페이스 참조 정보를 입력받아
시험 시나리오, 테스트 케이스, 단계별 시험 절차를 생성하는
`TestScenarioGenerationAgent`를 개발했습니다.

### 상세 구현

#### 입력 검증 및 전처리

- 산출물 코드 `TS`와 실행 모드 검증
- `udt_yn`을 기준으로 신규 생성·수정 흐름 분리
- 요구사항·인터페이스 참조 목록의 필수 입력 확인
- 기능 요구사항 필터링 및 LLM 전달용 입력 압축
- 필수 입력 누락 시 오류 코드와 실패 상태 반환

#### 단계별 생성 파이프라인

1. 기능 요구사항 기반 시나리오 생성
2. 요구사항 ID 기준 연결 누락 확인 및 보완
3. 시나리오별 테스트 케이스 생성
4. 시험 절차의 기본 단계 생성
5. 인터페이스 참조 기반 상세 절차 생성
6. 확정된 최종 절차를 기준으로 설명 요약 생성

상세 절차를 확정한 뒤 요약을 생성하여,
요약과 최종 시험 절차의 불일치를 줄이도록 구성했습니다.

#### 요구사항 추적

- `source_requirement_ids`로 원본 요구사항과 시나리오 연결
- 입력 요구사항과 생성 결과의 ID 비교
- 연결되지 않은 요구사항의 시나리오 보완
- 보완 내용을 경고 정보로 기록
- 테스트 케이스까지 요구사항 추적 정보 전달

요구사항 ID 연결 여부와 시험 내용의 충분성은 구분하여 검토합니다.

#### 구조화된 출력 및 오류 대응

- 시나리오·케이스·절차·상세 정보를 JSON 목록으로 구성
- 공통 `LLMClient`와 병렬 호출 유틸리티 활용
- JSON 응답 파싱 및 필드 자료형 정규화
- 호출·파싱 실패 시 기본 생성 로직 적용
- 경고와 일부 원본 응답 기록을 통한 후속 검토 지원
- 실제 시험 전 `test_result`를 `None`으로 유지

#### 공통 워크플로우 연동

- `WorkflowState`에서 선행 에이전트 출력 참조
- `agent_outputs`에 생성 결과 저장
- 성공·실패 상태와 경고·오류 구분
- 기존 산출물 수정 및 단계별 정제 흐름 구성

### 주요 출력

| 필드 | 내용 |
|---|---|
| `scenario_json_list` | 요구사항 기반 시험 시나리오 |
| `test_case_json_list` | 시나리오별 테스트 케이스 |
| `step_json_list` | 케이스별 시험 절차 |
| `step_detail_json_list` | 사전조건·입력값·예상결과·화면 ID |
| `warnings` | 누락 보완·기본값 적용 등 검토 정보 |
| `errors` | 처리 실패 관련 오류 정보 |

### 팀 프로젝트 기술 구성

`Python` · `LangGraph` · `FastAPI` · `Django`  
`Qwen` · `vLLM` · `Qdrant` · `MySQL` · `SQLAlchemy`

*위 기술은 팀 프로젝트 전체 구성입니다.
개인 담당 영역은 통합시험 시나리오 생성 에이전트입니다.*

🔗 [Repository](https://github.com/junhaj27-jpg/jun)
· [Agent Code](https://github.com/junhaj27-jpg/jun/tree/HEAD/ALPLED-CORE/agents/test_scenario)

---

## 🧠 NeuroAge-MAS
### 뇌 체적·임상·유전체 데이터 연구 플랫폼

**표 형식 뇌 부피·임상·유전체 자료의 입력 검증부터
분석 실행, 내부 연구 검토와 보고서 생성까지 연결하는 연구용 플랫폼입니다.**

> 입력 검증 → 데이터 처리 → 분석·모델 비교 → 정합성 검사 → 내부 검토 → 보고서 생성

### 프로젝트 기술 구성

프로젝트 수준의 기술 구성으로, 개인 기여 범위와는 구분합니다.

| 분야 | 기술 및 구현 범위 |
|---|---|
| Languages | Python, TypeScript, JavaScript, SQL, HTML/CSS |
| Backend | FastAPI, Pydantic, Uvicorn |
| Frontend | React, React DOM, Vite, TypeScript, Lucide React |
| Research Dashboard | Streamlit, Altair |
| Data Processing | Pandas, NumPy, SciPy, CSV/Excel/Parquet, openpyxl |
| Machine Learning | scikit-learn, XGBoost, Joblib |
| Regression | Dummy baseline, Ridge, ElasticNet, Random Forest, SVR |
| Classification | Logistic Regression, Random Forest, XGBoost |
| Model Selection | 환자 단위 분할, fold 내부 전처리, 교차검증, 선택적 Optuna 탐색 |
| Multimodal Fusion | 조기 결합, 고정 가중치 결합, OOF 기반 stacking |
| Explainability | Permutation importance, 선택적 SHAP |
| Uncertainty | Bootstrap, conformal prediction interval, drift 점검 |
| Harmonization | 메타데이터 확인 조건의 neuroHarmonize ComBat 연계 |
| Neural Network Experiment | 선택적 PyTorch MLP, CPU 기반 로컬 FedAvg 시뮬레이션 |
| Evidence Retrieval | TF-IDF, cosine similarity, 출처·페이지 포함 문서 발췌 검색 |
| Visualization | Matplotlib, mplot3d, Altair, React SVG |
| Reports | ReportLab PDF, python-docx, HTML/Markdown/CSV/JSON |
| Presentation | 별도 Node.js 아티팩트 런타임 기반 PPTX 생성 스크립트 |
| Storage & Execution | SQLite, 자체 작업 큐·worker, 선택적 Redis 알림 |
| Quality & Tooling | pytest, FastAPI TestClient, Ruff, pytest-cov, pip-audit |
| Development & CI | GitHub Actions, Dev Container, Vite build |

### 주요 기능

#### 1. 종단 뇌 부피 분석

- 대상자·방문·단위·시점의 입력 계약 검증
- ROI별 부피 변화량 및 변화율 계산
- 시간 간격이 확인된 경우에만 연간 변화 환산
- 입력 근거와 분석 가능 범위 표시

#### 2. 임상 데이터 분석

- 코드북 기반 변수 처리
- 특수 결측 코드 관리
- 교육용 임상 자료에서 당뇨 첫 확인 조사일 분석
- 데이터 간 연결 근거 및 해석 범위 표시

#### 3. 모델 비교 및 멀티모달 실험

- 표형 특징 기반 회귀·분류 모델 비교
- 환자 단위 데이터 분할
- 학습 fold 내부 전처리를 통한 데이터 누수 방지
- 교차검증 및 선택적 하이퍼파라미터 탐색
- 조기 결합·고정 가중치 결합·OOF stacking
- Permutation importance 및 선택적 SHAP 분석

#### 4. 불확실성 및 데이터 분포 점검

- Bootstrap 기반 추정
- Conformal prediction interval
- 데이터 drift 점검
- 조건을 충족한 메타데이터 기반 ComBat 연계

#### 5. 유전체 연계

- PLINK BED/BIM/FAM 구조 검사
- QC·PCA·PRS·GWAS 실행 래퍼
- 유전 PC·PRS의 출처 확인
- 유전체 빌드 및 대상자 연결 검사

PLINK 분석에는 별도 실행 파일과
검증된 입력·매핑·가중치가 필요합니다.

#### 6. 근거 문서 검색

- TF-IDF 기반 문서 표현
- Cosine similarity 기반 관련 발췌 검색
- 검색 결과에 출처와 페이지 정보 포함
- 분석 결과를 검토할 때 참고할 근거 제공

#### 7. 추적 가능한 연구 워크플로

- 역할별 Python 에이전트 및 산출물 오케스트레이션
- 입력·설정·모델·결과의 해시 기록
- 실행 이력 관리
- 분석 실행과 정합성 검사 상태 분리
- 내부 연구 검토·승인 상태 관리
- 집계 시각화와 PDF·DOCX·웹 보고서 생성

### 선택적·별도 실행 경로

- XGBoost·SHAP·Optuna·ComBat·PyTorch 실험은 의존성과 설정 조건에 따라 사용합니다.
- PyTorch MLP와 CPU 기반 FedAvg는 선택적 실험 경로입니다.
- NiBabel·abagen·scikit-image는 표준 뇌 모형 자산 생성 스크립트에서 사용합니다.
- Redis는 선택적 알림 용도입니다.
- 외부 LLM 설명 연동과 PostgreSQL 기반 분산 운영은 현재 구현 범위와 구분합니다.

### 범위와 결과 해석

- 주요 분석 대상은 표 형식 뇌 체적·임상·유전체 자료입니다.
- 원본 MRI 영상의 분할·정합이나 3D CNN 학습은 현재 플랫폼의 범위에 포함하지 않습니다.
- 뇌 나이 실험은 실제 나이 라벨·촬영 시점·입력 근거를 충족해야 하는 별도 경로입니다.
- 합성 자료·교육용 자료·실제 자료를 구분합니다.
- 합성 실험 결과를 실제 환자 성능이나 의료적 효과로 해석하지 않습니다.
- FedAvg는 로컬 시뮬레이션이며 실제 병원 간 연합학습을 의미하지 않습니다.
- 내부 연구 승인은 임상적 유효성 검증이나 규제 승인을 의미하지 않습니다.
- 성능 수치와 개인 기여는 실행 기록과 역할 근거가 확인된 범위에서 기재합니다.

🔗 [Repository](https://github.com/PostMarketSurveillance/NeuroAge-MAS)

---

## 🏥 의료기기 PMS 업무 지원

**의료기기 시판 후 관리 과정의 업무·기록·후속 조치를 연결하는 시스템을 개발하고 있습니다.**

### 개발·고도화 항목

| 항목 | 주요 내용 |
|---|---|
| 담당 업무·기한 관리 | 담당자 지정, 마감일, 개인별 할 일 |
| CAPA 관리 | 조치 이력, 증빙 등록, 효과성 평가 |
| 리콜 회수 이력 | 거래처별 통보·회신·회수 수량·미회수 사유 |
| 보고 규칙 버전 관리 | 적용 조건, 시행일, 규칙 변경 이력 |
| 보고서 출력 | 업무 기록과 증빙을 보고서로 정리 |

업무 이력의 추적성, 담당자의 검토·승인,
규정 근거와 적용 시점에 따른 규칙 관리를 중심으로 설계합니다.

*개발 완료 기능과 고도화 목표는 프로젝트 문서에서 구분하여 관리합니다.*

---

## 🤝 Other Projects

- [SKN24-1st-Team](https://github.com/SKNETWORKS-FAMILY-AICAMP/SKN24-1st-Team)  
  지역별 자동차 등록 및 교통사고 현황

- [SKN24-2nd-4Team](https://github.com/SKNETWORKS-FAMILY-AICAMP/SKN24-2nd-4Team)  
  팀 프로젝트 참여

- [SKN24-3rd-1Team](https://github.com/SKNETWORKS-FAMILY-AICAMP/SKN24-3rd-1Team)  
  팀 프로젝트 참여

---

## 🌱 What I’m Working On

- 요구사항과 테스트 케이스의 연결 관계 문서화
- LLM 생성 결과의 품질 평가와 오류 처리 개선
- 뇌 체적·임상·유전체 데이터의 연결 근거 검증
- 모델 비교와 불확실성 분석
- 재현 가능한 실행 환경과 연구 이력 관리
- 프로젝트별 개인 기여 및 검증 사례 정리

---

## 💼 Career Interests

- AI 에이전트·LLM 응용 서비스 개발
- 헬스케어 데이터 분석
- 의료 AI 연구·개발
- 의료기기 QA·PMS 업무 자동화
- 규정과 근거를 연결하는 업무 지원 시스템

---

## 🧪 How I Work

- 왜 필요한 설계인지 먼저 확인합니다.
- 팀 전체 성과와 개인 기여를 구분합니다.
- 구현된 기능과 실험·계획 단계를 구분합니다.
- 입력 데이터와 분석 결과의 근거를 기록합니다.
- AI 생성 코드와 문서는 실행·검토를 통해 확인합니다.
- 결과를 재현하고 다시 검토할 수 있도록 문서화합니다.

---

## 🧑‍💻 Contact Me

[![GitHub](https://img.shields.io/badge/GitHub-junhaj27--jpg-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/junhaj27-jpg)
