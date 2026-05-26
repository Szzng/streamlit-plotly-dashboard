# Streamlit Plotly Dashboard — Gapminder

Hans Rosling의 TED 강연으로 유명한 Gapminder 데이터(1952~2007, 142개국)를 **Streamlit + Plotly**로 시각화하는 인터랙티브 대시보드.

## 화면 구성 (4개 탭)

- 🫧 **애니메이션 버블** — 연도별 GDP × 기대수명 변화
- 🗺️ **세계 지도** — 지표별 국가 색칠 (GDP / 기대수명 / 인구)
- 📈 **국가 트렌드** — 선택 국가들의 시간 흐름
- 🏆 **대륙 비교** — 슬라이더로 연도 선택 + 대륙별 비교

## 로컬 실행

```bash
pip install -r requirements.txt
streamlit run plotly_dashboard.py
```

브라우저가 자동으로 `http://localhost:8501` 열림.

## Streamlit Community Cloud 배포

1. [share.streamlit.io](https://share.streamlit.io) 접속 → GitHub 로그인
2. **Create app** → 이 레포 선택
3. Main file path: `plotly_dashboard.py`
4. **Deploy!**

## 파일 구조

```
.
├── plotly_dashboard.py   # 메인 앱 코드
├── gapminder.csv         # 데이터 (Hans Rosling Foundation)
├── requirements.txt      # 의존성 (streamlit / pandas / plotly)
└── .gitignore
```
