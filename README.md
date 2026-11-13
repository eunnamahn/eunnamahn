<h2 align="center">안녕하세요, AI 엔지니어 안은남입니다 👋</h2>
<p align="center">
  <b>LLM의 답이 맞는지 측정하는 AI 엔지니어</b><br/>
  골든셋과 검증기로 RAG · LLM 서비스의 신뢰성을 만듭니다.
</p>

<p align="center">
  <a href="https://eunnamahn.github.io"><img src="https://img.shields.io/badge/웹사이트-eunnamahn.github.io-1F4E8C?style=flat-square&logo=githubpages&logoColor=white"/></a>
  <a href="https://eunnamahn.github.io/en/"><img src="https://img.shields.io/badge/English-Website-1F4E8C?style=flat-square"/></a>
  <a href="https://www.linkedin.com/in/eunnamahn/"><img src="https://img.shields.io/badge/LinkedIn-eunnamahn-0A66C2?style=flat-square&logo=linkedin&logoColor=white"/></a>
  <a href="mailto:baduk89@hanmail.net"><img src="https://img.shields.io/badge/Email-baduk89%40hanmail.net-555555?style=flat-square&logo=maildotru&logoColor=white"/></a>
  <img src="https://img.shields.io/badge/TOEIC-985%2F990-555555?style=flat-square"/>
</p>

---

### 🙋 소개
- 수학적 모델을 만들고 **그 결과를 믿어도 되는지 검증하던 연구자**였습니다. 실제 서비스로 사람에게 닿는 일을 하고 싶어 AI 엔지니어로 전환했습니다.
- **평가 기준을 먼저 세우고, 그 기준을 코드로 구현합니다.** 중요한 판단은 규칙 기반 코드가 내리고, LLM은 그 결과를 설명만 하며, 답변은 검증기를 거칩니다.
- 미국 **펜실베이니아 주립대**에서 9년간 영어로 연구하고 논문을 쓰고 학부 수업을 가르쳤습니다.
- 코드잇 스프린트 AI 엔지니어 과정 6개월 동안 팀 프로젝트 3회와 해커톤 1회에 참여하며 **팀장을 3회 역임**했습니다.

> 해석해로 시뮬레이터를 검증하던 일과 골든셋으로 LLM을 검증하는 일은 같은 질문에서 출발합니다.

### 📏 일하는 방식 — 프로젝트마다 먼저 정한 기준

| 프로젝트 | 먼저 정한 기준 | 결과 |
|---|---|---|
| SAVERS | 보호자 응답 골든셋 40건 + 적대 회귀 12건, 거절을 **양쪽 방향**으로 측정 | 적대 12/12 차단, **과소거절 100% 발견** |
| 입찰메이트 | 5유형 95문항 골든셋과 유형별 채점 기준 | 708개 조합 비교, MRR 0.65 → 0.977 |
| AI 광고 스튜디오 | 제품 보존율을 1순위 지표로, 원본 제품을 배경 위에 합성 | CLIP 유사도 ≥ 0.85, 대표 4건 통과 |
| PillScope | 촬영 옵션만 다른 사진을 같은 split으로 묶어 누수 방지 | Kaggle mAP@[.75:.95] 0.936 |

### 📄 논문
- **재난 취약계층을 위한 근거 기반 대피 안내 서비스의 설계 및 구현.**
  한국정보처리학회 학술대회(ACK 2026), KIPS_C2026B0142 · *제1저자 · 구두발표(2026.11.06)*
