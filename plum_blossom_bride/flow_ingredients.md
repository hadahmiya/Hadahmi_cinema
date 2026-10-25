# Flow 공통 레퍼런스 — 룩 & 고증 가이드 (전 10화 공용)

## 0. 비주얼 콘셉트: "밝고 맑은 조선"
레퍼런스 무드: 드라마 〈옥씨부인전〉(2024–25)의 톤 — **자연광 위주의 하이키 화면, 맑은 공기감, 파스텔 계열 한복과 초록 자연의 조화, 고증 디테일은 단정하게.**
※ Flow 프롬프트에는 작품명·배우명을 넣지 않고 아래처럼 *룩을 말로 풀어* 넣는다 (모델이 이름을 모르거나 정책상 거부할 수 있음).

| 원칙 | 적용 |
|---|---|
| **밝기** | 낮 장면은 부드러운 순광/역광 햇살. 밤 장면도 "어두운 밤"이 아니라 **달빛 + 등불로 환한 블루아워**. 비극 장면도 따뜻한 촛불로 밝고 아름답게(어둡고 칙칙한 톤 금지) |
| **팔레트** | 바탕: 한지 아이보리 · 소나무/버들 초록 · 기와 회청 · 나무 기둥 꿀색. 의상: 연분홍 · 옥색 · 연두 · 연노랑 · 연보라 같은 **파스텔** + 포인트로 **다홍 · 자주 · 쪽빛** |
| **조화 규칙** | 한 화면 안에 파스텔 2–3색 + 진한 포인트 1색. 인물마다 고유 색을 정해 화면에서 바로 구분되게 |
| **질감** | 명주·모시·비단의 은은한 광택, 한지 문살로 걸러진 확산광, 반사판 느낌의 깨끗한 피부톤 |

## 1. [STYLE] — 모든 컷 끝에 붙임
```
Bright, airy Korean historical drama look set in late Joseon (18th century). High-key natural lighting, soft diffused sunlight filtered through hanji paper doors, clean luminous skin tones, gentle lens bloom. Harmonious pastel palette of soft peach-pink, celadon jade, spring green, butter yellow and pale lilac, accented by vermilion, deep plum-purple and indigo. Lush green pine and willow, ivory hanji, grey-blue roof tiles, honey-colored wood. Historically accurate hanbok in fine silk and ramie with delicate sheen. Shot on 35mm, shallow depth of field, smooth gentle camera movement, photorealistic, 4K, no text, no subtitles, no watermark.
```

## 2. [NIGHT] — 밤 장면은 STYLE 뒤에 추가
```
Luminous blue-hour night, bright full moonlight with warm glowing lanterns, faces clearly and softly lit, rich but not dark, dreamy and romantic.
```

## 3. [FLASHBACK] — 회상 컷은 STYLE 대신
```
Warm dreamlike flashback, overexposed golden spring sunlight, gentle haze and bloom, soft pastel colors, late-Joseon Korea, 35mm film, no text.
```

## 4. [NEG]
```
dark gloomy lighting, heavy shadows, desaturated grey image, Chinese hanfu, Japanese kimono, modern objects, modern hairstyles, makeup with heavy eyeliner, distorted hands, extra fingers, text, logo, cartoon, anime
```

---

## 5. 고증 메모 (프롬프트에 반영됨)
- **미혼 여성은 땋은머리 + 댕기**, 비녀는 혼인 후 쪽머리에만 꽂는다 → 서연의 은비녀는 *어머니의 유품*으로 평소엔 **주머니(노리개)에 넣어 다니고**, 혼례 이후에만 머리에 꽂는다.
- **세자빈 예복 = 자적(紫赤)원삼** (왕비 홍원삼, 공주·반가 녹원삼과 구분). 혼례 후 침전에서는 화관을 쓴 채.
- **왕세자 곤룡포 = 아청색(짙은 남청) + 사조룡(발톱 4개) 보**, 익선관. (붉은 대홍 곤룡포는 왕의 것)
- **녹의홍상(연두 저고리 + 다홍치마)** = 혼기 찬 규수의 대표적 성장(盛裝). 서연의 각성 의상.
- 저고리는 18세기식 **짧은 길이·좁은 소매**, 치마는 가슴 위로 높게 여밈. 반가 여성은 **삼회장 저고리**(깃·끝동·곁마기·고름 색 다르게).
- 첫날밤 술은 원래 **합환주(근배)** — 1화의 독은 '피로를 푸는 차'로 위장한 나인을 통해 들어온다.
- 정월대보름 밤 **다리밟기(답교놀이)**: 한양 청계천 돌다리(수표교 형태)에서 등불을 들고 다리를 건너는 풍습 → 1화 다리 장면의 근거.
- 세자의 반가면은 **극적 각색 요소**(고증 외). 외출복은 고증대로 옥색 도포 + 흑립.

