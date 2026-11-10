<h2 align="center">안녕하세요, AI 엔지니어 안은남입니다 👋</h2>
<p align="center">
  <b>AI 엔지니어 · LLM / RAG · 평가 설계</b><br/>
  LLM이 내놓은 답을 근거와 맞춰 보고, 근거가 없으면 내보내지 않는 시스템을 만듭니다.
</p>

<p align="center">
  <a href="https://eunnamahn.github.io"><img src="https://img.shields.io/badge/웹사이트-eunnamahn.github.io-1F4E8C?style=flat-square&logo=githubpages&logoColor=white"/></a>
  <a href="https://eunnamahn.github.io/en/"><img src="https://img.shields.io/badge/English-Website-1F4E8C?style=flat-square"/></a>
  <a href="mailto:baduk89@hanmail.net"><img src="https://img.shields.io/badge/Email-baduk89%40hanmail.net-555555?style=flat-square&logo=maildotru&logoColor=white"/></a>
  <img src="https://img.shields.io/badge/TOEIC-985%2F990-555555?style=flat-square"/>
</p>

---

### 🙋 소개
- **검증할 수 있는** LLM 서비스를 만듭니다. 중요한 판단은 규칙 기반 코드가 내리고, LLM은 그 결과를 설명만 하며, 모든 답변은 검증기를 거칩니다.
- 미국 **펜실베이니아 주립대** 석사·박사과정에서 수학·통계 모델을 만들고 실제 데이터로 검증하는 연구를 했습니다.
- 영어로 논문을 쓰고 **영어로 학부 수업 조교**를 맡았습니다.
- 코드잇 스프린트 AI 엔지니어 과정에서 프로젝트 4개 중 3개를 팀장으로 이끌었습니다.

### 📄 논문
- **재난 취약계층을 위한 근거 기반 대피 안내 서비스의 설계 및 구현.**
  한국정보처리학회 학술대회(ACK 2026) · *제1저자 · 구두발표(2026.11.06)*
