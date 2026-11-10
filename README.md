안녕하세요, 정준하입니다 👋

## 1. 소개

### “원래 그렇게 한다”는 말에서, 더 나은 방법을 찾습니다.

LLM 기반 에이전트와 데이터 분석을 활용해 실제 업무에 도움이 되는 서비스를 개발하고 있습니다.

멀티 에이전트 기반 개발 문서 자동화 플랫폼 **ALPLED**에서 **통합시험 시나리오 생성 에이전트 개발**을 담당했습니다.

**NeuroAge-MAS**에서는 뇌 체적·임상·유전체 자료의 입력 검증부터 모델 비교, 연구 결과 검토와 보고서 생성까지 연결하는 연구용 플랫폼을 개발하고 있습니다.

또한 **MedWatch PMS**를 통해 의료기기 시판 후 관리 업무를, **Brain MRI** 프로젝트를 통해 의료영상 로딩·마스크 처리·부피 계산·3D 시각화를 다루고 있습니다.

입력 데이터의 근거와 처리 과정을 확인하고, 결과를 재현하고 다시 검토할 수 있는 구조를 만드는 데 관심이 있습니다.

네 프로젝트에서 일관되게 다룬 질문은 **결과를 받은 사람이 무엇을 근거로 그 결과를 확인할 수 있는가**입니다. 시험 문서에서는 요구사항과 테스트 케이스를 연결하고, 연구 분석에서는 입력과 실행 설정을 남기며, 시판 후 안전관리에서는 규칙과 승인 당시 자료를 기록합니다. 의료영상에서는 마스크와 voxel의 공간 정보로부터 부피 계산을 설명합니다.

| 프로젝트 | 다루는 문제 | 역할 및 범위 | 검토할 수 있는 결과 |
|---|---|---|---|
| ALPLED | 요구사항을 시험 가능한 문서로 변환 | 팀 프로젝트에서 통합시험 시나리오 생성 에이전트 담당 | 요구사항 연결, 시나리오, 테스트 케이스, 시험 절차, 경고 |
| NeuroAge-MAS | 단위·방문·결측 기준이 다른 연구 자료 분석 | 표 형식 뇌 체적·임상·유전체 연구 플랫폼 개발 | 입력 검증 결과, 모델 비교, 불확실성, 실행 기록, 연구 보고서 |
| MedWatch PMS | 시판 후 안전관리 판단과 후속 조치 추적 | 의료기기 RA·QA 업무 지원 포트폴리오 | 사건 상태, CAPA, 보고 규칙 적용 근거, 리콜, 승인 기록 |
| Brain MRI | 의료영상에서 마스크, 부피, 3D 표면 확인 | 원본 영상 처리 및 시각화 프로토타입 | 3개 평면 슬라이스, 마스크 진단, 영역별 부피, 3D 파일과 PDF |

### 🛠️ 기술 스택

참여·개발 프로젝트에서 사용하는 기술입니다.  
팀 프로젝트 전체 기술과 개인 담당 범위, 기본 기능과 선택적 실험은 각 프로젝트 설명에서 구분합니다.

#### 💻 Languages

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=for-the-badge)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css&logoColor=white)

#### 🧠 AI / ML & Data