---

## 6. 인물 레퍼런스 (이미지 생성용)
모든 프롬프트 앞에 `Full-body character reference, front and three-quarter view,`, 뒤에 `plain warm ivory background, bright soft studio light, photorealistic, historically accurate late-Joseon hanbok.` 를 붙인다.

| 이름 | 고유색 | 프롬프트 |
|---|---|---|
| **@SEOYEON** | 연분홍 × 옥색 | `a 19-year-old Korean noble maiden, delicate oval face, clear bright dark-brown eyes, gentle but intelligent expression, natural fresh makeup, long black hair in a single low braid tied with a deep plum-purple daenggi ribbon, wearing a short soft peach-pink samhoejang jeogori with deep plum-purple collar, cuffs and ties, and a high-waisted celadon jade-green silk chima, a small embroidered silk pouch norigae at her waist` |
| **@SEOYEON_HONGSANG** | 연두 × 다홍 (녹의홍상) | 같은 얼굴·머리, `wearing a spring-green jeogori with deep plum-purple ties and cuffs and a vivid vermilion-red silk chima with a subtle gold-leaf hem (the traditional nogui-hongsang maiden's formal dress), jade butterfly norigae` |
| **@SEOYEON_BRIDE** | 자적 × 금 | 같은 얼굴, `as a crown princess bride: deep plum-red (jajeok) wonsam ceremonial robe with gold-leaf phoenix patterns and rainbow-striped sleeves, jeweled hwagwan flower crown, hair in a married chignon with a plain silver binyeo hairpin, red yeonji-gonji dots on cheeks and forehead` |
| **@HWAN** | 아청 × 금 | `a 24-year-old Korean crown prince, tall, sharp jawline, warm deep eyes, calm dignified expression, wearing a deep indigo-blue (acheong) gonryongpo robe with gold four-clawed dragon roundels on chest and shoulders, black ikseongwan winged cap, jade belt, black boots` |
| **@HWAN_MASK** | 옥색 × 흑 | 같은 얼굴, `incognito as a scholar: pale celadon-blue silk dopo robe with a thin dark sash, black horsehair gat hat with bead strap, an elegant black lacquered half-mask covering eyes and nose` |
| **@HWAN_WEDDING** | 아청 × 금 | @HWAN과 동일 의상, 가례 당일 버전 (`gold embroidery gleaming, a red silk ribbon at the belt`) |
| **@HWARYEONG** | 연노랑 × 장미분홍 | `a 21-year-old Korean noble maiden, round pretty face, sweet bright smile that does not reach her eyes, long braid with a rose-pink daenggi and small gold ornaments, butter-yellow jeogori with subtle gold-leaf trim and rose-pink ties, a rose-pink silk chima, a small red knotted silk perfume pouch (hyangnang) tied at her waist` |
| **@HWARYEONG_NAIN** | 연두 × 남 | 같은 얼굴, `disguised as a palace maid (nain): pale green jeogori, navy chima, hair in a plain braided court bun` |
| **@LADYMIN** | 회청 × 쪽빛 | `a 45-year-old Korean noble matriarch, elegant but cold narrow eyes, thin smile, married chignon with a jade binyeo, slate-blue jeogori with indigo ties and a deep indigo chima, carved jade ring` |
| **@DALI** | 생성 × 남 | `a 16-year-old Korean servant girl, bright round eyes, freckles, cheerful face, single long braid with a faded red daenggi, plain undyed cotton jeogori and a navy cotton chima with a white apron tied at the waist` |
| **@EUNUCH_PARK** | 청록 | `a 50-year-old Joseon palace eunuch, kind smiling wrinkled face, beardless, teal-green official robe with round collar, black official hat` |
| **@JO** | 홍 | `a 60-year-old Joseon high official, gaunt face, grey goatee, deep red danryeong official robe with crane insignia, black samo hat` |
| **@DOWAGER** / **@DOWAGER_HAND** | 진남 × 금 | `a 65-year-old Korean Queen Dowager, regal and icy, large formal court wig (eoyeomeori) with gold ornaments, deep navy dangui with gold phoenix embroidery, carved green jade dragon ring` / 손 클로즈업만: `elderly royal hand with a carved green jade dragon ring, navy silk sleeve with gold embroidery` |
| **@SHAMAN** | 오방색 | `an ageless Korean female shaman (mudang), long white hair, layered robes in the five traditional colors (blue, red, yellow, white, black), brass bells in hand, piercing kind eyes` |
| **@YOUNG_SEOYEON** / **@YOUNG_HWAN** | | `8-year-old girl in a rainbow-striped saekdong jeogori and pink chima, two short braids with red daenggi` / `14-year-old boy prince in a pale blue robe and small black hat, tear-stained face` |

