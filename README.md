# 11번가 GNB·탭바 아이디에이션 프로토타입 — B안

**보기:** https://remnantran.github.io/11st-gnb-tabbar-prototypeB/

홈을 스크롤하면 분홍 헤더(로고·검색·타이틀배너)가 올라가고 카테고리 탭이 상단에 고정되며,
탭 아래로 `floating_text` 띠배너가 내려와요. 띠배너 문구는 왼쪽으로 계속 흐르고 배경 그라데이션도 천천히 움직여요.

- **AI검색:** 탭바 왼쪽 'AI 맞춤검색' 알약을 누르면 알약이 제자리에서 늘어나 AI검색 바텀시트가 돼요. 바깥 탭·손잡이 끌어내리기·`Esc`로 닫으면 다시 알약으로 오므라들어요.
- **나의11번가:** 탭바의 나의11번가를 누르면 홈 GNB 알약이 제자리에서 나의11번가 GNB로 바뀌고, 화면이 아래에서 떠오르며 덮어요. 탭바는 '11번가+ 구매미션' 알약 + 흰 알약(뒤로·홈·카테고리·11톡·최근본)으로 바뀌어요.

키보드: `H` 핫스팟 보기 · `←`/`Esc` 뒤로.

Figma: [K03Ye6qjq9vaqKREhSuN9o](https://www.figma.com/design/K03Ye6qjq9vaqKREhSuN9o/) — 홈 32:3309, 스크롤 후 홈 86:64817 (floating_text 88:66423), AI검색 펼침 111:92774, 나의11번가 111:95109

## 파일

| 파일 | 설명 |
|---|---|
| `index.html` | 원본. 수정은 여기서만. GitHub Pages도 이 파일을 보여줌 |
| `img/` | Figma 2x 내보내기. `_orig/`는 자르기 전 원본 |
| `build.py` | 아래 두 파일 생성 |
| `11st-gnb-tabbar-prototypeB.html` | 이미지 내장 단일 파일 — 메일·메신저로 보내 더블클릭으로 열기 |
| `share.html` | claude.ai Artifact 재배포용 |

## 수정 후 반영

```bash
python3 -m http.server 8766   # 로컬 확인: http://localhost:8766
python3 build.py
git add -A && git commit -m "..." && git push   # 1~2분 뒤 Pages 반영
```
