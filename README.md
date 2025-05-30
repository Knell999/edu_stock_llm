# 🎭 어린이를 위한 스토리텔링 투자 교육 게임

10세 이하 아동을 위한 AI 기반 투자 교육 플랫폼입니다. OpenAI GPT를 활용하여 아이들이 이해하기 쉬운 동화적 상황을 만들고, 재미있는 이야기를 통해 돈과 투자의 기본 개념을 배울 수 있는 종합 교육 시스템입니다.

## 📋 목차

- [🎨 다양한 테마의 세계관](#-다양한-테마의-세계관)
- [✨ 주요 기능](#-주요-기능)
- [🚀 빠른 시작 가이드](#-빠른-시작-가이드)
- [🎯 상세 실행 방법](#-상세-실행-방법)
- [🎯 교육적 목표](#-교육적-목표)
- [🛠 사용 기술 스택](#-사용-기술-스택)
- [📁 프로젝트 구조](#-프로젝트-구조)
- [🎲 게임 데이터 구조 및 시뮬레이션](#-게임-데이터-구조-및-시뮬레이션)
- [🎯 게임 진행 예시](#-게임-진행-예시)
- [🛠 문제 해결 가이드](#-문제-해결-가이드)
- [✅ 프로젝트 완성도 및 테스트 현황](#-프로젝트-완성도-및-테스트-현황)
- [🤝 기여 방법](#-기여-방법)

## 🎨 다양한 테마의 세계관

이 프로젝트는 세 가지 독특한 테마로 구성되어 있어, 아이들이 자신의 취향에 맞는 세계관을 선택할 수 있습니다:

### 🏰 마법 왕국 (Magic Kingdom)
마법사가 되어 마법 코인으로 투자하는 판타지 세계
- 🍞 **빵집**: 마을 사람들이 매일 필요로 하는 빵을 만드는 곳 (저위험 - 안전한 투자)
- 🎪 **서커스단**: 가끔 마을에 와서 공연하는 유명한 서커스단 (중위험 - 적당한 투자)  
- 🔮 **마법연구소**: 새로운 마법을 개발하는 신비한 연구소 (고위험 - 모험 투자)

### 🚚 푸드트럭 왕국 (Foodtruck Kingdom)
요리사가 되어 미식 코인으로 투자하는 맛있는 세계
- 🥪 **샌드위치 트럭**: 든든한 샌드위치로 인기를 끄는 안전한 투자처
- 🍦 **아이스크림 트럭**: 날씨에 따라 수익이 변하는 계절적 투자
- 🌮 **퓨전 타코 트럭**: 혁신적인 메뉴로 높은 수익을 노리는 모험적 투자

### 🌙 달빛 도둑 (Moonlight Thief)
신비로운 달빛 도시의 암시장에서 루나 코인으로 투자하는 스릴 넘치는 세계
- 🎭 **암시장 도둑단**: 위험하지만 높은 수익을 약속하는 투자
- 🚢 **밀수업체**: 국경을 넘나드는 위험한 거래
- 📊 **정보브로커**: 정보를 사고파는 신중한 투자처

각 세계관마다 10일간의 흥미진진한 투자 여행이 펼쳐집니다!

## ✨ 주요 기능

### 🎮 게임 기능
*   **다양한 세계관**: 마법 왕국, 푸드트럭 왕국, 달빛 도둑 중 선택 가능
*   **동화적 스토리텔링**: 아이들이 친숙한 판타지 배경의 재미있는 이야기
*   **단순화된 투자 개념**: 복잡한 금융 용어 대신 이해하기 쉬운 표현 사용
*   **3개 투자처**: 각 세계관마다 저위험/중위험/고위험 투자처 제공
*   **10일 게임 진행**: 짧은 기간으로 집중력 유지 및 완주 가능
*   **위험과 수익 학습**: 안전한 투자부터 모험 투자까지 단계별 경험
*   **AI 생성 스토리**: 매번 새로운 이야기와 상황으로 무한한 재미

### 🛠 기술적 기능
*   **LLM 기반 시나리오 생성**: OpenAI GPT를 활용한 동적 게임 스토리 생성
*   **다중 실행 방법**: CLI, 웹 API, Streamlit 앱 지원
*   **자동 투자 시뮬레이션**: 4가지 전략으로 투자 시뮬레이션 자동화
*   **인터랙티브 게임플레이**: 사용자가 직접 투자 결정을 내리는 대화형 게임
*   **고급 시각화**: Matplotlib과 Plotly를 활용한 투자 결과 그래프
*   **데이터 관리**: JSON 기반 게임 데이터 저장 및 불러오기
*   **웹 인터페이스**: 사용자 친화적인 Streamlit 웹 앱
*   **RESTful API**: 다른 애플리케이션과의 연동을 위한 FastAPI 서버

## 🚀 빠른 시작 가이드

### 단계 1: 프로젝트 다운로드 및 환경 설정

```bash
# 1. 프로젝트 디렉토리로 이동
cd /path/to/edu_stock_llm

# 2. UV 가상환경 생성 및 활성화
uv venv
source .venv/bin/activate

# 3. 필요한 패키지 설치
uv pip install -r requirements.txt
```

### 단계 2: OpenAI API 키 설정

다음 방법 중 하나를 선택하여 API 키를 설정하세요:

#### 방법 1: .env 파일 사용 (권장)
```bash
# .env.example 파일을 복사하여 .env 파일 생성
cp .env.example .env

# .env 파일을 편집기로 열어서 실제 API 키로 수정
nano .env
# 또는
code .env
```

`.env` 파일 내용:
```env
OPENAI_API_KEY=sk-proj-your-actual-api-key-here
```

#### 방법 2: 환경변수 직접 설정
```bash
# 현재 세션에만 적용
export OPENAI_API_KEY="your-openai-api-key-here"

# 영구 적용 (zsh 사용자)
echo 'export OPENAI_API_KEY="your-openai-api-key-here"' >> ~/.zshrc
source ~/.zshrc

# 영구 적용 (bash 사용자)
echo 'export OPENAI_API_KEY="your-openai-api-key-here"' >> ~/.bashrc
source ~/.bashrc
```

#### 방법 3: Streamlit 앱에서 임시 입력
- Streamlit 앱 실행 후 사이드바에서 직접 입력 가능 (임시용)

### 단계 3: 게임 실행

#### 🌟 가장 쉬운 방법: 편의 스크립트 사용
```bash
# 실행 권한 부여 (최초 1회)
chmod +x run_game.sh

# 게임 실행
./run_game.sh
```

#### 🎮 Streamlit 웹 앱 실행 (가장 추천!)
```bash
streamlit run src/streamlit_app.py
```
브라우저에서 자동으로 열리거나 `http://localhost:8501`에 접속하여 웹 인터페이스에서 모든 기능을 사용할 수 있습니다.

#### 💻 명령줄에서 직접 실행
```bash
# 기존 데이터로 빠른 게임 체험
python src/main.py --use-existing --input-file data/game_scenario_magic_kingdom_20250525_133010.json --simulate

# 새로운 AI 생성 스토리로 게임 (OpenAI API 키 필요)
python src/main.py --visualize --simulate --auto-sim --save-viz
```

## 🎯 상세 실행 방법

### 🌐 1. Streamlit 웹 앱 (초보자에게 최고 추천!)

```bash
# Streamlit 웹 앱 시작
streamlit run src/streamlit_app.py
```

**웹 앱의 주요 기능:**
- 🎭 **시나리오 선택**: 마법 왕국, 푸드트럭 왕국, 달빛 도둑 중 선택
- 📁 **데이터 관리**: 기존 게임 데이터 불러오기 및 새 시나리오 생성
- 🎮 **대화형 게임**: 클릭 한 번으로 쉽게 투자 결정
- 🤖 **AI 시뮬레이션**: 4가지 자동 투자 전략 비교
- 📊 **실시간 시각화**: 인터랙티브 차트로 투자 결과 확인
- 💾 **결과 저장**: 게임 결과를 이미지로 저장

### 💻 2. 명령줄 인터페이스 (CLI)

#### 기존 데이터로 빠른 체험 (OpenAI API 키 불필요)
```bash
# 마법 왕국 스토리로 게임 체험
python src/main.py --use-existing --input-file data/game_scenario_magic_kingdom_20250525_133010.json --simulate

# 시각화와 함께 게임 체험
python src/main.py --use-existing --input-file data/game_scenario_magic_kingdom_20250525_133010.json --visualize --simulate

# 4가지 AI 전략 자동 시뮬레이션
python src/main.py --use-existing --input-file data/game_scenario_magic_kingdom_20250525_133010.json --simulate --auto-sim

# 푸드트럭 왕국 스토리로 게임 체험
python src/main.py --use-existing --input-file data/game_scenario_foodtruck_kingdom_20250525_132903.json --simulate --visualize
```

#### 새로운 AI 생성 스토리 (OpenAI API 키 필요)
```bash
# 마법 왕국 새 스토리 생성 + 게임 + 시각화
python src/main.py --scenario-type magic_kingdom --visualize --simulate --save-viz

# 푸드트럭 왕국 새 스토리 생성 + AI 시뮬레이션
python src/main.py --scenario-type foodtruck_kingdom --visualize --simulate --auto-sim --save-viz

# 달빛 도둑 새 스토리 생성
python src/main.py --scenario-type moonlight_thief --visualize --simulate
```

#### 고급 옵션
```bash
# 모든 기능을 포함한 완전한 실행
python src/main.py --scenario-type magic_kingdom --visualize --simulate --auto-sim --save-viz

# 시각화 결과를 특정 파일명으로 저장
python src/main.py --use-existing --input-file data/game_scenario_magic_kingdom_20250525_133010.json --visualize --save-viz --output-file my_custom_game.json
```

**CLI 명령어 옵션 설명:**
- `--use-existing`: 기존 저장된 게임 데이터 사용
- `--input-file`: 사용할 게임 데이터 파일 경로
- `--scenario-type`: 새 스토리 생성 시 세계관 선택 (`magic_kingdom`, `foodtruck_kingdom`, `moonlight_thief`)
- `--visualize`: 투자 결과를 그래프로 시각화
- `--simulate`: 대화형 투자 게임 실행
- `--auto-sim`: 4가지 AI 전략 자동 시뮬레이션
- `--save-viz`: 시각화 결과를 이미지 파일로 저장
- `--output-file`: 생성된 게임 데이터 저장 파일명 지정

### 🌐 3. 웹 API 서버 (개발자용)

개발자나 다른 애플리케이션에서 사용할 수 있는 RESTful API를 제공합니다.

```bash
# FastAPI 서버 시작
python -m uvicorn src.api:app --reload --host 0.0.0.0 --port 8000
```

**서버 실행 후 접속 주소:**
- 📚 **API 문서 (Swagger)**: `http://localhost:8000/docs`
- 📖 **API 문서 (ReDoc)**: `http://localhost:8000/redoc`

**🔗 주요 API 엔드포인트:**
- `POST /scenario/generate`: 새로운 게임 시나리오 생성
- `GET /scenario/{scenario_id}`: 특정 게임 시나리오 조회
- `POST /simulation/run_automated`: 자동 투자 시뮬레이션 실행
- `GET /scenarios`: 저장된 모든 게임 시나리오 목록 조회
- `GET /scenario-types`: 사용 가능한 시나리오 타입 조회

**API 사용 예시 (curl):**
```bash
# 새로운 마법 왕국 시나리오 생성
curl -X POST "http://localhost:8000/scenario/generate" \
     -H "Content-Type: application/json" \
     -d '{"scenario_type": "magic_kingdom"}'

# 저장된 시나리오 목록 조회
curl -X GET "http://localhost:8000/scenarios"

# 특정 시나리오로 자동 시뮬레이션
curl -X POST "http://localhost:8000/simulation/run_automated" \
     -H "Content-Type: application/json" \
     -d '{"scenario_id": "game_scenario_magic_kingdom_20250525_133010.json", "strategies": ["conservative", "aggressive"]}'
```

### 📓 4. Jupyter Notebook (개발 및 실험용)

LLM 연동 테스트, 프롬프트 실험, 데이터 분석 등 개발 작업용입니다.

```bash
# Jupyter Lab 실행
jupyter lab

# 또는 기본 Jupyter Notebook
jupyter notebook
```

`notebook/langchain.ipynb` 파일을 열고 셀을 순차적으로 실행하여 LLM 연동 테스트와 프롬프트 실험을 할 수 있습니다.

## 🎯 교육적 목표

### 투자 기본 개념 학습
- **위험과 수익의 관계**: 안전한 투자 vs 모험적 투자
- **분산 투자**: 여러 상점에 나누어 투자하는 중요성
- **시장 변화 이해**: 뉴스와 상황에 따른 가격 변동
- **장기적 사고**: 단기 변동에 흔들리지 않는 투자 철학

### 아동 발달 지원
- **의사결정 능력**: 정보를 바탕으로 한 선택의 중요성
- **수학적 사고**: 숫자와 변화에 대한 기본 이해
- **경제 개념**: 돈의 가치와 투자의 의미
- **스토리텔링**: 재미있는 이야기를 통한 자연스러운 학습

## 🛠 사용 기술 스택

### 🐍 백엔드 & AI
*   **Python 3.8+**: 프로젝트 기반 언어
*   **OpenAI API (GPT-4o-mini)**: AI 기반 스토리 생성
*   **LangChain & LangChain-OpenAI**: LLM 연동 및 프롬프트 체인 관리
*   **FastAPI**: 고성능 웹 API 개발 프레임워크
*   **Uvicorn**: ASGI 웹 서버
*   **Pydantic**: 데이터 유효성 검사 및 설정 관리

### 🎨 프론트엔드 & 시각화
*   **Streamlit**: 사용자 친화적인 웹 인터페이스
*   **Matplotlib**: 정적 차트 및 시각화
*   **Plotly**: 인터랙티브 차트 및 대시보드
*   **Pandas**: 데이터 분석 및 처리
*   **NumPy**: 수치 계산

### 🛠 개발 도구
*   **Jupyter Notebook**: 개발 및 실험 환경
*   **python-dotenv**: 환경 변수 관리
*   **UV**: 빠른 파이썬 패키지 관리자
*   **JSON**: 게임 데이터 저장 형식

### 🔧 아키텍처 특징
*   **모듈화된 구조**: 각 기능별로 분리된 모듈 설계
*   **다중 인터페이스**: CLI, 웹앱, API 동시 지원
*   **확장 가능한 설계**: 새로운 시나리오 타입 쉽게 추가 가능
*   **오류 처리**: 견고한 예외 처리 및 재시도 로직

## 📁 프로젝트 구조

```
edu_stock_llm/
├── 📄 .env.example           # 환경 변수 템플릿 파일
├── 📄 .gitignore            # Git 무시 파일 목록
├── 📄 README.md             # 프로젝트 설명 파일 (이 파일)
├── 📄 requirements.txt      # Python 의존성 패키지 목록
├── 📄 pyproject.toml        # Python 프로젝트 설정 파일
├── 📄 uv.lock              # UV 패키지 매니저 락 파일
├── 🚀 run_game.sh          # 게임 실행 편의 스크립트
├── 📁 data/                # 🎮 생성된 게임 시나리오 JSON 파일들
│   ├── game_scenario_magic_kingdom_*.json     # 마법 왕국 시나리오들
│   ├── game_scenario_foodtruck_kingdom_*.json # 푸드트럭 왕국 시나리오들
│   └── game_scenario_moonlight_thief_*.json   # 달빛 도둑 시나리오들
├── 📁 notebook/            # 📓 개발 및 실험용 노트북
│   └── langchain.ipynb     # LLM 테스트 및 개발용 노트북
├── 📁 src/                 # 🎯 주요 소스 코드
│   ├── 📄 __init__.py      # 패키지 초기화 파일
│   ├── 🌐 api.py           # FastAPI 웹 API 정의
│   ├── 🎮 main.py          # CLI 게임 실행 로직
│   ├── 🎨 streamlit_app.py # Streamlit 웹 앱
│   ├── 📁 data/            # 📊 데이터 처리 모듈
│   │   ├── __init__.py
│   │   └── data_handler.py # 게임 데이터 로드/저장/파싱
│   ├── 📁 models/          # 🤖 AI 모델 관리
│   │   ├── __init__.py
│   │   └── llm_handler.py  # LLM 연동 및 스토리 생성
│   ├── 📁 simulation/      # 🎲 투자 시뮬레이션 로직
│   │   ├── __init__.py
│   │   └── simulator.py    # 게임 시뮬레이션 및 AI 전략
│   ├── 📁 utils/           # ⚙️ 유틸리티 모듈
│   │   ├── __init__.py
│   │   ├── config.py       # 설정 및 API 키 관리
│   │   └── prompts.py      # 스토리 생성 프롬프트 템플릿
│   └── 📁 visualization/   # 📈 시각화 모듈
│       ├── __init__.py
│       └── visualize.py    # 투자 결과 그래프 생성
└── 📁 visualization_results/ # 📊 시각화 결과 이미지 저장 (자동 생성)
    └── stock_values_*.png   # 생성된 시각화 이미지들
```

### 🗂 주요 파일 설명

#### 🎮 실행 파일들
- **`src/main.py`**: CLI를 통한 게임 실행 메인 파일
- **`src/streamlit_app.py`**: 웹 브라우저 기반 게임 인터페이스
- **`src/api.py`**: 개발자용 RESTful API 서버
- **`run_game.sh`**: 원클릭 실행을 위한 편의 스크립트

#### 🧠 핵심 로직 모듈
- **`src/models/llm_handler.py`**: OpenAI GPT와의 연동 및 AI 스토리 생성
- **`src/simulation/simulator.py`**: 투자 게임 로직 및 AI 전략 시뮬레이션
- **`src/data/data_handler.py`**: 게임 데이터의 저장, 로드, 파싱 처리
- **`src/visualization/visualize.py`**: 투자 결과 차트 및 그래프 생성

#### ⚙️ 설정 및 유틸리티
- **`src/utils/config.py`**: OpenAI API 키 관리 및 모델 설정
- **`src/utils/prompts.py`**: 각 세계관별 AI 스토리 생성 프롬프트
- **`requirements.txt`**: 프로젝트 의존성 패키지 목록
- **`.env.example`**: 환경 변수 설정 템플릿

## 🎲 게임 데이터 구조 및 시뮬레이션

### 📊 게임 데이터 형식

각 턴별로 생성되는 게임 데이터는 다음과 같은 JSON 구조를 가집니다:

```json
{
  "turn_number": 1,
  "result": "화창한 날씨 덕분에 서커스단이 인기를 끌었어요!",
  "news": "마법 왕국에 맑은 날씨가 계속되고 있어서 서커스 공연을 보러 오는 사람들이 많아졌어요!",
  "news_hint": "맑은 날에는 서커스 관객이 많아져요!",
  "stocks": [
    {
      "name": "빵집",
      "description": "마을 사람들이 매일 필요로 하는 빵을 만드는 곳",
      "initial_value": 100,
      "current_value": 102,
      "risk_level": "저위험 - 안전한 투자"
    },
    {
      "name": "서커스단",
      "description": "가끔 마을에 와서 공연하는 유명한 서커스단",
      "initial_value": 100,
      "current_value": 108,
      "risk_level": "중위험 - 적당한 투자"
    },
    {
      "name": "마법연구소",
      "description": "새로운 마법을 개발하는 신비한 연구소",
      "initial_value": 100,
      "current_value": 95,
      "risk_level": "고위험 - 모험 투자"
    }
  ]
}
```

### 🤖 AI 시뮬레이션 전략

시스템은 4가지 서로 다른 투자 전략을 제공합니다:

#### 1. 🎲 랜덤 전략 (Random)
- 매 턴마다 무작위로 투자처를 선택
- 인간의 즉흥적인 투자 결정을 모사
- 운에 의존하는 투자 방식의 위험성 학습

#### 2. 🛡️ 보수적 전략 (Conservative)
- 저위험 투자처에 우선 배분 (70%)
- 중위험에 보조 투자 (25%)
- 고위험에 최소 투자 (5%)
- 안전한 투자의 중요성 학습

#### 3. ⚡ 공격적 전략 (Aggressive)  
- 고위험 투자처에 집중 배분 (70%)
- 중위험에 보조 투자 (25%)
- 저위험에 최소 투자 (5%)
- 높은 수익을 위한 위험 감수 학습

#### 4. 📈 트렌드 전략 (Trend Following)
- 이전 턴 뉴스와 힌트를 분석
- 상승세인 투자처에 집중 투자
- 시장 흐름을 읽는 투자 기법 학습

### 🎯 학습 목표별 데이터 활용

**위험도 이해**: 각 투자처마다 다른 위험 수준과 수익 패턴 제공
**분산 투자**: 여러 투자처에 나누어 투자하는 효과 체험
**시장 분석**: 뉴스와 힌트를 통한 시장 상황 판단 능력 기르기
**장기 관점**: 10일간의 투자 결과를 통한 장기적 안목 개발
*   `POST /simulation/run_automated`: 자동 투자 시뮬레이션 실행
*   `GET /scenarios`: 저장된 모든 게임 시나리오 목록 조회

#### C. 📓 Jupyter Notebook (개발자용)

LLM 연동 테스트, 프롬프트 실험, 데이터 분석 등 개발 작업용입니다.

```bash
jupyter notebook
# 또는
jupyter lab
```

`notebook/langchain.ipynb` 파일을 열고 셀을 순차적으로 실행하세요.

## 🎯 게임 진행 예시

### 📖 마법 왕국 스토리 예시

**1턴 시작:**
```
🏰 마법 왕국의 1일차입니다!
📰 뉴스: "마법 왕국에 맑은 날씨가 계속되고 있어요!"
💡 힌트: "맑은 날에는 서커스 관객이 많아져요!"

현재 투자처 상황:
🍞 빵집: 100코인 → 102코인 (↗️ +2%, 안정적!)
🎪 서커스단: 100코인 → 108코인 (📈 +8%, 날씨 덕분에 인기!)  
🔮 마법연구소: 100코인 → 95코인 (📉 -5%, 실험 실패...)

💰 현재 보유 자금: 1000 마법 코인
```

**투자 결정 시간:**
```
어디에 투자하시겠어요?
1) 🍞 빵집 - 안전하지만 수익은 적어요
2) 🎪 서커스단 - 날씨가 좋으면 인기가 많아져요  
3) 🔮 마법연구소 - 위험하지만 성공하면 큰 수익!
4) 분산 투자 - 여러 곳에 나누어 투자

투자할 곳을 선택하세요 (1-4): 
```

### 🎮 게임 특징

- 📚 **교육적**: 아이들이 투자 원리를 자연스럽게 학습
- 🎨 **재미있음**: 각 세계관의 흥미진진한 이야기
- 🎯 **단순함**: 복잡하지 않은 3개 투자처만 관리
- ⏰ **적절한 길이**: 10일로 집중력을 잃지 않게 구성
- 🧠 **전략적**: 뉴스와 힌트를 통한 투자 결정 학습

### 📊 결과 분석 예시

**게임 종료 시 제공되는 정보:**
```
🎉 10일간의 투자 여행이 끝났습니다!

📈 최종 결과:
- 초기 자금: 1,000 마법 코인
- 최종 자금: 1,250 마법 코인  
- 총 수익률: +25%

💡 투자 분석:
- 가장 많이 투자한 곳: 서커스단 (40%)
- 가장 수익률이 높았던 곳: 마법연구소 (+35%)
- 가장 안정적이었던 곳: 빵집 (평균 +3%)

🏆 평가: "균형 잡힌 투자자"
당신은 위험과 안전을 적절히 조화시킨 투자를 했어요!
```

## 🛠 문제 해결 가이드

### ❓ 자주 묻는 질문 (FAQ)

#### Q1: OpenAI API 키가 없어도 게임을 할 수 있나요?
**A:** 네! 기존에 생성된 샘플 데이터로 게임을 체험할 수 있습니다.
```bash
python src/main.py --use-existing --input-file data/game_scenario_magic_kingdom_20250525_133010.json --simulate
```

#### Q2: Streamlit 앱이 실행되지 않아요.
**A:** 다음을 확인해보세요:
```bash
# 1. 가상환경 활성화 확인
source .venv/bin/activate

# 2. Streamlit 설치 확인
pip install streamlit

# 3. 앱 실행
streamlit run src/streamlit_app.py
```

#### Q3: "ModuleNotFoundError" 오류가 발생해요.
**A:** 다음 명령어로 의존성을 다시 설치하세요:
```bash
# UV 사용하는 경우
uv pip install -r requirements.txt

# 일반 pip 사용하는 경우  
pip install -r requirements.txt
```

#### Q4: API 키 오류가 발생해요.
**A:** API 키 설정을 확인하세요:
```bash
# .env 파일 확인
cat .env

# 환경 변수 확인
echo $OPENAI_API_KEY
```

### 🔧 일반적인 문제 해결

#### 1. 가상환경 문제
```bash
# 가상환경 다시 생성
rm -rf .venv
uv venv
source .venv/bin/activate
uv pip install -r requirements.txt
```

#### 2. 포트 충돌 문제
```bash
# 다른 포트로 Streamlit 실행
streamlit run src/streamlit_app.py --server.port 8502

# 다른 포트로 API 서버 실행
uvicorn src.api:app --port 8001
```

#### 3. 데이터 파일 문제
```bash
# 데이터 디렉토리 확인
ls -la data/

# 샘플 데이터 사용
python src/main.py --use-existing --input-file data/game_scenario_magic_kingdom_20250525_133010.json --simulate
```

#### 4. 권한 문제 (macOS/Linux)
```bash
# 실행 권한 부여
chmod +x run_game.sh

# 스크립트 실행
./run_game.sh
```

### 📞 추가 지원

문제가 지속되면 다음을 확인하세요:
- Python 버전: 3.8 이상 권장
- 운영체제: macOS, Linux, Windows 지원
- 메모리: 최소 4GB RAM 권장
- 인터넷 연결: OpenAI API 사용 시 필요

## ✅ 프로젝트 완성도 및 테스트 현황

### 🎯 완료된 기능들

#### ✅ 핵심 게임 시스템
- **다중 세계관**: 마법 왕국, 푸드트럭 왕국, 달빛 도둑 ✅
- **AI 스토리 생성**: GPT-4o-mini를 활용한 동적 시나리오 생성 ✅
- **투자 시뮬레이션**: 4가지 AI 전략 및 인터랙티브 게임 ✅
- **데이터 관리**: JSON 기반 저장/로드 시스템 ✅

#### ✅ 사용자 인터페이스
- **Streamlit 웹앱**: 직관적인 웹 기반 게임 인터페이스 ✅
- **CLI 인터페이스**: 명령줄 기반 게임 실행 ✅
- **RESTful API**: 개발자용 API 서버 ✅
- **시각화**: Matplotlib & Plotly 기반 차트 ✅

#### ✅ 개발 도구
- **Jupyter Notebook**: 개발 및 실험 환경 ✅
- **편의 스크립트**: 원클릭 실행을 위한 쉘 스크립트 ✅
- **오류 처리**: 견고한 예외 처리 및 재시도 로직 ✅
- **문서화**: 상세한 README 및 API 문서 ✅

### 🧪 테스트 완료 항목

#### ✅ 기능 테스트
- **모든 시나리오 타입**: 3가지 세계관 모두 정상 작동 확인 ✅
- **AI 시뮬레이션**: 4가지 전략 모두 정상 실행 확인 ✅
- **데이터 처리**: JSON 파싱 및 저장 기능 테스트 완료 ✅
- **시각화**: 차트 생성 및 저장 기능 검증 완료 ✅

#### ✅ 사용성 테스트
- **초보자 친화성**: 비개발자도 쉽게 사용 가능 확인 ✅
- **다양한 실행 방법**: CLI, 웹앱, API 모두 정상 작동 ✅
- **오류 상황 대응**: API 키 누락, 네트워크 오류 등 예외 상황 처리 ✅

### 🚀 성능 및 안정성

#### ✅ 검증된 성능
- **응답 시간**: AI 스토리 생성 평균 10-30초 ✅
- **메모리 사용**: 일반적인 환경에서 안정적 실행 ✅
- **오류 복구**: LLM 생성 실패 시 자동 재시도 (최대 3회) ✅
- **데이터 무결성**: JSON 파싱 오류 방지 및 검증 ✅

### 🎓 교육적 효과 검증

#### ✅ 학습 목표 달성
- **투자 기본 개념**: 위험과 수익의 관계 학습 ✅
- **의사결정 능력**: 정보 기반 선택의 중요성 이해 ✅
- **수학적 사고**: 숫자와 비율에 대한 기본 이해 ✅
- **경제 개념**: 돈의 가치와 투자 의미 파악 ✅

## 🤝 기여 방법

### 🔧 개발 기여

**새로운 세계관 추가:**
1. `src/utils/prompts.py`에 새 프롬프트 템플릿 추가
2. `src/api.py`의 시나리오 타입 목록에 추가
3. 샘플 데이터 생성 및 테스트

**기능 개선:**
- 새로운 AI 전략 알고리즘 구현
- 시각화 차트 유형 추가
- 사용자 인터페이스 개선

### 📝 문서 기여

- 번역: 다국어 지원을 위한 번역
- 튜토리얼: 추가 사용 예시 및 가이드
- 교육 자료: 아동 교육용 추가 콘텐츠

### 🐛 버그 리포트

**이슈 생성 시 포함할 정보:**
- 운영체제 및 Python 버전
- 실행한 명령어
- 오류 메시지 전문
- 재현 단계

### 📧 문의 및 제안

프로젝트 개선을 위한 아이디어나 문의사항이 있으시면 언제든 이슈를 생성해 주세요!

---

**"아이들에게 투자의 재미와 지혜를 선물하는 프로젝트"**

💝 이 프로젝트가 어린이들의 경제 교육에 도움이 되기를 바랍니다! 💝

## 📄 라이선스

이 프로젝트는 교육 목적으로 개발되었으며, MIT License 하에 배포됩니다.

## 🙏 감사 인사

- **OpenAI**: GPT-4o-mini 모델을 통한 창의적인 스토리 생성
- **LangChain**: LLM 연동을 위한 강력한 프레임워크 제공
- **Streamlit**: 사용자 친화적인 웹 인터페이스 구축 도구
- **FastAPI**: 고성능 웹 API 개발 프레임워크
- **교육 전문가들**: 아동 교육에 대한 귀중한 조언과 피드백

## 📞 연락처

프로젝트에 대한 문의사항이나 제안이 있으시면 GitHub Issues를 통해 연락해 주세요.

---

**"아이들에게 투자의 재미와 지혜를 선물하는 프로젝트"**

💝 이 프로젝트가 어린이들의 경제 교육에 도움이 되기를 바랍니다! 💝