# 프롬프트 실험실

Streamlit과 Google Gemini API로 만든 프롬프트 실험용 챗봇입니다.

같은 질문이라도 챗봇 역할, 답변 길이, 출력 형식, temperature 값에 따라 AI 답변이 어떻게 달라지는지 비교해볼 수 있습니다.

## 실행 방법

1. 패키지를 설치합니다.

```bash
pip install -r requirements.txt
```

2. 프로젝트 루트에 `.env` 파일을 만들고 Gemini API 키를 입력합니다.

```env
GEMINI_API_KEY="your_gemini_api_key_here"
GEMINI_MODEL="gemini-3-flash-preview"
```

3. Streamlit 앱을 실행합니다.

```bash
streamlit run app.py
```

실행 후 터미널에 표시되는 주소로 접속하면 됩니다. 일반적으로 `http://localhost:8501`에서 열립니다.

## 주요 파일

- `app.py`: Streamlit 챗봇 앱
- `requirements.txt`: Python 실행에 필요한 패키지 목록
- `.env.example`: 환경 변수 예시 파일
- `.gitignore`: API 키, 캐시, 빌드 결과물 제외 설정

## 기능

- 챗봇 역할 선택
- 답변 길이 선택
- 출력 형식 선택
- temperature 조절
- 현재 적용된 시스템 프롬프트 확인
- 대화 기록 유지
- 대화 초기화
- 샘플 질문 선택
- AI 답변 피드백 기록