- **Multi-Well Analytical Solution for Coning Under Simultaneous Steady-State Flow of Three Phases.**
  SPE Improved Oil Recovery Conference, 2018 · *제1저자 · 영문* · [doi.org/10.2118/190182-MS](https://doi.org/10.2118/190182-MS)

### 🎯 프로젝트

**[SAVERS](https://github.com/eunnamahn/savers-project) · 재난 취약계층 맞춤 대피 안내** 🏆 — 2026.07–09 · 팀장 · PM · QA/보안 · 인프라 (4인)
- 대피소·도보 경로는 OSMnx·NetworkX **규칙 코드가 결정**하고, LLM은 정해진 결과를 설명만 하는 구조
- 검증기를 검증할 평가셋을 명세만 보고 직접 작성: 보호자 응답 골든셋 **40건**, 적대 회귀 **12건**, 채점 스크립트
- 정답 답변 **35/35** 검증기 통과 · 오답 유도 **12/12** 차단 (처음 8/12 → 뚫린 4건 분석해 채점기 보강)
- 거절이 정답인 대조군 6건을 넣어 **과소거절 100%(0/6)**를 발견, 원인을 검증기가 아닌 앞단 검색으로 특정
- 지인 52명 설문: 행동 명확성 **3.2 → 8.3점**(10점 만점, Wilcoxon p<0.001), "5분 안에 집을 나서겠다" 13% → 60%
- 고용노동부장관상(장려상, **326팀 중 3위**) · ACK 2026 제1저자
- 내가 쓴 코드: 평가 코드([`apps/ai-engine/eval`](https://github.com/eunnamahn/savers-project/tree/main/apps/ai-engine/eval)), FCM 실발송 [#214](https://github.com/team-savers/savers-project/pull/214) · [#215](https://github.com/team-savers/savers-project/pull/215), AWS EC2 배포

`FastAPI` `LangChain` `OSMnx` `NetworkX` `AWS EC2` `FCM`

**[입찰메이트](https://github.com/eunnamahn/bidmate-rfp-rag) · 공공 RFP 문서 RAG 질의응답·요약** — 2026.06–07 · 평가 담당 (5인)
- K-means로 대표 문서를 골라 골든셋 50건 제작 → **5유형 95문항**으로 확장, 유형별 채점 스크립트 구현
- 검색·답변 설정 **708개 조합**을 같은 골든셋으로 3단계 비교: **MRR 0.65 → 0.977**, 거절 정확도 0.91 → 1.0
- OpenAI 대신 KURE-v1 + EXAONE 3.5 로컬 스택: 평균 응답 **11.3초 → 3.6초**, API 비용 0원
- 점수가 0.3에서 멈춘 원인이 모델이 아닌 **골든셋 오류**임을 찾아 수정, Ollama 컨텍스트 4K → 8K로 근거 잘림 해결, 지연만 6.75배 늘린 리랭커 제거
- 내가 쓴 코드: 골든셋·전처리 실험([`experiments/`](https://github.com/eunnamahn/bidmate-rfp-rag/tree/main/experiments))

`LangChain` `LangGraph` `FAISS` `KURE-v1` `EXAONE 3.5` `RAGAS`

**[AI 광고 스튜디오](https://github.com/eunnamahn/ad-creative-studio) · 소상공인용 광고 이미지·문구 생성** — 2026.08 · 팀장 · PM · 평가 기준 설계 (5인)
- **제품 보존율을 1순위 지표**로 정의, 마스크 영역 CLIP 유사도 ≥ 0.85 + 육안 재검수로 대표 조합 **4/4** 통과
- 4주 스프린트 운영, 최종 보고서 총괄
- 팀 성과: LCM-LoRA로 배경 생성 17.47초 → 1.72초, 자동화 테스트 486건 통과
- 내가 쓴 문서: 평가 기준 [`eval/eval_criteria.md`](https://github.com/eunnamahn/ad-creative-studio/blob/main/eval/eval_criteria.md)

`SDXL` `ControlNet` `IP-Adapter` `FastAPI` `GCP L4`

**[PillScope](https://github.com/eunnamahn/OralMedicineImageDetection) · 경구약제 이미지 객체 탐지** — 2026.04–05 · 팀장 · PM · 모델 실험 (5인)
- 비슷한 56종, 학습 이미지 186장, 클래스 불균형 51배 → 비슷한 사진을 같은 split으로 묶어 **데이터 누수 방지**
- Crop & Paste 증강으로 **186 → 1,026장**, mAP@0.5 0.886 → 0.964, 탐지 못 하던 희귀 클래스까지 탐지
- 4종 모델 7단계 실험, YOLOv11l로 Kaggle mAP@[.75:.95] **0.851 → 0.936** (RF-DETR 0.882, RT-DETRv2 0.883)
- 내가 쓴 코드: COCO → YOLO 파이프라인, EDA·전처리·증강 노트북([`members/eunnam`](https://github.com/eunnamahn/OralMedicineImageDetection/tree/main/members/eunnam))

`YOLOv11` `RT-DETRv2` `RF-DETR` `COCO`

**생의학 논문 초록 문장 분류 · BERT vs. SciBERT** — 2019 · Penn State 딥러닝 수업, 2인 팀(동일 기여)
- BiLSTM-CRF의 Word2Vec 임베딩을 SciBERT로 교체해 임베딩 크기 **약 1/175**로 정확도 유지(92.35% → 92.43%)

`TensorFlow`

### 🔬 대학원 연구 (펜실베이니아 주립대)
- **시공간 저류층 데이터와 딥러닝(Seq2Seq-LSTM)을 활용한 원유 생산량 예측** (박사 연구, 2021–2024): 운영 조건이 바뀔 때의 생산량 예측, 유전 알고리즘으로 튜닝해 테스트 **R² 0.81 이상**
- **실험계획법(DOE)을 결합한 인공신경망 대리 모델 개발** (박사 연구, 2019–2020): 느린 저류층 시뮬레이션을 대신하는 모델, 테스트 **평균 오차 2% 미만, 최대 8% 미만**
- **물·가스 유입 현상(코닝)의 수학 공식 유도** (석사 논문 · SPE 2018 제1저자, 2015–2018): 시뮬레이션 없이 계산하는 해석해를 **6가지 유정 배치**로 확장, 수치 시뮬레이터 검증 기준으로 제시
- **원유·물·가스 흐름 시뮬레이터** (수업 프로젝트, 2016): MATLAB 약 1,000줄로 **처음부터 구현**, Newton-Raphson · GMRES, 매 스텝 질량 보존 검사로 수치 오류 감지

### 💼 희망 직무
`LLM 평가와 신뢰성` `RAG 시스템 설계와 개선` `에이전트 안전장치`

### 🛠️ 기술
**AI · LLM**<br/>
<img src="https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white"/>
<img src="https://img.shields.io/badge/LangGraph-1C3C3C?style=flat-square&logo=langgraph&logoColor=white"/>
<img src="https://img.shields.io/badge/OpenAI-412991?style=flat-square&logo=openai&logoColor=white"/>
<img src="https://img.shields.io/badge/FAISS-0467DF?style=flat-square"/>
<img src="https://img.shields.io/badge/EXAONE%203.5-A50034?style=flat-square"/>
<img src="https://img.shields.io/badge/YOLO-111F68?style=flat-square"/>
<img src="https://img.shields.io/badge/Stable%20Diffusion-SDXL-7B3FE4?style=flat-square"/>

**평가 · 품질**<br/>
<img src="https://img.shields.io/badge/골든셋%20설계-1F4E8C?style=flat-square"/>
<img src="https://img.shields.io/badge/주장%20단위%20검증-1F4E8C?style=flat-square"/>
<img src="https://img.shields.io/badge/RAGAS-1F4E8C?style=flat-square"/>
<img src="https://img.shields.io/badge/pytest-0A9EDC?style=flat-square&logo=pytest&logoColor=white"/>
<img src="https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white"/>

**백엔드 · 인프라**<br/>
<img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white"/>
<img src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white"/>
<img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white"/>
<img src="https://img.shields.io/badge/AWS%20EC2-FF9900?style=flat-square&logo=amazonec2&logoColor=white"/>
<img src="https://img.shields.io/badge/GCP-4285F4?style=flat-square&logo=googlecloud&logoColor=white"/>
<img src="https://img.shields.io/badge/FCM-FFCA28?style=flat-square&logo=firebase&logoColor=black"/>

**ML · 수리 · 데이터**<br/>
<img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white"/>
<img src="https://img.shields.io/badge/TensorFlow-FF6F00?style=flat-square&logo=tensorflow&logoColor=white"/>
<img src="https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white"/>
<img src="https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white"/>
<img src="https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white"/>
<img src="https://img.shields.io/badge/MATLAB-0076A8?style=flat-square"/>
<br/>해석해 유도(라플라스 방정식·중첩 원리) · 실험계획법(DOE) · 인공신경망 대리 모델 · 유전 알고리즘 · Seq2Seq-LSTM 시계열 예측 · PDE 수치해석·시뮬레이션

### 🎓 학력 · 교육
- **펜실베이니아 주립대학교 (미국)** · 에너지광물공학 박사과정 수료 (부전공: 통계학, 계산과학 · GPA 3.81/4.00) · 2018–2024
- **펜실베이니아 주립대학교 (미국)** · 에너지광물공학 석사(석유천연가스공학 세부전공 · GPA 3.71/4.00) · 2015–2018
- **한양대학교** · 자원환경공학과 학사 · 학과 수석(33명 중 1위), 제2공과대학 차석 졸업 · 2009–2015
- **코드잇 스프린트** · AI 엔지니어 10기 수료 · 2026

### 🏅 수상 · 활동
- 고용노동부장관상(장려상), 제8회 K-디지털 트레이닝 해커톤 (326팀 중 3위) · 2026
- EME 올해의 대학원 조교상, 펜실베이니아 주립대 (학과 조교 약 60명 중 1명) · 2017
- 대학원 학생회 공동회장, College of Earth and Mineral Sciences, 펜실베이니아 주립대 · 2019–2024
- 대학생 논문 공모전 3회 입상 (GS에너지 3위, 한국광해관리공단·한국환경산업기술원 2위) · 2013–2014
- 국가 이공계 장학금, 4학기 전액 · 2013–2014

### 📜 자격증
- TOEIC 985 / 990 (Listening 490, Reading 495) · 2026
- 데이터분석 준전문가(ADsP), 한국데이터산업진흥원 · 2026
- Engineer in Training(EIT), 미국 NCEES FE 시험 합격 · 2017
