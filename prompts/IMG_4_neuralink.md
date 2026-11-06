# 4번 「뉴럴링크는 왜 돼지와 원숭이 뇌에 칩을 심었나」 이미지 제작 명세서

| 항목 | 내용 |
|---|---|
| 페이지 | 4_neuralink_animal_brain_ai.html |
| 모드 / 주 앵커 | 교과서 모드 / A 생물(초파리·까마귀·돼지·원숭이) + D 현장(블록 도로) |
| 시즌 | 기본 |
| 대결 | 채널을 다 쓸까, 잘 골라 쓸까 → 결과 **F**(초파리 81.3% vs 주판봇 27.3%, 차이 54%p) |
| 새로 그릴 그림 | P1 3장 · P2 3장 · P3 2장 |
| 재사용 | 표정 16장 (캐릭터 팩 `sprites_96.js`, 이미 페이지에 들어 있음) |
| 그림이 없을 때 | 페이지는 픽셀 동물·대체 표지(캔버스)로 이미 완성 상태 |

## 1. 그림체와 고정 외형
- 스타일: 스킬 18-3 (16비트 RPG 픽셀아트, 굵은 외곽선, 2~3단계 명암)
- 캐릭터 고정 외형: 캐릭터 팩 18-4 그대로 (주판봇은 v2 기준: 베이지 CRT 몸체, 초록 화면 얼굴, 주판알 안테나, 무한궤도)
- 장소: 밤의 연구실 옆 **블록 들판** (일반 정육면체 블록, 특정 게임의 텍스처·로고·몹 디자인을 따라 하지 않음)
- 실존 인물(머스크 등)·회사 로고·실제 칩 제품 모양은 그리지 않는다. 칩은 "작은 동전 모양 장치"로만.

## 2. 필요한 그림 전체

| # | 키 | 판 | 크기 | 상태 | 우선 | 들어가는 곳 | 대신 쓰는 그림 |
|---|---|---|---|---|---|---|---|
| 0 | cover_4 | L | 1920×1080 | 새로 (COVER_4_neuralink.md) | P1 | 맨 위 표지 | 캔버스 대체 표지 |
| 1 | sc_4_hero | E | 1200×800 | 새로 | P1 | 히어로 무대(선택) | 표지 |
| 2 | cut_4_brains | G | 960×540 | 새로 | P1 | 동물 뇌 대시보드 머리 | 없음(캔버스 점구름) |
| 3 | cut_4_pipe | G | 960×540 | 새로 | P2 | ③ 데이터 파이프 위 | 캔버스 애니메이션 |
| 4 | cut_4_pong | G | 960×540 | 새로 | P2 | ④ 강화학습 위 | 픽셀 원숭이 |
| 5 | sc_4_outro | E | 1200×800 | 새로 | P2 | 아웃트로 | 말풍선 4개 |
| 6 | thumb_4 | I | 600×400 | 새로 (표지 자르기) | P3 | 목차 카드 | 색 카드 |
| 7 | og_4 | K | 1200×630 | 새로 (표지 자르기) | P3 | 공유 미리보기 | 없음 |
| — | 표정 16장 | A~D | 96px | 재사용 | — | 말풍선·대결 | — |
| — | 픽셀 동물·차, 뇌 점구름 | — | — | 코드 | — | 캔버스 | — |

## 3. 새로 그릴 그림 상세

### 3-1. `sc_4_hero` — 블록 들판의 네 동물과 연구실 넷
| 항목 | 내용 |
|---|---|
| 구도 | 앞줄 블록 위에 초파리·까마귀·돼지·원숭이 몹, 오른쪽 멀리 카메라 달린 상표 없는 블록 차. 뒤에 박사(가운데 뒤), 조수(왼쪽 옆), 초파리 연구원(왼쪽, 오른쪽을 봄), 주판봇(오른쪽, 왼쪽을 봄) |
| 표정 | 호기심, 결과 전 (승패 암시 없음) |
| 대체 글 | 블록 들판에서 연구실 네 캐릭터가 초파리·까마귀·돼지·원숭이와 자율주행차를 바라보는 장면 |
```
16-bit RPG style pixel art, bold dark outline, 2–3 tone shading, small highlights, consistent with the reference images, cozy night laboratory mood, purple light, soft magenta and green fluorescent accents, 3:2 landscape scene, medium brightness, a field of generic cube blocks beside a night lab, four small animals standing on blocks in a row: a fruit fly, a dark crow, a pink pig, a small brown macaque monkey, a generic unbranded blocky car with a small roof camera far right, behind them the four lab characters from the reference images: the scientist at the back center, the pink-haired assistant at the left side, the fruit fly researcher on the left facing right, the abacus CRT robot on the right facing left, curious friendly rivalry, no text, no letters, no numbers, no logos, no weapons, no cigarettes, no alcohol, no blood, no real brands
```

### 3-2. `cut_4_brains` — 네 개의 뇌 홀로그램
| 항목 | 내용 |
|---|---|
| 구도 | 연구실 탁자 위 네 개의 빛나는 뇌 홀로그램(크기 순: 작은 초파리 뇌, 빽빽한 점의 까마귀 뇌, 주름진 돼지 뇌, 둥근 원숭이 뇌). 조수가 옆에서 가리킴 |
| 피할 것 | 해부학 단면·피, 실제 뇌 사진 느낌 |
| 대체 글 | 연구실 탁자 위에 크기가 다른 네 동물의 뇌 홀로그램이 떠 있는 컷 |
```
16-bit RPG style pixel art, bold dark outline, 2–3 tone shading, consistent with the reference images, cozy night laboratory mood, 16:9 illustration panel, four glowing holographic brains floating above a lab table in a row from small to large: a tiny insect brain with two side lobes, a compact bird brain made of dense small dots, a folded pig brain, a rounder folded monkey brain, the pink-haired assistant from the reference pointing at them, no text, no letters, no numbers, no logos, no blood, no real brands
```

