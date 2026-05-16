# `web/public/og/` — 라스터 OG 후속 차환 슬롯

> 2026-05-16 EOD 신설 (web-lead 김민준 자율).

## 현재 상태 (2026-05-16)

- `opengraph-image.tsx` SSG 빌드 타임 PNG 78건 = 1차 fallback a (시각 메타 정합).
- chapter_01 (`v2_0-1`) = 한지우 character_key_visual v1.0 §2.1 + §2.2 정합 강화 분기 채택.
- 라스터 PNG 차환 = 류재현 Vertex AI Imagen 3 후속 발주 슬롯 (5/22 D-day 또는 5/22 직후).

## 차환 절차 (한지우 v1.0 §6.2)

1. 류재현 Vertex AI Imagen 3 호출 — 한지우 `designs/graphics/character_key_visual_v2_9_set/01_park_jeongju.md` §2.3 프롬프트 + §2.4 negative 풀 인용
2. 1차 출력 4~8장 중 한지우 시각 검수
3. PD 시각 사인 (있으면, 없으면 한지우 자율 채택)
4. 김민준 `web/public/og/v2_0_chapter_01.png` 박힘 (1200×630, sRGB, < 200KB)
5. `opengraph-image.tsx` `renderJeongjuOG` 분기 = 라스터 직접 import 또는 SVG 메타 + 라스터 background 혼합 옵션
6. `npm run deploy` 1회 재배포

## 4 가드레일 (한지우)

- border-radius 4px (UI 적용 시)
- 그라디언트 0
- 순백 0
- 파란강조 0

## 후속 캐릭터 시드

- `01_park_jeongju.md` — 5/14 도착 ✓ (1체)
- `02_jinie.md` — 5/14 도착 ✓
- `03_dobby.md` — 5/14 도착 ✓
- 04~09 = 한지우 5/19 D+8 9체 시드 완성 자율 슬롯
