# 메탄올–물 증류탑 발표자료 (Quarto revealjs)

- `메탄올-물_증류탑_발표.qmd` — 원본 (Quarto Markdown, 25장, 15분 발표 기준)
- `메탄올-물_증류탑_발표.html` — 렌더 결과 (단일 파일, 오프라인 열람 가능). 브라우저에서 `F` 전체화면, `S` 발표자 노트, `E` 인쇄용 보기
- `custom.scss` — 테마
- `figures/` — 팀 GitHub 그림 + `scripts/make_figures.py`로 만든 그림
- `data/` — DWSIM UNIFAC 평형점 224개(`unifac_vle_101p3kPa.csv`), xlsx 덤프(`xlsx_dump.json`, 2026-11-17부터 `물-메탄올 증류_data_수정.xlsx` 기준), 검증 결과(`verification.json`)
- `수정권고사항.txt` — 계산 검토 의견과 반영 현황

## 다시 만들기

```bash
cd 발표자료
python scripts/make_figures.py          # 그림 + Ex 21.2 / DWSIM 작도 재현 검증
quarto render 메탄올-물_증류탑_발표.qmd
```

PDF가 필요하면 HTML을 Chrome에서 `?print-pdf`를 붙여 열고 인쇄 → PDF로 저장.