- **Multi-Well Analytical Solution for Coning Under Simultaneous Steady-State Flow of Three Phases.**
  SPE Improved Oil Recovery Conference, 2018 · *제1저자 · 영문* · [doi.org/10.2118/190182-MS](https://doi.org/10.2118/190182-MS)

### 🎯 프로젝트

**[SAVERS](https://github.com/team-savers/savers-project) · 재난 취약계층 맞춤 홍수 대피 안내** 🏆 — 2026 · 팀장
- 기록에 없는 내용 0건: 실제 응답 **30/30** 통과, 오답 유도 질문 **12/12** 차단
- 주민 52명 설문에서 대피 의향 **3.2 → 8.3** (p<0.001), 고용노동부장관상(장려상)

`FastAPI` `LangChain` `NetworkX` `AWS EC2`

**[입찰메이트](https://github.com/Eastar0102/codeit-part3-team1) · 공공 RFP 문서 RAG 질의응답** — 2026 · 평가 담당
- 평가용 질문 95개(골든셋)로 검색·답변 설정 **708개 조합** 비교
- 최종 무료 로컬 조합: **MRR 0.977**, 거절해야 할 질문 **19/19** 거절, 응답 **3.6초**, API 비용 0원

`LangChain` `LangGraph` `FAISS` `KURE-v1` `EXAONE 3.5`

**[AI 광고 스튜디오](https://github.com/codeit-part4-team2/ad-creative-studio) · 소상공인용 광고 이미지·문구 생성** — 2026 · 팀장
- 제품이 바뀌지 않았는지 자동 검사(CLIP ≥ 0.85) 후 사람이 보는 **2단계 품질 관문**, 대표 조합 4/4 통과
- 배경 생성 **17.47초 → 1.72초(약 10배)**, 자동화 테스트 **486건** 통과

`SDXL` `ControlNet` `IP-Adapter` `FastAPI` `GCP`

**[PillScope](https://github.com/qja0707/OralMedicineImageDetection) · 경구약제 이미지 객체 탐지** — 2026 · 팀장
- 비슷한 56개 클래스, 이미지 **186장 → 오려 붙이기 증강으로 1,026장**, 희귀 알약까지 탐지
- 최종 mAP **0.936**, 모델 3개 앙상블로 수업 내 Kaggle 대회 **0.851 → 0.9355**

`YOLOv11` `RT-DETRv2` `RF-DETR`

**생의학 논문 초록 문장 분류 · BERT vs. SciBERT** — 2019 · 딥러닝 수업 프로젝트, 2인 팀
- BERT·SciBERT 임베딩으로 Word2Vec을 대체해, 임베딩 크기를 **약 1/175**로 줄이고도 같은 수준의 정확도 유지

`TensorFlow`

### 🔬 대학원 연구 (펜실베이니아 주립대)
- **원유 생산 모델의 확률적 보정** (박사 연구, 2021–2024): 몬테카를로 시뮬레이션·실험계획법으로 예측 불확실성을 범위로 제시, 최적화 알고리즘으로 생산 조건 탐색
- **LSTM 생산량 예측** (박사 연구, 2019–2020): 업계 표준(감소곡선) 대비 정확도 **최대 23%** 향상
- **물·가스 유입 현상의 수학 공식 유도** (석사 논문 · SPE 2018 제1저자, 2015–2018): 시뮬레이션 없이 계산하는 해석해, 여러 유정으로 확장
- **원유·물·가스 흐름 시뮬레이터** (수업 프로젝트, 2016): MATLAB으로 **처음부터 구현**(약 1,000줄), **표준 예제와 결과 일치**

### 🛠️ 기술
**AI · LLM**<br/>
<img src="https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white"/>
<img src="https://img.shields.io/badge/LangGraph-1C3C3C?style=flat-square&logo=langgraph&logoColor=white"/>
<img src="https://img.shields.io/badge/OpenAI-412991?style=flat-square&logo=openai&logoColor=white"/>
<img src="https://img.shields.io/badge/FAISS-0467DF?style=flat-square"/>
<img src="https://img.shields.io/badge/YOLO-111F68?style=flat-square"/>
<img src="https://img.shields.io/badge/Stable%20Diffusion-SDXL-7B3FE4?style=flat-square"/>

**평가 · 품질**<br/>
<img src="https://img.shields.io/badge/골든셋%20설계-1F4E8C?style=flat-square"/>
<img src="https://img.shields.io/badge/RAGAS-1F4E8C?style=flat-square"/>
<img src="https://img.shields.io/badge/pytest-0A9EDC?style=flat-square&logo=pytest&logoColor=white"/>
<img src="https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white"/>

**백엔드 · 인프라**<br/>
<img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white"/>
<img src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white"/>
<img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white"/>
<img src="https://img.shields.io/badge/AWS%20EC2-FF9900?style=flat-square&logo=amazonec2&logoColor=white"/>
<img src="https://img.shields.io/badge/GCP-4285F4?style=flat-square&logo=googlecloud&logoColor=white"/>

**ML · 수리 · 데이터**<br/>
<img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white"/>
<img src="https://img.shields.io/badge/TensorFlow-FF6F00?style=flat-square&logo=tensorflow&logoColor=white"/>
<img src="https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white"/>
<img src="https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white"/>
<img src="https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white"/>
<img src="https://img.shields.io/badge/MATLAB-0076A8?style=flat-square"/>
<br/>편미분방정식 해석해 · 몬테카를로 시뮬레이션 · 실험계획법 · 최적화 · LSTM 시계열 예측 · 수치해석·시뮬레이션

### 🎓 학력 · 교육
- **펜실베이니아 주립대학교 (미국)** · 에너지광물공학 박사과정 수료 (부전공: 통계학, 계산과학) · 2018–2024
- **펜실베이니아 주립대학교 (미국)** · 석유천연가스공학 석사 · 2015–2018
- **한양대학교** · 자원환경공학과 학사 · 학과 수석(33명 중 1위), 제2공과대학 차석 졸업 · 2009–2015
- **코드잇 스프린트** · AI 엔지니어 10기 수료 · 2026

### 🏅 수상
- 고용노동부장관상(장려상), 제8회 K-디지털 트레이닝 해커톤 · 2026
- EME 올해의 대학원 조교상, 펜실베이니아 주립대 (학생 학습에 대한 헌신과 기여) · 2017
- 국가 이공계 장학금, 4학기 전액 · 2013–2014

### 📜 자격증
- TOEIC 985 / 990 · 2026
- 데이터분석 준전문가(ADsP), 한국데이터산업진흥원 · 2026
- Engineer in Training(EIT), 미국 NCEES FE 시험 합격 · 2017
