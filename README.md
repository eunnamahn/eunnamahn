<h2 align="center">안녕하세요, AI 엔지니어 안은남입니다 👋</h2>
<p align="center">
  <b>AI 엔지니어 · LLM / RAG 시스템 · 평가·품질 · 수리 모델링 · 영어 능통</b><br/>
  평가 기준을 먼저 세우고, 그 기준으로 설계를 고릅니다.
</p>

<p align="center">
  <a href="https://eunnamahn.github.io"><img src="https://img.shields.io/badge/웹사이트-eunnamahn.github.io-1F4E8C?style=flat-square&logo=githubpages&logoColor=white"/></a>
  <a href="https://eunnamahn.github.io/en/"><img src="https://img.shields.io/badge/English-Website-1F4E8C?style=flat-square"/></a>
  <a href="mailto:baduk89@hanmail.net"><img src="https://img.shields.io/badge/Email-baduk89%40hanmail.net-555555?style=flat-square&logo=maildotru&logoColor=white"/></a>
  <img src="https://img.shields.io/badge/영어-능통%20(미국%20대학원%209년)-555555?style=flat-square"/>
</p>

---

### 🙋 소개
- **검증할 수 있는** LLM 서비스를 만듭니다. 결정은 결정론적 컴포넌트가 내리고, LLM은 결과를 설명만 하며, 모든 주장은 검증기를 거칩니다.
- 미국 **펜실베이니아 주립대**에서 9년간 석사·박사과정을 밟으며 편미분방정식 해석해, 몬테카를로 시뮬레이션, 통계 모델링으로 연구했습니다.
- 영어로 논문을 썼고, **8년간 영어로 학부 수업 조교**를 맡았습니다.
- 코드잇 스프린트 AI 엔지니어 과정에서 프로젝트 4개 중 3개를 팀장으로 이끌었습니다 · 🏆 고용노동부장관상(장려상, 2026)

### 📄 논문
- **재난 취약계층을 위한 근거 기반 대피 안내 서비스의 설계 및 구현.**
  한국정보처리학회 학술대회(ACK 2026) · *제1저자 · 구두발표(2026.11.06)*
- **Multi-Well Analytical Solution for Coning Under Simultaneous Steady-State Flow of Three Phases.**
  SPE Improved Oil Recovery Conference, 2018 · *제1저자 · 영문* · [doi.org/10.2118/190182-MS](https://doi.org/10.2118/190182-MS)

### 🎯 프로젝트
**2026**
| 프로젝트 | 내용 | 핵심 결과 | 기술 |
|---|---|---|---|
| [**SAVERS**](https://github.com/team-savers/savers-project) 🏆 | 재난 취약계층 맞춤 홍수 대피 안내 (앱 설치 불필요) · 팀장 | **로그에 없는 주장 0건**: 런타임 응답 30/30 일치, 적대 프롬프트 12/12 차단 · 대피 의향 **3.2 → 8.3** (52명, p<0.001) | FastAPI, LangChain, NetworkX, AWS EC2 |
| [**AI 광고 스튜디오**](https://github.com/codeit-part4-team2/ad-creative-studio) | 소상공인용 광고 이미지·문구 생성, 제품은 절대 바뀌지 않게 · 팀장 | 제품 보존 관문(마스크 CLIP ≥ 0.85) **4/4** 통과 · LCM-LoRA로 배경 생성 **17.47초 → 1.72초**(약 10배) · 테스트 486건 | SDXL, ControlNet, IP-Adapter, GCP |
| [**입찰메이트**](https://github.com/Eastar0102/codeit-part3-team1) | 공공 RFP 100건(HWP·PDF) RAG 질의응답, 출처 인용·답변 불가 시 거절 · 평가 담당 | 골든셋 95문항으로 708개 조합 비교 · 최종 **MRR 0.977**, 거절 정확도 1.0(19/19), 응답 3.6초, **API 비용 0원** | LangChain, LangGraph, FAISS, KURE-v1, EXAONE 3.5 |
| [**PillScope**](https://github.com/qja0707/OralMedicineImageDetection) | 경구약제 객체 탐지: 비슷한 56개 클래스, 이미지 186장, 51배 불균형 · 팀장 | Crop & Paste로 186 → 1,026장 · 검증 mAP@[.75:.95] **0.936** · WBF 앙상블로 비공개 Kaggle 대회 **0.851 → 0.9355** | YOLOv11, RT-DETRv2, RF-DETR |

**대학원 연구 (펜실베이니아 주립대)**
- 유전 모델을 실제 생산 데이터에 맞추는 확률적 보정: 몬테카를로·실험계획법으로 불확실성 정량화, Simulated Annealing 생산 최적화 (2021–2024)
- 과거 생산량으로 미래 생산량을 예측하는 LSTM 모델, 업계 표준(감소곡선) 대비 **정확도 최대 23% 향상** (2019–2020)
- 유정에 물·가스가 함께 빨려 드는 현상의 해석해: 라플라스 방정식·중첩 원리로 다중 유정의 정확한 해 도출 (석사 논문, 2015–2018)

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
<img src="https://img.shields.io/badge/TensorFlow-FF6F00?style=flat-square&logo=tensorflow&logoColor=white"/>
<img src="https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white"/>
<img src="https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white"/>
<img src="https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white"/>
<br/>편미분방정식 해석해 · 몬테카를로 시뮬레이션 · 실험계획법 · 최적화 · 시계열·통계 모델링

### 🎓 학력 · 교육
- **펜실베이니아 주립대학교 (미국)** — 에너지광물공학 박사과정 수료 (부전공: 통계학, 계산과학) · 2018–2024
- **펜실베이니아 주립대학교 (미국)** — 석유천연가스공학 석사 · 2015–2018
- **한양대학교** — 자원환경공학과 학사 · 학과 수석(33명 중 1위), 제2공과대학 차석 졸업 · 2009–2015
- **코드잇 스프린트** — AI 엔지니어 10기 수료 · 2026

### 🏅 수상 · 자격증
- 🏆 고용노동부장관상(장려상), 제8회 K-디지털 트레이닝 해커톤 · 2026
- 🏆 EME 올해의 대학원 조교상, 펜실베이니아 주립대 · 2017
- TOEIC 985/990 · 데이터분석 준전문가(ADsP) · Engineer in Training (EIT, 미국 NCEES FE 시험 합격)

<p align="center">
  <img height="150" src="https://github-readme-stats.vercel.app/api/top-langs/?username=eunnamahn&layout=compact&hide_border=true&title_color=1F4E8C"/>
</p>
