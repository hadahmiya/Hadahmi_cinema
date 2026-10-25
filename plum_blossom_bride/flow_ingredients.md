# Flow 공통 레퍼런스 (전 10화 공용)

## 사용법
1. 아래 프롬프트로 이미지를 만들고 Flow 프로젝트에 **이름 그대로** 저장 (`@SEOYEON` 등).
2. 각 컷 생성 시 표기된 `@` 레퍼런스를 *Ingredients to Video*로 첨부 → 컷 프롬프트 붙여넣기.
3. `→ EXTEND` 표시는 직전 컷의 마지막 프레임에서 이어 생성.
4. 16:9 권장(쇼츠 재가공 시 9:16 리프레임). 컷당 3–4테이크 생성 후 베스트 선택.

## [STYLE] — 모든 컷 끝에 붙임
```
Cinematic Joseon-dynasty Korean period drama, shot on 35mm anamorphic lens, shallow depth of field, soft volumetric light, historically accurate hanbok silk textures, color palette of jade green, deep crimson, antique gold and ink black, subtle film grain, elegant slow camera movement, 4K, no text, no subtitles, no watermark.
```

## [NEG]
```
Chinese or Japanese costume, kimono, hanfu, modern objects, distorted hands, extra fingers, text, logo, cartoon style
```

## [FLASHBACK] — 회상 컷에 STYLE 대신
```
Soft warm dreamlike flashback, overexposed golden haze, gentle bloom, slightly desaturated, Joseon-dynasty Korea, 35mm film, no text.
```

---

## 인물
| 이름 | 프롬프트 (앞에 `Character reference sheet, front and three-quarter view,` / 뒤에 `neutral grey background, soft studio light, photorealistic.`) |
|---|---|
| **@SEOYEON** | `a 19-year-old Korean noblewoman of the Joseon dynasty, delicate oval face, clear dark-brown eyes, calm intelligent gaze, black hair in a low chignon held by a single plain silver binyeo hairpin, pale jade-green jeogori with a deep indigo chima` |
| **@SEOYEON_CRIMSON** | 위와 동일 얼굴, `pure white jeogori with a deep crimson chima` (각성 후 기본 의상) |
| **@SEOYEON_BRIDE** | 위와 동일 얼굴, `green wonsam bridal robe with gold patterns, gold flower crown (hwagwan), red dots on cheeks and forehead (yeonji-gonji)` |
| **@HWAN** | `a 24-year-old Korean crown prince of the Joseon dynasty, sharp jawline, deep gentle eyes that turn cold in public, crimson gonryongpo royal robe with golden dragon roundels, black ikseongwan winged cap, jade belt` |
| **@HWAN_MASK** | 위와 동일 얼굴, `black dopo robe, black gat hat, a black half-mask covering the upper face` |
| **@HWAN_WEDDING** | 위와 동일 얼굴, `deep crimson royal wedding robe (myeonbok style) with gold embroidery, ceremonial crown` |
| **@HWARYEONG** | `a 21-year-old Korean noblewoman, round soft face, sweet innocent smile that does not reach her eyes, ornate gold tteoljam hairpins, peach-pink jeogori with pale green chima, a small red knotted silk perfume pouch tied at her sleeve` |
| **@LADYMIN** | `a 45-year-old Korean noble matriarch, cold narrow eyes, thin lips, formal chignon with gold binyeo, deep purple dangui jacket, jade ring` |
| **@DALI** | `a 16-year-old Korean servant girl of the Joseon dynasty, bright round eyes, freckles, single long braid with red daenggi ribbon, plain beige cotton hanbok` |
| **@EUNUCH_PARK** | `a 50-year-old Joseon palace eunuch, kind wrinkled face, beardless, dark green official robe, black hat` |
| **@JO** | `a 60-year-old Joseon high official, gaunt face, grey goatee, dark red gwanbok official robe with crane insignia, black samo hat` |
| **@DOWAGER** | `a 65-year-old Korean Queen Dowager, regal and icy, elaborate eoyeomeori wig with gold ornaments, deep blue dangui with gold phoenix embroidery, carved dragon jade ring` (4화까지는 `@DOWAGER_HAND`: 반지 낀 손 클로즈업만) |
| **@SHAMAN** | `an ageless Korean female shaman (mudang), long white hair, colorful obangsaek layered robes, bells in hand, piercing eyes` |
| **@YOUNG_SEOYEON** / **@YOUNG_HWAN** | `8-year-old girl in pink saekdong hanbok with braided hair` / `14-year-old boy prince in simple blue robe, tear-stained face` |

## 장소
| 이름 | 프롬프트 |
|---|---|
| **@LOC_BRIDAL** | `Joseon royal bridal chamber at night, red silk bedding, peony folding screen, many tall red candles, paper doors, warm flickering light` |
| **@LOC_HOUSE** | `Joseon noble hanok courtyard at dawn, a blooming white plum tree, stone steps, tiled roofs, morning mist` |
| **@LOC_BRIDGE** | `Stone arch bridge over a stream during a night lantern festival, hundreds of floating lanterns on water, crowds in hanbok, warm glow` |
| **@LOC_PRINCE_ROOM** | `Crown prince's private study at night, low desk, scrolls, a lacquered box, candlelight, moonlight through lattice windows` |
| **@LOC_TEAHALL** | `Grand Joseon palace hall, red lacquered pillars, dancheong beams, low tea tables, rows of kneeling court ladies, golden light through paper windows` |
| **@LOC_LIBRARY** | `Joseon royal library, tall wooden shelves of scrolls and books, narrow aisles, dust in light beams` |
| **@LOC_SNOWCOURT** | `Snow-covered palace courtyard at night, stone path, falling snow, distant lanterns, main hall in background` |
| **@LOC_PAVILION** | `Royal pavilion over a lotus pond at night, full moon reflected on water, lanterns, dancheong eaves` |
| **@LOC_SHRINE** | `Mountain seonangdang shrine at dusk, sacred tree wrapped in five-colored cloth, stone cairn, mist` |
| **@LOC_PRISON** | `Dark Joseon royal prison, wooden bars, straw floor, single torch, cold blue moonlight` |
