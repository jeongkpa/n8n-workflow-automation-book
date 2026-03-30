# n8n으로 업무 자동화 진짜 잘함

> **📘 도서 실습용 n8n 워크플로 파일 모음**

「n8n으로 업무 자동화 진짜 잘함」 책에서 다루는 실습 워크플로 JSON 파일을 제공하는 공식 저장소입니다.  
각 챕터별로 정리되어 있으며, n8n에 직접 임포트하여 바로 실습할 수 있습니다.

## 📖 도서 정보

| 항목 | 내용 |
|------|------|
| **도서명** | n8n으로 업무 자동화 진짜 잘함 |
| **저자** | 박정기 |
| **출간일** | 2026년 4월 17일 |
| **페이지** | 136쪽 (내지 기준) |

## 📂 워크플로 목록

### CHAPTER 03 — n8n 기본 기능 익히기

| 파일명 | 워크플로명 | 설명 |
|--------|-----------|------|
| `fastcampus_EX1.json` | fastcampus EX1 | HTTP 요청, Google Sheets 연동, 다양한 트리거(Schedule, Webhook, Form, Chat) 기본 실습 |
| `fastcampus_EX1_IF.json` | fastcampus_EX1 IF | 위 워크플로에 **If 조건 분기** 노드를 추가한 버전 |
| `fastcampus_EX1_Switch.json` | fastcampus_EX1 Switch | 위 워크플로에 **Switch 다중 분기** 노드를 추가한 버전 |
| `fastcampus_EX_Expr.json` | fastcampus EX2 | n8n **표현식(Expression)** 실습 — 문자열 조작, 수학, 조건문, 날짜, n8n 고유 기능 등 |

### CHAPTER 08 — 프로젝트 1: 자동 리포트 생성

| 파일명 | 워크플로명 | 설명 |
|--------|-----------|------|
| `CHAPTER08.json` | PROJECT 1 | Schedule Trigger → Google Sheets 데이터 수집 → QuickChart 차트 생성 → Gmail 발송 |

### CHAPTER 09 — 프로젝트 2: 이메일 자동화

| 파일명 | 워크플로명 | 설명 |
|--------|-----------|------|
| `CHAPTER09.json` | PRJ 2 | Gmail Trigger → Zoom 메일 필터링 → HTML 콘텐츠 생성 → Slack 메시지 전송 + Gmail 발송 |

### CHAPTER 10 — 프로젝트 3: AI 뉴스 분석 봇

| 파일명 | 워크플로명 | 설명 |
|--------|-----------|------|
| `CHAPTER10.json` | 2025-08-04-PRJ3 | RSS 뉴스 피드(TSLA, NVDA, AAPL) 수집 → AI 모델(OpenAI, Groq, Perplexity) 분석 → Discord/Dropbox 배포. Form 트리거로 종목 선택 가능 |

### CHAPTER 11 — 프로젝트 4: AI 에이전트

| 파일명 | 워크플로명 | 설명 |
|--------|-----------|------|
| `CHAPTER11.json` | part5 google sheet Agent | AI Agent + Google Gemini/OpenAI → Google Sheets HR 데이터 조회 → Google Docs 문서 자동 생성. 채팅 인터페이스 기반 |

## 🚀 사용 방법

### 1. 워크플로 파일 다운로드

이 저장소를 클론하거나, 원하는 JSON 파일을 개별 다운로드합니다.

```bash
git clone https://github.com/<YOUR_USERNAME>/n8n으로-업무-자동화.git
```

### 2. n8n에 임포트

1. n8n 편집기를 엽니다.
2. 좌측 메뉴에서 **Workflows** 클릭
3. 우측 상단 **⋮** 메뉴 → **Import from File** 선택
4. 다운로드한 `.json` 파일을 선택하면 워크플로가 임포트됩니다.

### 3. 크리덴셜 설정

임포트한 워크플로에는 **크리덴셜(인증 정보)이 포함되어 있지 않습니다.**  
각 노드에서 사용하는 서비스(Google Sheets, Gmail, Slack, Discord 등)의 크리덴셜을 직접 생성하고 연결해 주세요.  
자세한 크리덴셜 설정 방법은 도서를 참고해 주세요.

## 🔧 사전 준비 사항

- **n8n** 설치 (클라우드 또는 셀프 호스팅)
- 각 프로젝트에서 사용하는 외부 서비스 계정:

| 챕터 | 필요한 서비스 |
|-------|-------------|
| CHAPTER 03 | Google Sheets |
| CHAPTER 08 | Google Sheets, Gmail |
| CHAPTER 09 | Gmail, Slack |
| CHAPTER 10 | OpenAI API, Groq API, Discord, Dropbox |
| CHAPTER 11 | OpenAI API 또는 Google Gemini API, Google Sheets, Google Docs |

## 📄 라이선스

이 저장소의 워크플로 파일은 「n8n으로 업무 자동화 진짜 잘함」 도서의 학습 목적으로 제공됩니다.  
자유롭게 학습 및 수정하여 사용할 수 있으나, 상업적 재배포는 금지합니다.

## 🙋 문의

도서 내용이나 워크플로 관련 문의사항은 [Issues](../../issues) 탭에 남겨주세요.