## 7. 장소 레퍼런스
모든 프롬프트 뒤에 `bright, historically accurate late-Joseon architecture, photorealistic, wide establishing shot.`

| 이름 | 프롬프트 |
|---|---|
| **@LOC_BRIDAL** | `crown princess's bridal chamber in the palace at night, glowing warm with dozens of tall red candles, ivory hanji walls, a ten-panel peony folding screen, layered red and ivory silk bedding, low lacquer table with mother-of-pearl inlay, everything bathed in soft golden light` |
| **@LOC_HOUSE** | `a modest noble family hanok in early spring morning, sunlit wooden maru porch, ivory paper doors, a white plum tree in full bloom in the courtyard, earthen walls, clay jars, soft green hills behind` |
| **@LOC_SEOYEON_ROOM** | `a young noblewoman's sunlit room in a hanok, hanji lattice doors glowing with morning light, a folding screen with flower-and-bird painting, embroidered cushions, a small bronze mirror stand, a lacquered mother-of-pearl chest` |
| **@LOC_BRIDGE** | `a granite stone bridge over the Cheonggyecheon stream in Hanyang on the first full moon night of the lunar year, crowds in white and pastel hanbok carrying paper lanterns, lanterns reflected on the water, huge bright full moon, willow trees` |
| **@LOC_PRINCE_ROOM** | `crown prince's study in the East Palace, warm wooden floor, low writing desk with brushes and inkstone, bookshelves of bound books, a lacquered treasure box, lattice windows with moonlight and candle glow` |
| **@LOC_MIN_ROOM** | `the lady of the house's inner room (anbang) in a hanok, refined furniture, a ten-panel embroidered screen, lamp light, wealthy but austere` |
| **@LOC_TEAHALL** | `a bright palace hall with red lacquered pillars and colorful dancheong beams, polished wooden floor, rows of low tea tables, sunlight streaming through open lattice doors` |
| **@LOC_LIBRARY** | `royal library with tall wooden shelves of books and scrolls, sunbeams with dust motes` |
| **@LOC_SNOWCOURT** | `palace courtyard covered in fresh white snow, granite path, warm lanterns, softly glowing snowfall` |
| **@LOC_PAVILION** | `a royal pavilion over a lotus pond under a bright full moon, lanterns on the eaves, reflections on calm water` |
| **@LOC_SHRINE** | `a mountain seonangdang shrine with a sacred tree tied with five-colored cloth strips, stone cairn, golden-hour light` |
| **@LOC_PRISON** | `royal prison with wooden bars and straw floor, shafts of pale light through a high window` |
