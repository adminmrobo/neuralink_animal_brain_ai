# 표지 지시문 — 목차 (index.html)

| 항목 | 내용 |
|---|---|
| 키 · 판 | `cover_index` · L (16:9, 가로 1920 이상) |
| 넣을 곳 | `assets/img/cover_index.webp` (1600×900, 220 KB 이하) — 넣으면 index.html이 자동으로 바꿔 씀 |
| 장소 (앵커) | 밤의 연구실 안 (B 연구실) — 본편 표지(블록 들판)와 겹치지 않게 실내 |
| 주제 은유 | 연구실 가운데 큰 원형 홀로그램 테이블 위에 네 동물의 뇌가 떠 있고, 그 신호가 한 줄로 모여 천장 근처의 작은 드론으로 이어진다 — "동물 뇌의 결론으로 드론을 띄운다" |
| 네 캐릭터 포즈 | 박사: 테이블 뒤 가운데, 두 팔을 벌려 홀로그램을 소개 / 조수(하루): 왼쪽 옆, 태블릿(빈 화면)을 든 채 드론을 올려다봄 / 초파리 연구원: 왼쪽 앞, 오른쪽을 보며 초파리 뇌 홀로그램을 가리킴 / 주판봇: 오른쪽 앞, 왼쪽을 보며 주판을 들고 큰 뇌(원숭이)를 가리킴 |
| 대체 글 (alt) | 밤의 연구실에서 네 캐릭터가 동물 뇌 홀로그램과 드론을 둘러싼 목차 표지 |
| 본편 표지와 다른 점 | 본편 `cover_4`는 바깥 블록 들판 + 동물 몹 + 자동차. 목차는 실내 + 뇌 홀로그램 + 드론 |

**참고 이미지 (함께 올리기):** 네 캐릭터 기본 그림 4장 (기준: GitHub `adminmrobo/fruitfly-lab-expressions`, 주판봇은 v2 단체 사진 기준).

**Genspark에 붙여 넣기 ↓**
```
웹페이지 맨 위에 거는 표지 그림 1장을 만들어 줘.
- 비율 16:9, 가로 1920px 이상
- 첨부한 참고 이미지의 네 캐릭터(박사, 조수, 초파리 연구원, 주판봇)를 같은 그림체·같은 외형으로, 넷 모두 등장
- 그림 안에 글자·숫자·로고를 넣지 말 것. 실존 인물, 실제 회사 로고, 실제 칩·드론 제품 모양을 그리지 말 것
- 뇌는 빛나는 홀로그램으로만, 해부 단면이나 피는 그리지 말 것
- 얼굴과 손은 가장자리에서 떨어진 가운데 영역에, 왼쪽 아래 구석은 어둡고 단순하게
아래 영어 프롬프트를 그대로 써 줘.

Website top cover illustration, wide 16:9.
Match the art style, proportions and colors of the attached reference images exactly.
Cozy night laboratory mood, purple light, soft magenta and green fluorescent accents.
Scene: inside a night laboratory with shelves of glowing monitors and test tube racks, a large round holographic table in the center.
All four characters together:
  the scientist with thin teal glasses, black hair with one white streak and a small ponytail in a white lab coat over a black vest and tie, standing behind the table at the center with both arms open, presenting;
  the girl assistant with long pink hair in two round buns and a navy streak, at the left side holding a tablet with a blank screen, looking up at the drone;
  the anthropomorphic fruit fly researcher with big red compound eyes and a blue helmet with a gold stripe, front left, facing right, pointing at the smallest hologram;
  the boxy beige retro CRT-monitor robot with a dark green screen face, mint pixel eyes, an antenna topped with a red-brown abacus bead and small tank treads, front right, facing left, holding a wooden abacus and pointing at the largest hologram.
Visual metaphor of the topic: above the table float four glowing holographic brains in a row from small to large — a tiny insect brain, a compact bird brain made of dense dots, a folded pig brain with a tiny glowing coin-shaped device on top, a rounder folded monkey brain; thin light lines rise from all four and merge into one bright line that reaches a small generic quadcopter drone hovering near the ceiling.
Composition: keep every face and hand inside the central safe area (12% margin left and right, 10% top, 18% bottom); keep the bottom-left corner dark and simple; the light falls on the merging line and the drone.
Mood: curious, friendly rivalry, the moment before the result.
No text, no letters, no numbers, no logos, no weapons, no cigarettes, no alcohol, no blood, no real brands, no real people.
```

**고칠 때 (같은 대화에서):** `Same four characters, same art style and composition. Change only: {고칠 점}. Still no text.`

**받은 뒤 처리 (스킬 18-15):** 16:9 확인 → 글자 없는지 확인 → 네 캐릭터 외형 확인 → WebP 1600×900(220 KB 이하) + 960×540(110 KB 이하) → `assets/img/cover_index.webp` 로 올림 → 390·768·1280 폭에서 얼굴 잘림 확인.