![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white)
![XGBoost](https://img.shields.io/badge/XGBoost-337AB7?style=for-the-badge)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![SciPy](https://img.shields.io/badge/SciPy-8CAAE6?style=for-the-badge&logo=scipy&logoColor=white)

#### 🤖 Agent & Workflow

![LLM Agents](https://img.shields.io/badge/LLM_Agents-6D28D9?style=for-the-badge)
![LangGraph](https://img.shields.io/badge/LangGraph-1C3C3C?style=for-the-badge&logo=langgraph&logoColor=white)
![Evidence Retrieval](https://img.shields.io/badge/Evidence_Retrieval-0F766E?style=for-the-badge)
![Structured Output](https://img.shields.io/badge/Structured_Output-475569?style=for-the-badge&logo=json&logoColor=white)

#### ⚙️ Backend

![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)
![Django](https://img.shields.io/badge/Django-092E20?style=for-the-badge&logo=django&logoColor=white)
![Django REST Framework](https://img.shields.io/badge/Django_REST_Framework-A30000?style=for-the-badge&logo=django&logoColor=white)
![Pydantic](https://img.shields.io/badge/Pydantic-E92063?style=for-the-badge&logo=pydantic&logoColor=white)

#### 🖥️ Frontend & Dashboard

![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white)
![Chart.js](https://img.shields.io/badge/Chart.js-FF6384?style=for-the-badge&logo=chartdotjs&logoColor=white)

#### 📊 Visualization

![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=for-the-badge)
![Altair](https://img.shields.io/badge/Altair-1F77B4?style=for-the-badge)
![Plotly](https://img.shields.io/badge/Plotly-3F4F75?style=for-the-badge&logo=plotly&logoColor=white)
![Three.js](https://img.shields.io/badge/Three.js-000000?style=for-the-badge&logo=threedotjs&logoColor=white)

#### 🩻 Medical Image

![pydicom](https://img.shields.io/badge/pydicom-3776AB?style=for-the-badge)
![NiBabel](https://img.shields.io/badge/NiBabel-4C72B0?style=for-the-badge)
![scikit-image](https://img.shields.io/badge/scikit--image-F7931E?style=for-the-badge)
![trimesh](https://img.shields.io/badge/trimesh-00897B?style=for-the-badge)

#### 🗄️ Database

![SQLite](https://img.shields.io/badge/SQLite-003B57?style=for-the-badge&logo=sqlite&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)

#### 📄 Reports

![ReportLab](https://img.shields.io/badge/ReportLab-003B7A?style=for-the-badge)
![python-docx](https://img.shields.io/badge/python--docx-2B579A?style=for-the-badge)
![Markdown](https://img.shields.io/badge/Markdown-000000?style=for-the-badge&logo=markdown&logoColor=white)

#### 🔧 Tools & Quality

![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white)
![pytest](https://img.shields.io/badge/pytest-0A9EDC?style=for-the-badge&logo=pytest&logoColor=white)
![Ruff](https://img.shields.io/badge/Ruff-D7FF64?style=for-the-badge&logo=ruff&logoColor=black)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)

### 프로젝트별 기술 구성

| 분야 | 원문에서 확인되는 기술과 방법 | 맥락 |
|---|---|---|
| 언어 | Python, TypeScript, JavaScript, SQL, HTML5, CSS3 | 에이전트·데이터 처리·API와 웹 화면 |
| LLM·워크플로 | LangGraph, Qwen, vLLM, Qdrant | ALPLED 팀 전체 구성 |
| 서버·검증 | FastAPI, Django, Django REST Framework, Pydantic, Uvicorn | ALPLED, NeuroAge-MAS, MedWatch PMS의 프로젝트별 구성 |
| 웹·대시보드 | React, Vite, Lucide React, Streamlit, Chart.js | NeuroAge-MAS, MedWatch PMS, Brain MRI |
| 데이터 처리 | Pandas, NumPy, SciPy, openpyxl | NeuroAge-MAS |
| 머신러닝 | scikit-learn, XGBoost, Joblib | NeuroAge-MAS 모델 비교와 실험 |
| 연구 확장 | PLINK, Optuna, SHAP, neuroHarmonize ComBat, PyTorch | 실행 전제나 별도 설정이 있는 연구 경로 포함 |
| 저장·실행 | MySQL, SQLAlchemy, SQLite, PostgreSQL, 자체 작업 큐·worker, 선택적 Redis 알림 | ALPLED 팀 구성, MedWatch PMS 기술 구성, NeuroAge-MAS 실행 경로 |
| 시각화 | Altair, Matplotlib, mplot3d, React SVG, Three.js, Plotly | 연구 결과 및 의료영상 표현 |
| 보고서 | ReportLab, python-docx, 서버 PDF 출력 | 프로젝트별 보고서 기능 |
| 영상 처리 | pydicom, NiBabel, scikit-image, trimesh, DICOM, NIfTI, Marching Cubes, HD-BET·SynthSeg 연계, GLB·STL | Brain MRI의 영상 형식, 도구, 메시 출력 |
| 품질·개발 | Git, GitHub, Docker, pytest, FastAPI TestClient, Ruff, pytest-cov, pip-audit, GitHub Actions, Dev Container, Vite build | 공통 개발 도구와 프로젝트별 테스트·빌드 구성 |

NeuroAge-MAS의 현재 실행 구성은 SQLite와 자체 작업 큐이며, PostgreSQL은 MedWatch PMS의 기술 구성과 NeuroAge-MAS의 분산 운영 확장 방향에 각각 등장합니다.

## 2. ALPLED | 통합시험 시나리오 생성 에이전트

**프로젝트:** 멀티 에이전트 기반 AI-DLC 문서 생성 자동화 플랫폼  
**개인 담당:** 통합시험 시나리오 생성 에이전트  
**팀 기술:** Python · LangGraph · FastAPI · Django · Qwen · vLLM · Qdrant · MySQL · SQLAlchemy

ALPLED는 제안요청서와 회의록을 바탕으로 요구사항·설계·테스트를 포함한 6종 개발 산출물을 생성하는 팀 프로젝트입니다. 제 담당은 선행 산출물에 담긴 기능 요구사항을 통합시험 시나리오, 테스트 케이스, 시험 절차와 상세 정보로 변환하는 에이전트(`TestScenarioGenerationAgent`)였습니다.

### 해결하려던 문제

시험 문서가 읽기 좋더라도, 원본 요구사항과의 연결이 빠져 있으면 어떤 기능이 시험 범위에서 누락됐는지 알기 어렵습니다. 요구사항 ID가 연결돼 있어도 예상결과가 모호하거나 사전조건이 잘못되면 시험 문서로 사용하기 어렵습니다. 여기에 LLM 호출 실패, 파싱할 수 없는 응답, 응답 필드의 자료형 불일치, 최종 절차와 설명의 불일치가 더해집니다.

따라서 생성 흐름에 **필수 입력 확인, 요구사항 ID 대조, 출력 정규화, 오류와 경고 분리**를 포함했습니다. 요구사항 연결 여부는 ID 대조로 확인하고, 개별 시험 내용의 충분성은 검토 항목으로 남깁니다.

### 입력부터 출력까지

| 단계 | 구현 내용 | 검토하는 이유 |
|---|---|---|
| 1. 실행 조건 확인 | 산출물 코드 `TS`와 실행 모드를 검증하고 `udt_yn`을 기준으로 신규 생성과 기존 산출물 수정 흐름을 구분 | 요청과 처리 경로가 일치해야 이후 생성 결과를 해석할 수 있음 |
| 2. 선행 자료 확인 | 요구사항과 인터페이스 참조 정보를 확인하고 필수 입력 누락 시 오류 코드와 실패 상태 반환 | 근거가 없는 상태에서 시험 절차를 생성하는 일을 방지 |
| 3. 입력 정리 | 기능 요구사항을 필터링하고 LLM에 전달할 내용을 압축 | 현재 시험 생성 단계에 필요한 자료에 집중 |
| 4. 시나리오 생성 | 기능 요구사항을 바탕으로 시험 시나리오 생성 | 어떤 기능을 어떤 상황에서 검증할지 정의 |
| 5. 요구사항 연결 점검 | 원본 요구사항 ID와 생성 결과의 `source_requirement_ids`를 대조하고 누락 시나리오 보완 | 시험 범위의 연결 누락을 드러내고 보완 이력을 남김 |
| 6. 케이스 생성 | 시나리오별 테스트 케이스를 만들고 요구사항 추적 정보를 전달 | 개별 시험 항목이 어느 요구사항에서 출발했는지 확인 |
| 7. 시험 절차 구성 | 케이스별 기본 시험 절차를 생성 | 실행 순서를 갖춘 절차의 뼈대를 구성 |
| 8. 상세화 | 인터페이스 참조를 사용해 사전조건·입력값·예상결과·화면 ID 등 상세 절차 구성 | 시험을 수행할 때 필요한 맥락과 결과 확인 기준을 제공 |
| 9. 설명 요약 | 확정된 최종 시험 절차를 기준으로 설명 생성 | 절차 수정 이후 요약에 이전 내용이 남을 가능성을 줄임 |
| 10. 결과 정규화 | JSON 파싱과 필드 자료형 정규화, 성공·실패 상태와 경고·오류 반환 | 후속 워크플로에서 구조화 결과와 검토 정보를 활용 |

공통 `LLMClient`와 병렬 호출 유틸리티를 활용하고, `WorkflowState`에서 선행 에이전트의 산출물을 참조합니다. 생성 결과는 `agent_outputs`에 저장합니다. LLM 호출 또는 파싱 실패 시 해당 단계에 기본 생성 로직을 적용할 수 있도록 구성했으며, 기본값이 사용된 경우와 처리에 실패한 경우를 구분합니다.

### 주요 산출물

| 산출물 | 담는 정보 | 확인할 항목 |
|---|---|---|
| 시나리오 목록 (`scenario_json_list`) | 시험 목적과 참조 요구사항 | 기능 요구사항이 시나리오에 연결됐는가 |
| 테스트 케이스 목록 (`test_case_json_list`) | 시나리오에 속한 개별 검증 항목 | 무엇을 입력하고 무엇을 확인하는가 |
| 시험 절차 목록 (`step_json_list`) | 케이스를 실행하는 단계 | 실행 순서와 케이스 목적이 맞는가 |
| 상세 절차 목록 (`step_detail_json_list`) | 사전조건, 입력값, 예상결과, 화면 ID | 참조 화면과 관찰할 결과가 명확한가 |
| 설명 요약 | 최종 절차의 설명 | 실제 단계와 설명에 모순이 없는가 |
| warnings | 누락 보완, 기본값 적용 등 검토 정보 | 생성 후 사람이 다시 확인할 부분은 무엇인가 |
| errors | 처리 실패 관련 정보 | 어떤 선행 입력 또는 단계가 실패했는가 |
| 실제 시험 결과 (`test_result`) | 시험 실행으로 확인한 값 | 시험 전에는 None으로 유지되는가 |

### 설명용 검토 사례

**사례 A — 요구사항 ID 연결 누락.** 입력에 기능 요구사항이 세 개 있고 결과가 그중 두 개만 참조한다고 가정합니다. 원본 ID와 결과의 참조 ID를 대조해 누락을 확인하고, 해당 요구사항을 위한 시나리오를 보완한 뒤 경고를 남깁니다. 검토자는 새 시나리오가 생겼는지와 함께, 그 시나리오의 조건·입력값·예상결과가 요구사항을 충분히 검증하는지 확인합니다.

**사례 B — 응답 구조 불일치.** 특정 단계의 응답을 JSON으로 파싱할 수 없다면 기본 생성 경로와 연결합니다. 이후 검토에서는 문서가 반환됐는지, 어떤 단계가 기본값으로 채워졌는지, 그 결과가 후속 단계에서 어떤 영향을 주는지 구분합니다.

**사례 C — 시험 절차 상세화.** 화면을 통해 동작을 확인하는 시험이라고 가정합니다. 기본 절차를 만든 뒤 인터페이스 참조로 화면 ID와 확인 항목을 채우고, 확정된 절차에서 설명을 생성합니다. 예상결과는 시험에서 기대하는 동작이며, 실제 결과는 시험 수행 전까지 비어 있습니다.

**개인 기여 요약:** 선행 산출물을 받아 시험 문서로 변환하는 에이전트를 담당했습니다. 입력 검증, 단계별 생성, 요구사항 추적, JSON 정규화, 기본 생성 경로와 경고·오류 반환을 공통 워크플로에 연결했습니다.

## 3. NeuroAge-MAS | 뇌 체적·임상·유전체 연구 플랫폼

**범위:** 표 형식 연구 자료의 입력 검증, 종단 분석, 모델 비교, 불확실성 점검, 내부 검토 및 보고서 생성.

연구 자료를 결합할 때 모델 선택 이전에 대상자 식별 기준, 방문 시점, 단위, 특수 결측 코드, 자료의 출처가 일치하는지 확인해야 합니다. NeuroAge-MAS는 이 확인 과정을 분석과 연결해, 결과를 검토할 때 어떤 입력과 설정이 사용됐는지 되짚을 수 있도록 개발하고 있습니다.

**처리 흐름:** 입력 계약 검증 → 자료 처리 → 종단 분석 및 모델 비교 → 불확실성·분포 점검 → 결과 정합성 확인 → 내부 연구 검토 → 보고서 출력.

### 3.1 입력 계약과 자료 연결

| 검증 기준 | 확인할 내용 | 분석에 미치는 영향 |
|---|---|---|
| 대상자 | 파일 간 식별자가 어떻게 연결되는가 | 서로 다른 대상자의 데이터가 합쳐지면 모든 후속 분석이 달라짐 |
| 방문 | 기준 방문과 추적 방문은 무엇인가 | 방문 순서가 틀리면 변화 방향이 바뀔 수 있음 |
| 날짜·기간 | 방문 간격을 계산할 근거가 있는가 | 기간 확인이 필요한 연간 변화량의 계산 가능 여부가 달라짐 |
| 단위 | 동일 ROI의 부피 단위가 일치하는가 | 단위가 다른 수치를 비교하면 변화량을 해석할 수 없음 |
| 결측 | 코드북의 특수 코드가 어떤 상태를 뜻하는가 | 결측 코드가 실측값으로 섞이면 통계와 모델 입력이 왜곡될 수 있음 |
| 자료 출처 | 코드북과 대상자 매핑을 어디에서 확인하는가 | 자료가 바뀌었을 때 연결 근거와 처리 범위를 다시 검토할 수 있음 |

임상 자료는 코드북에 따라 변수를 해석하고 특수 결측 코드를 처리합니다. 교육용 임상 자료에서는 **당뇨가 처음 확인된 조사일**을 분석합니다. 이 값은 관측 자료에서 확인된 최초 시점이므로, 결과를 읽을 때 실제 발병 시점과 구분합니다.

### 3.2 종단 뇌 체적 분석

동일 대상자의 서로 다른 방문을 비교하고, 관심 영역(ROI)별 절대 변화량과 변화율을 계산합니다. 시간 간격이 확인될 경우에는 연간 변화도 볼 수 있습니다. 입력에 방문 순서만 있고 실제 기간을 뒷받침하는 근거가 없다면 방문 간 변화와 연간 변화는 해석 범위가 다릅니다.

| 지표 | 의미 | 전제 |
|---|---|---|
| 절대 변화량 | 추적 방문 값에서 기준 방문 값을 뺀 값 | 동일 대상자·ROI, 같은 단위 |
| 상대 변화율 | 절대 변화량을 기준 방문 값으로 나눈 비율 | 기준값이 유효하고 0이 아님 |
| 연간 절대 변화 | 절대 변화량을 방문 간 경과 연수로 나눈 값 | 경과 기간이 확인되고 양수임 |

**가상 예시:** 같은 ROI가 기준 방문에서 100 cm³, 2년 후 방문에서 94 cm³라면 절대 변화는 −6 cm³, 상대 변화율은 −6%, 연간 절대 변화는 −3 cm³/년입니다. 이 수치는 계산법 설명용이며 실제 데이터 결과가 아닙니다.

### 3.3 모델 비교와 멀티모달 실험

| 분류 | 모델·방법 | 비교 관점 |
|---|---|---|
| 회귀 | Dummy baseline, Ridge, ElasticNet, Random Forest, SVR, XGBoost | 기준선 대비 차이, 선형·비선형 모델 간 차이 |
| 분류 | Logistic Regression, Random Forest, XGBoost | 같은 데이터 분할에서 모델별 결과 비교 |
| 검증 | 환자 단위 분할, 교차검증 | 같은 환자의 여러 방문이 학습과 평가에 동시에 들어가지 않도록 관리 |
| 전처리 | 학습 fold 내부 전처리 | 전체 데이터로 먼저 통계나 변환을 학습하는 누수 방지 |
| 탐색 | 선택적 Optuna | 하이퍼파라미터 탐색을 별도 설정으로 구분 |
| 조기 결합 | 뇌 체적·임상·유전체 특징을 표 형태로 결합 | 개별 자료와 결합 자료를 비교 |
| 고정 가중치 결합 | 자료별 모델 출력을 지정한 가중치로 합산 | 자료별 예측 기여를 고정 조건에서 비교 |
| OOF stacking | 학습에 쓰이지 않은 fold의 예측을 이용해 결합 모델 구성 | 같은 행으로 학습한 예측값이 결합 학습에 섞이는 문제를 줄임 |
| 결과 해석 | Permutation importance, 선택적 SHAP | 모델이 활용한 특징과 실제 인과 해석을 구분 |

예를 들어 한 대상자의 기준 방문이 학습에 있고 추적 방문이 평가에 있으면, 모델이 사실상 이미 본 대상자를 평가할 수 있습니다. 이를 점검하려면 분할 단위를 데이터 행이 아니라 환자로 설정했는지 확인합니다. 모델의 결과를 비교할 때는 모델 이름뿐 아니라 환자 분할, 전처리 범위, 특징 구성, 실험 설정을 함께 봅니다.

### 3.4 불확실성과 분포 점검

- **Bootstrap:** 재표집을 활용해 추정치의 변동을 살펴봅니다. 반복 방문 자료라면 어떤 단위를 재표집하는지가 해석에 영향을 줍니다.
- **Conformal prediction interval:** 점예측과 함께 예측 구간을 확인하는 방법입니다. 구간의 해석에는 보정 자료와 평가 조건이 필요합니다.
- **데이터 drift 점검:** 학습 시점과 비교 대상 데이터의 입력 분포가 달라졌는지 살펴봅니다. 분포 차이는 추가 검토의 단서가 됩니다.
- **neuroHarmonize ComBat:** 필요한 메타데이터 조건을 충족할 때 연계하는 경로입니다. 어떤 배치 변수와 자료를 사용했는지 확인해야 결과를 해석할 수 있습니다.

### 3.5 유전체 자료 연계

PLINK BED·BIM·FAM 입력 구조를 확인하고 QC·PCA·PRS·GWAS 실행 래퍼를 제공합니다. 유전 PC·PRS의 출처, 유전체 빌드, 대상자 연결 기준을 함께 점검합니다.

| 항목 | 검토 지점 |
|---|---|
| BED·BIM·FAM | 한 세트로 사용할 수 있는 구조인지, 표본과 변이 정보의 연결이 타당한지 |
| QC | 제외 기준과 실행 결과를 어떤 설정으로 해석할 수 있는지 |
| PCA | 유전 PC가 어느 입력과 처리 조건에서 생성됐는지 |
| PRS | 가중치의 출처, 대상자 매핑, 빌드와 입력 자료의 근거가 있는지 |
| GWAS | 실행에 사용한 표현형과 대상자 매핑, 결과 해석 범위가 무엇인지 |

실행에는 별도 PLINK 실행 파일, 검증된 입력, 대상자 매핑이 필요합니다. PRS 경로에는 적절한 가중치와 출처도 필요합니다.

### 3.6 근거 검색, 실행 이력, 보고서

관련 문서 발췌는 TF-IDF와 cosine similarity를 사용하며 검색 결과에 출처와 페이지 정보를 포함합니다. 검색 순위는 관련 문서를 찾는 데 쓰고, 적용 근거는 원문에서 확인할 수 있게 합니다. 역할별 Python 에이전트가 작업과 산출물을 연결합니다.

- 입력·설정·모델·결과의 해시를 기록해 실행에 사용된 자료를 구분합니다.
- 작업 실행 상태와 결과 정합성 검사 상태를 분리합니다. 실행 완료 이후에도 결과 검토가 남아 있을 수 있습니다.
- 내부 연구 검토와 승인 이력을 남깁니다.
- PDF·DOCX·HTML·Markdown·CSV·JSON으로 결과를 출력합니다.
- SQLite와 자체 작업 큐·worker를 사용하며, Redis는 선택적 알림 용도로 구분합니다.

### 3.7 뇌 나이 실험과 연구 범위

Brain Age Gap(BAG)은 예측 뇌 나이에서 실제 나이를 뺀 값입니다. 예를 들어 예측 뇌 나이가 65세이고 실제 나이가 60세라면 BAG는 +5년입니다. 이 값만으로 의료적 해석을 내릴 수는 없으며, 실제 나이 라벨의 기준 시점, 촬영 시점과 특징의 출처를 확인해야 합니다.

SHAP·Optuna·ComBat·PyTorch 실험은 의존성과 설정을 충족한 경우 사용합니다. PyTorch MLP와 CPU 기반 FedAvg는 선택 경로이며, FedAvg는 로컬 시뮬레이션입니다. 외부 LLM 설명 연동과 PostgreSQL 기반 분산 운영은 현재 구현과 구분합니다. 원본 MRI 분할·정합과 3D CNN 학습은 이 플랫폼 범위에 포함되지 않습니다. 합성·교육용·실제 자료를 구분하고, 합성 실험이나 내부 검토 결과를 실제 환자 성능 또는 임상적 유효성으로 해석하지 않습니다.

### 3.8 검토자가 확인할 순서

1. 데이터 출처와 코드북을 확인하고 대상자·방문이 어떤 근거로 연결됐는지 확인합니다.
2. ROI, 부피 단위, 결측 처리, 기간 환산 가능 여부를 확인합니다.
3. 환자 단위 분할과 fold 내부 전처리를 확인한 뒤 모델 결과를 비교합니다.
4. 예측값, 추정치, 예측 구간과 입력 분포 점검 결과를 함께 읽습니다.
5. 실행 기록과 해시로 입력·설정·모델·결과를 연결하고 정합성 검사와 내부 검토 상태를 확인합니다.

### 3.9 기술 구성

| 분야 | 기술 |
|---|---|
| Backend | FastAPI · Pydantic · Uvicorn |
| Frontend | React · TypeScript · Vite · Lucide React |
| Dashboard | Streamlit · Altair |
| Data | Pandas · NumPy · SciPy · openpyxl |
| ML | scikit-learn · XGBoost · Joblib |
| Visualization | Matplotlib · mplot3d · React SVG |
| Reports | ReportLab · python-docx |
| Execution | SQLite · 자체 작업 큐·worker |
| Quality | pytest · FastAPI TestClient · Ruff · pytest-cov · pip-audit |
| Development | GitHub Actions · Dev Container · Vite build |

## 4. MedWatch PMS | 의료기기 시판 후 안전관리

[![Repository](https://img.shields.io/badge/GitHub-medical--divice--pms-181717?style=flat-square&logo=github)](https://github.com/junhaj27-jpg/medical-divice-pms)

**범위:** 고객 불만, 이상사례 판단, 위험평가, CAPA, 보고 검토와 리콜을 사건 단위로 연결하는 RA·QA 포트폴리오 프로젝트.

이 프로젝트는 사건을 처리할 때 **누가, 어느 시점에, 어떤 자료와 규칙을 근거로 판단했는지** 확인할 수 있도록 업무 흐름을 구성합니다. 불만 기록과 CAPA, 규제보고 검토와 회수 진행 상황이 흩어져 있으면 후속 담당자가 이전 판단을 되짚기 어렵습니다. 사건 기록에 각 단계와 근거를 연결해 업무 인계와 검토를 지원합니다.

**대표 흐름:** 불만 접수 → 이상사례 판단 → 위험평가 → CAPA 검토·등록 → 규제보고 검토 → 리콜 검토 → 승인 → 조치 완료와 종료.

### 4.1 접수, 업무 상태, 접근 권한

- 단계별 상태 전이와 선행조건을 검증합니다.
- STAFF·RA_QA·ADMIN 역할별로 업무 범위를 구분합니다.
- STAFF는 본인이 접수한 사건을 조회하는 범위로 제한합니다.
- 화면과 API에서 개별 사건에 대한 접근 권한을 검사합니다.
- 담당자, 기한, 개인별 할 일과 알림을 사건 진행과 연결합니다.

업무 상태는 사건이 어느 단계인지 보여주고, 권한은 해당 기록을 조회하거나 조치할 수 있는 사람이 누구인지 정합니다. 같은 단계의 사건이라도 접근 가능한 사용자는 달라질 수 있습니다.

### 4.2 위험평가와 CAPA

심각도와 발생 가능성에 따라 위험점수와 등급을 계산하고, 제품·LOT별로 반복되는 불만을 탐지합니다. 고위험 사건에서는 CAPA 등록의 선행조건을 검증합니다. CAPA에는 원인 분석, 시정·예방조치, 증빙, 효과성 평가와 미흡 시 재조치 이력을 연결합니다. 위험점수와 반복 불만 탐지 기준은 시연용 내부 규칙입니다.

**가상 사례:** 같은 제품 LOT에서 유사 불만이 반복된다면 검토자는 사건별 위험점수뿐 아니라 반복 불만을 연결한 기준을 확인합니다. CAPA가 등록된 경우 원인 분석이 조치 내용으로 이어지는지, 증빙이 있으며 효과성 평가 결과에 따라 재조치가 연결되는지를 검토합니다.

### 4.3 규정 문서와 보고 규칙

| 단계 | 구현 내용 | 남는 근거 |
|---|---|---|
| 문서 관리 | PDF·TXT 규정 문서의 출처·버전·시행일 관리 | 어떤 원문을 참조했는지 확인 |
| 근거 검색 | 페이지·절·문단 단위 로컬 검색 | 규칙의 근거가 된 위치를 확인 |
| 규칙 작성 | 원문 인용과 담당자의 해석을 연결 | 근거 문장과 업무상 적용 기준을 구분 |
| 검토와 승인 | 초안·검토·승인·시행·폐기 상태, 작성자와 승인자 분리 | 누가 작성하고 검토했는지 확인 |
| 버전 비교 | 버전별 차이와 변경 이력 보존 | 변경된 조건과 이전 버전의 관계를 확인 |
| 계산 미리보기 | 해당 입력으로 보고 기한 계산 확인 | 사건 적용 전에 조건과 계산값을 검토 |
| 사건 적용 | 사건에 규칙을 명시적으로 적용 | 적용 당시 규칙 버전·입력·계산 결과 스냅샷 |

규칙을 조회한 기록과 사건에 규칙을 실제로 적용한 기록을 구분합니다. 이후 규칙이 개정되어도 이전 사건의 판단을 확인할 때에는 적용 당시 기록을 기준으로 추적할 수 있습니다. 자동으로 법정 기한이나 공휴일을 제공하거나 실제 규제기관 제출을 수행하는 범위는 아닙니다.

### 4.4 리콜과 회수 관리

제품·UDI·LOT·시리얼을 추적하고 거래처별 통보, 회신, 부분 회수 이력을 기록합니다. 회수 수량을 검증하고 회수율을 계산하며, 미회수 사유와 후속 연락도 남깁니다. 승인·반려 이력과 종료 보고서가 사건에 연결됩니다.

예를 들어 회수 대상이 100개이고 거래처별 확인 수량의 합계가 70개인 가상 상황에서는, 집계값 70%와 함께 남은 30개가 어느 거래처에 해당하는지, 미회수 사유와 후속 연락 기록이 있는지를 확인합니다. 이 숫자는 부분 회수와 잔여 수량을 설명하기 위한 예입니다.

### 4.5 RA 도우미, 감사 기록, 증빙

- 사용자가 접근 가능한 사건에서 진행 상태, 고위험 사건, 기한 초과 현황을 조회합니다.
- CAPA·리콜 진행 상황과 업무 절차를 안내합니다.
- 사용자별 대화를 분리하고 직접 식별정보 입력을 차단합니다.
- 승인 요청 시점 자료를 스냅샷으로 남기고 주요 업무 감사 로그를 기록합니다.
- 증빙 파일 검사 상태에 따라 접근을 제한합니다.
- 서버에서 PDF를 생성하고 보고서 버전을 보존합니다.

기본 RA 도우미는 로컬 규칙 기반입니다. 외부 AI 어댑터 구조는 실제 공급자 연동과 검증을 마친 기능과 구분합니다.

### 4.6 사건 하나를 검토할 때

| 검토 질문 | 열어볼 기록 |
|---|---|
| 어떤 제품과 LOT에서 발생했는가 | 접수 정보, 관련 제품, LOT, 반복 불만 기록 |
| 위험도는 무엇을 근거로 정했는가 | 심각도·발생 가능성, 적용 기준, 산정 결과 |
| 원인과 조치가 이어지는가 | CAPA 원인 분석, 조치, 증빙, 효과성 평가 |
| 보고 기한은 어떤 규칙으로 계산했는가 | 승인된 규칙 버전, 원문 근거, 입력·결과 스냅샷 |
| 회수는 얼마나 진행됐는가 | 거래처별 통보·회신, 부분 회수, 잔여 수량, 미회수 사유 |
| 누가 무엇을 보고 승인했는가 | 승인 요청 시점 자료, 승인·반려 이력, 감사 로그 |
| 종료 보고서는 어떤 상태를 담았는가 | 종료 시점 기록과 보고서 버전 |

### 4.7 기술 구성

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Django](https://img.shields.io/badge/Django-092E20?style=flat-square&logo=django&logoColor=white)
![DRF](https://img.shields.io/badge/DRF-A30000?style=flat-square)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Chart.js](https://img.shields.io/badge/Chart.js-FF6384?style=flat-square&logo=chartdotjs&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)

### 4.8 고도화 목표

| 주제 | 검토 중인 방향 |
|---|---|
| 규정 개정 영향 분석 | 변경된 규칙과 관련 사건을 연결하고 기한 변화 예상값과 검토 업무를 표시 |
| 승인 무결성 | 승인 대상 자료 변경 감지, 재승인, 동시 처리 시 결과 검증 |
| 안전 신호 분석 | 제품·LOT별 불만 추세와 탐지 사유 표시 |
| 근거 기반 RA 도우미 | 검색한 실제 근거를 인용해 검토에 사용할 수 있는 답변 제공 |
| 독립 검증 에이전트 | 요구사항 대조, 결함 재현, 회귀 검증 |

이 항목들은 고도화 목표입니다. 프로젝트는 실제 규제기관 제출, 규정 준수 판단, 의료 판단을 자동 보장하지 않습니다.

## 5. Brain MRI | 3D 시각화와 마스크 기반 부피 측정

[![Repository](https://img.shields.io/badge/GitHub-mri-181717?style=flat-square&logo=github)](https://github.com/junhaj27-jpg/mri)

**범위:** DICOM·NIfTI MRI를 불러와 2D 슬라이스, 마스크, 부피, 3D 표면을 검토하는 연구용 웹 프로토타입. NeuroAge-MAS가 이미 정리된 표 형식 특징을 처리한다면, 이 프로젝트는 원본 영상과 공간 정보부터 다룹니다.

**처리 흐름:** 영상 로딩 → 강도 전처리와 슬라이스 확인 → 마스크 처리 → 품질 점검 → 부피 계산 → 3D 메시 → 결과 내보내기와 PDF.

### 5.1 영상 로딩과 공간 정보

DICOM 시리즈를 찾아 3D 볼륨을 구성하고, NIfTI 영상과 마스크를 불러옵니다. 영상 배열과 함께 affine, voxel spacing, 메타데이터를 관리합니다. NIfTI의 방향을 표준화하고 분석용 데이터를 저장합니다.

| 정보 | 의미 | 확인이 필요한 이유 |
|---|---|---|
| 배열 | 영상의 voxel 강도나 마스크 label을 담는 격자 | 영상과 마스크의 형상과 인덱스를 비교 |
| 방향 | 배열의 각 축이 영상 공간에서 향하는 방향 | 평면 표시와 오버레이 해석 |
| affine | voxel 좌표를 실제 영상 공간과 연결하는 변환 | 인덱스가 같아도 영상과 마스크의 물리적 위치가 다를 수 있음 |
| voxel spacing | 축별 voxel 간격 | 부피와 메시의 물리적 크기 계산 |
| 시리즈 구성 | 하나의 볼륨을 구성하는 슬라이스 집합 | 볼륨을 구성할 자료가 적절한지 확인 |

### 5.2 전처리와 2D 검토

영상 강도를 백분위수 기준으로 클리핑하고 정규화합니다. Axial·Coronal·Sagittal 슬라이스를 추출하고 마스크를 오버레이해 브라우저에서 처리 상태와 함께 확인합니다. 한 평면에서 적절해 보이는 마스크도 다른 평면에서 경계가 어긋날 수 있으므로 여러 방향에서 영상과 마스크의 관계를 봅니다.

### 5.3 마스크 처리와 품질 점검

뇌 추출 도구 실행 경로와 결과 마스크 로딩을 연계합니다. 마스크의 연결 요소와 경계 접촉 등을 진단하고, 신뢰 가능한 처리 경로와 임계값을 사용한 디버그 결과를 구분합니다. 마스크 상태에 따라 최종 3D 생성이 제한됩니다.

- **연결 요소:** 큰 영역과 작은 조각이 어떻게 나뉘는지 확인합니다. 작은 영역이 많으면 마스크 품질을 다시 검토할 단서가 됩니다.
- **경계 접촉:** 마스크가 영상 경계에 닿는 위치와 범위를 봅니다. 경계에 닿았다는 사실만으로 마스크 오류를 확정할 수는 없습니다.
- **오버레이:** 배열 크기뿐 아니라 실제 공간에서 영상과 마스크가 맞는지 검토합니다.
- **마스크 종류:** 뇌 추출 마스크와 병변 마스크는 목적이 다르므로 별도로 분석합니다. 밝기 임계값 기반 후보 영역은 종양 진단 결과가 아닙니다.
- **외부 연계:** HD-BET·SynthSeg 경로에는 도구 설치와 실행 환경이 필요합니다.

### 5.4 전체·영역별 부피

선택한 마스크에 포함되는 voxel 수를 세고, 한 voxel의 물리적 부피를 곱합니다. 영역별 labelmap에서는 label을 구분해 부피를 집계하고 CSV로 내보냅니다.

**부피(cm³) = 마스크 voxel 수 × voxel 부피(mm³) ÷ 1,000**

| 가상 입력 | 계산 | 결과 |
|---|---|---|
| 20,000 voxel, spacing 1 × 1 × 1 mm | 20,000 × 1 ÷ 1,000 | 20 cm³ |
| 20,000 voxel, spacing 0.5 × 0.5 × 2 mm | 20,000 × 0.5 ÷ 1,000 | 10 cm³ |

같은 voxel 수라도 spacing에 따라 결과가 달라집니다. 위 예시는 축별 spacing을 곱해 voxel 부피를 구할 수 있는 격자를 가정합니다. 결과를 검토할 때는 입력 마스크, 선택한 label, spacing과 단위를 함께 확인합니다.

### 5.5 3D 메시와 내보내기

Marching Cubes를 사용해 마스크 표면을 추출하고, 다운샘플링·평활화와 메시 후처리를 적용합니다. 연결 요소와 메시 품질을 점검하고 Three.js·Plotly로 시각화합니다. GLB·STL과 결과 PDF를 내보낼 수 있습니다. PDF에는 슬라이스, 마스크, 부피 결과를 포함합니다.

메시를 검토할 때는 화면에서 표면이 매끄럽게 보이는지와 더불어, 입력 마스크와 후처리 조건이 무엇인지 확인합니다. 부피 집계의 근거는 마스크의 voxel과 공간 정보이며, 시각화용 메시의 외형과 구분합니다.

### 5.6 주요 코드 구성

| 파일 | 역할 |
|---|---|
| mri_loader.py | DICOM·NIfTI 로딩, 볼륨과 영상 정보 관리 |
| preprocessing.py | 강도 정규화와 평면별 슬라이스 추출 |
| brain_mask.py | 뇌 마스크 생성·보정 |
| skull_stripping.py | 뇌 추출 처리 |
| region_segmentation.py | 외부 영역 분할 연계, labelmap과 부피 집계 |
| mesh_builder.py | 3D 메시 생성·후처리·내보내기 |
| backend/server.py | 웹 요청과 영상 처리 연결 |
| report.py | PDF 보고서 생성 |

### 5.7 검토 순서

1. 영상과 마스크의 출처, 배열, 방향, affine, spacing을 확인합니다.
2. 세 평면에서 마스크가 의도한 영역과 겹치는지 확인합니다.
3. 연결 요소와 경계 접촉 상태를 보고 마스크 처리 경로를 확인합니다.
4. label별 voxel 집계와 단위 환산이 맞는지 확인합니다.
5. 메시 후처리 설정과 GLB·STL, CSV·PDF의 산출물을 확인합니다.

이 프로젝트는 연구·포트폴리오용 프로토타입이며, 영상 결과를 진단이나 치료 효과 판정에 사용하지 않습니다.

### 5.8 기술 구성

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white)
![pydicom](https://img.shields.io/badge/pydicom-3776AB?style=flat-square)
![NiBabel](https://img.shields.io/badge/NiBabel-4C72B0?style=flat-square)
![scikit-image](https://img.shields.io/badge/scikit--image-F7931E?style=flat-square)
![Plotly](https://img.shields.io/badge/Plotly-3F4F75?style=flat-square&logo=plotly&logoColor=white)
![Three.js](https://img.shields.io/badge/Three.js-000000?style=flat-square&logo=threedotjs&logoColor=white)

## 6. 네 프로젝트를 관통하는 개발 방식

| 관점 | ALPLED | NeuroAge-MAS | MedWatch PMS | Brain MRI |
|---|---|---|---|---|
| 입력 근거 | 기능 요구사항과 인터페이스 | 대상자·방문·단위·코드북 | 사건·제품·규정 출처 | 영상 시리즈·공간 정보·마스크 |
| 추적 대상 | 요구사항 → 시나리오 → 케이스 | 입력·설정 → 실행 → 결과 | 사건 → 판단 → 조치·승인 | 원본 영상 → 마스크 → 부피·메시 |
| 대표 검증 | 참조 ID 대조와 파싱 | 환자 분할·fold 내부 전처리·정합성 | 권한·선행조건·규칙 적용 이력 | 오버레이·연결 요소·spacing |
| 결과 구분 | 예상결과와 실제 시험 결과 | 분석 실행과 연구 검토 | 계산 미리보기와 사건 적용 | 디버그 마스크와 최종 3D 생성 |
| 남기는 자료 | 구조화 시험 문서, 경고·오류 | 실행 기록, 결과 해시, 보고서 | 감사 로그, 규칙·승인 스냅샷 | CSV, 3D 파일, PDF |

작업을 시작할 때는 해결할 문제와 입력 조건, 완료 기준을 정리합니다. 이후 입력과 결과 사이에 어떤 식별자나 기록을 남겨야 하는지 정하고, 입력 오류·실행 실패·근거 부족·검토 대기처럼 원인이 다른 상태를 구분합니다. AI가 작성한 코드와 문서는 실행 및 테스트, 내용 검토를 통해 확인합니다. 팀 작업에서는 전체 프로젝트 구성과 개인 담당 영역을 분리해 설명합니다.

## 7. 기타 교육 프로젝트

| 프로젝트 | 주제 |
|---|---|
| **SKN24-1st-Team** | 지역별 자동차 등록·교통사고 현황 분석 |
| **SKN24-2nd-4Team** | 패션 산업 고객 이탈 예측 모델 개발 |
| **SKN24-3rd-1Team** | 조선 왕 캐릭터 AI 챗봇 |
| **SKN24-4rd-1Team** | 조선 왕 캐릭터 AI 챗봇 고도화 |
| **SKN24-5rd-3Team** | ALPLED · 통합시험 시나리오 생성 에이전트 |

세부 담당 범위, 사용 기술, 결과 수치는 확인 가능한 자료를 기준으로 추후 보강할 항목입니다.

## 8. 현재 정리하고 있는 과제

- **LLM 생성 품질:** 요구사항과 테스트 케이스의 연결을 문서화하고, 생성 결과의 품질 평가와 오류 대응을 보강합니다.
- **연구 자료 연결:** 뇌 체적·임상·유전체 자료의 연결 근거, 모델 비교 조건과 불확실성 분석을 정리합니다.
- **PMS 업무 추적:** 규정 개정의 영향과 승인 자료 변경 검증을 고도화 과제로 관리합니다.
- **독립 검증:** 결함을 재현하고 수정 후 같은 조건에서 다시 확인하는 회귀 검증 흐름을 정리합니다.
- **포트폴리오 증빙:** 프로젝트마다 개인 기여, 확인 가능한 산출물, 재현 조건과 검토 사례를 연결합니다.

## 9. 관심 직무 및 분야

- AI 에이전트와 LLM 응용 서비스 개발
- 헬스케어 데이터 분석과 연구 지원 도구
- 의료 AI 연구·개발 및 의료영상 처리
- 의료기기 QA·PMS 업무 자동화
- 규정 원문과 업무 판단을 연결하는 검토 지원 시스템

## 10. 연락처와 저장소

- 성명: 정준하
- GitHub 계정: [junhaj27-jpg](https://github.com/junhaj27-jpg)
- 저장소: [MedWatch PMS](https://github.com/junhaj27-jpg/medical-divice-pms) · [Brain MRI](https://github.com/junhaj27-jpg/mri)
- 교육 기수·팀 코드: SKN24 · 기타 교육 프로젝트 표 참조

[![GitHub](https://img.shields.io/badge/GitHub-junhaj27--jpg-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/junhaj27-jpg)

프로젝트의 구현 과정과 검증 기록을 GitHub에 정리하고 있습니다.