### 3-3. `cut_4_pipe` — 아날로그에서 디지털로
| 항목 | 내용 |
|---|---|
| 구도 | 왼쪽 돼지 몹 머리 위 작은 동전 모양 장치에서 물결선이 나와 계단 모양 선, 0/1 블록 조각으로 바뀌며 오른쪽 모니터로 날아감. 주판봇이 모니터 옆에서 주판을 듦 |
| 대체 글 | 돼지 머리 위 장치에서 나온 물결 신호가 계단 모양 디지털 신호로 바뀌어 모니터로 가는 컷 |
```
16-bit RPG style pixel art, bold dark outline, consistent with the reference images, 16:9 illustration panel, a pink pig on a treadmill with a small glowing coin-shaped device on its head, a wavy signal line rising from it turns into a stepped line and then into small square bits flying to a monitor, the abacus CRT robot from the reference standing by the monitor holding an abacus, no text, no letters, no numbers, no logos, no real brands
```

### 3-4. `cut_4_pong` — 보상으로 배우는 원숭이
| 항목 | 내용 |
|---|---|
| 구도 | 작은 원숭이가 화면 속 막대-공 게임을 보고, 옆 빨대 컵(과일 음료, 상표 없음). 초파리 연구원이 클립보드에 기록 |
| 피할 것 | 실제 영상 캡처 구도, 실험 장치의 사실적 묘사 |
| 대체 글 | 원숭이가 막대-공 게임 화면을 보고 옆에 과일 음료 컵이 놓인 컷 |
```
16-bit RPG style pixel art, bold dark outline, consistent with the reference images, 16:9 illustration panel, a small brown macaque monkey watching a simple paddle-and-ball game on a screen, a cup of fruit smoothie with a straw next to it, the fruit fly researcher from the reference taking notes on a clipboard, no text, no letters, no numbers, no logos, no real brands
```

### 3-5. `sc_4_outro` — 결과 F 아웃트로
| 항목 | 내용 |
|---|---|
| 구도 | 초파리 연구원이 앞에서 팔짱(이긴 쪽 앞·크게), 주판봇은 같은 화면에서 한숨 쉬며 주판을 내림(인정하는 몸짓), 박사 엄지, 조수 점수판 |
| 대체 글 | 대결이 끝난 뒤 초파리 연구원이 앞에 서고 주판봇이 웃으며 인정하는 아웃트로 장면 |
```
16-bit RPG style pixel art, bold dark outline, consistent with the reference images, cozy night laboratory mood, 3:2 landscape scene, the fruit fly researcher in front with arms crossed and a proud look, the abacus CRT robot beside him sighing good-naturedly and lowering its abacus, the scientist giving a thumbs up at the back, the pink-haired assistant holding a blank scoreboard, no text, no letters, no numbers, no logos, no real brands
```

## 4. 일관성 지침
- 참고 이미지: 캐릭터 팩 기본 그림 4장(`fruitfly-lab-expressions`), 주판봇은 v2 단체 사진 기준
- 같은 세션에서 연달아 생성, 표정만 바꿀 때: *same character, same size and position, only change the facial expression and pose to ...*
- 투명 배경이 필요 없는 장면·컷만 새로 그림

## 5. 넘겨받은 뒤 처리
1. 크기 확인 → WebP 압축 (E 760폭, G 640폭)
2. `data-img` 키 자리에 넣고, 페이지 그림 합계 표지 포함 600 KB 이하 확인 (현재 표정 16장 약 90 KB 포함 페이지 304 KB)
3. 표지는 스킬 18-15 절차

## 6. 매니페스트
```json
{"page":"4_neuralink_animal_brain_ai","anchor":"A:bio + D:block-road","season":"default","duel":{"result":"F","gap":0.54},
 "images":[
  {"key":"cover_4","plate":"L","size":[1920,1080],"status":"new","priority":"P1","slot":"cover","fallback":"canvas-cover","alt":"밤의 연구실 블록 들판에서 네 캐릭터가 초파리·까마귀·돼지·원숭이와 자율주행차를 바라보는 표지"},
  {"key":"sc_4_hero","plate":"E","size":[1200,800],"status":"new","priority":"P1","slot":"hero-stage","fallback":"cover_4"},
  {"key":"cut_4_brains","plate":"G","size":[960,540],"status":"new","priority":"P1","slot":"#brains","fallback":"canvas"},
  {"key":"cut_4_pipe","plate":"G","size":[960,540],"status":"new","priority":"P2","slot":"#lv3","fallback":"canvas"},
  {"key":"cut_4_pong","plate":"G","size":[960,540],"status":"new","priority":"P2","slot":"#lv4","fallback":"pixel"},
  {"key":"sc_4_outro","plate":"E","size":[1200,800],"status":"new","priority":"P2","slot":"#outro","fallback":"say-bubbles"},
  {"key":"thumb_4","plate":"I","size":[600,400],"status":"new","priority":"P3","slot":"index-card","fallback":"cover_4 crop"},
  {"key":"og_4","plate":"K","size":[1200,630],"status":"new","priority":"P3","slot":"og","fallback":"none"}]}
```
