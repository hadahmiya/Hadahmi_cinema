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

## 0-1. ⚠️ 한복이 일본·중국 의상으로 나오는 이유와 대책
| 원인 | 대책 (이 문서에 반영됨) |
|---|---|
| **Flow(Veo/Imagen)에는 네거티브 입력란이 없다.** `kimono`, `hanfu`를 프롬프트에 쓰면 "하지 마"가 아니라 *그 단어를 그리라는 신호*가 된다 | 네거티브 단어를 **전부 삭제**하고, 원하는 것만 긍정형으로 묘사 |
| `jeogori`, `wonsam`, `ikseongwan` 같은 한국어 고유명사는 학습 데이터가 적어 모델이 잘 모른다 → "동아시아 궁중 의상" 평균값(중국 사극 / 기모노)으로 대체 | 고유명사 + **모양을 영어로 풀어 쓰기** (아주 짧은 상의, 오른쪽 가슴의 긴 리본 매듭, 겨드랑이부터 퍼지는 종 모양 치마…) |
| `robe`, `flower crown`, `winged cap`, `palace maid`, `guards`, `hairpin` 같은 일반어 → 중국풍으로 끌려감 | 모든 의상/인물 앞에 **`Korean`, `Joseon`, `hanbok`** 을 반복 부착 |
| 넓은 소매 + 허리띠 묘사 → 기모노/한푸 실루엣 | **허리띠 없음, 좁은 소매, 하이웨이스트**를 명시 |
| 텍스트만으로 레퍼런스 이미지 생성 | **실제 한복 사진**(국립민속박물관·e뮤지엄 공공누리 이미지, 한복진흥센터 자료, 직접 촬영본)을 Flow 이미지 생성에 첨부해 `@` 레퍼런스를 만든다 — 가장 확실한 방법 |

**레퍼런스 이미지 합격 기준** (하나라도 틀리면 재생성):
- [ ] 여자 저고리가 **가슴 위에서 끝나는 짧은 길이**이고, 오른쪽 가슴에 **긴 고름 리본**이 늘어져 있다
- [ ] 치마가 **겨드랑이 높이에서 시작해** 종 모양으로 퍼지고, **허리띠(오비)가 없다**
- [ ] 깃이 **V자로 겹치고 흰 동정**이 둘려 있다
- [ ] 여자 머리가 **가운데 가르마로 납작하게** 빗겨 있다 (올림머리 장식 과다 = 중국풍)
- [ ] 남자 갓이 **넓고 반투명한 챙 + 원통형 모자 + 구슬 갓끈**이다 (삿갓·관모 형태 X)
- [ ] 세자 옷은 **둥근 깃(단령)** 에 가슴·양어깨의 **둥근 금색 용 흉배**, 모자는 뒤에 **작은 날개 두 개가 위로 선** 익선관

## 1. [STYLE] — 모든 컷 끝에 붙임
```
HANBOK ANCHOR: Korean sageuk historical drama set in Joseon-dynasty Korea; all characters are Korean people wearing authentic traditional Korean hanbok — women in very short cropped jeogori jackets ending above the chest, tied with a long ribbon bow (goreum) on the right side, white V-shaped collar strip, full bell-shaped chima skirts gathered high under the arms with no waist belt, narrow sleeves, hair smoothly center-parted; men in Korean dopo or durumagi coats and wide-brimmed translucent black horsehair gat hats. Korean hanok architecture with ondol floors and hanji paper doors.
LOOK: Bright, airy Korean historical drama look set in late Joseon (18th century). High-key natural lighting, soft diffused sunlight filtered through hanji paper doors, clean luminous skin tones, gentle lens bloom. Harmonious pastel palette of soft peach-pink, celadon jade, spring green, butter yellow and pale lilac, accented by vermilion, deep plum-purple and indigo. Lush green pine and willow, ivory hanji, grey-blue roof tiles, honey-colored wood. Historically accurate hanbok in fine silk and ramie with delicate sheen. Shot on 35mm, shallow depth of field, smooth gentle camera movement, photorealistic, 4K, no text, no subtitles, no watermark.
```

## 2. [NIGHT] — 밤 장면은 STYLE 뒤에 추가
```
Luminous blue-hour night, bright full moonlight with warm glowing lanterns, faces clearly and softly lit, rich but not dark, dreamy and romantic.
```

## 3. [FLASHBACK] — 회상 컷은 STYLE 대신
```
Warm dreamlike flashback, overexposed golden spring sunlight, gentle haze and bloom, soft pastel colors, late-Joseon Korea, 35mm film, no text.
```

## 4. 네거티브는 쓰지 않는다
Flow에는 네거티브 입력란이 없으므로 **금지어를 프롬프트에 넣지 않는다.** 대신 위 `HANBOK ANCHOR` + `LOOK`의 긍정형 묘사로 통제한다.
(Flow 밖의 이미지 도구 — 예: 네거티브 칸이 따로 있는 Midjourney `--no`, SD negative — 에서만 `kimono, hanfu, obi belt, wide sleeves, Chinese crown, dark lighting` 을 별도 칸에 넣는다.)

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
모든 프롬프트 앞에 `Full-body character reference photo for a Korean sageuk drama, front and three-quarter view, a Korean person wearing authentic traditional Korean hanbok,`, 뒤에 `plain warm ivory background, bright soft studio light, photorealistic, styled like a Korean Folk Museum hanbok reconstruction.` 를 붙인다.
가능하면 실제 한복 사진 1장을 함께 첨부한다.

| 이름 | 고유색 | 프롬프트 |
|---|---|---|
| **@SEOYEON** | 연분홍 × 옥색 | `a 19-year-old Korean noble maiden, delicate oval Korean face, clear bright dark-brown eyes, gentle intelligent expression, natural fresh makeup, black hair smoothly center-parted and woven into one long single braid down her back tied at the end with a deep plum-purple daenggi ribbon. She wears a Korean samhoejang jeogori: a very short cropped soft peach-pink silk jacket ending above the chest, with a deep plum-purple V-collar, white dongjeong collar strip, plum-purple cuffs and a long plum-purple goreum ribbon bow hanging on the right chest; and a full celadon jade-green chima skirt wrapped high under the arms, flaring like a bell to the floor, no belt. A small embroidered Korean silk pouch norigae with tassel hangs at her side` |
| **@SEOYEON_HONGSANG** | 연두 × 다홍 (녹의홍상) | 같은 얼굴·땋은 머리, `wearing the Korean nogui-hongsang maiden's formal hanbok: a very short cropped spring-green silk jeogori with deep plum-purple goreum ribbon and cuffs and white collar strip, and a full vivid vermilion-red chima skirt gathered high under the arms with a gold-leaf band at the hem, no belt, a jade butterfly norigae with long red tassel` |
| **@SEOYEON_BRIDE** | 자적 × 금 | 같은 얼굴, `as a Joseon crown princess bride in Korean royal wedding hanbok: a deep plum-red jajeok wonsam — a long front-open Korean ceremonial overcoat with wide rainbow-striped sleeve bands (saekdong) and long white hansam cuffs, gold-leaf phoenix pattern, worn over a vermilion chima; a small Korean jeweled hwagwan headpiece on top; hair in a low flat married chignon (jjokmeori) at the nape held by one plain silver binyeo; round red yeonji-gonji dots on both cheeks and forehead` |
| **@HWAN** | 아청 × 금 | `a 24-year-old Korean crown prince, tall, sharp jawline, warm deep eyes, calm dignified expression, wearing the Joseon royal gonryongpo: a deep indigo-blue (acheong) silk robe with a round collar (danryeong style), circular gold-embroidered four-clawed dragon badges on the chest, back and both shoulders, a stiff wide jade-plaque belt worn loose at the waist; a black Korean ikseongwan cap — a rounded black silk cap with two small rounded flaps standing upward at the back; black leather boots` |
| **@HWAN_MASK** | 옥색 × 흑 | 같은 얼굴, `incognito as a Korean seonbi scholar: a pale celadon-blue Korean dopo overcoat with a slit back panel and a thin dark-blue silk cord sash (sejodae) tied at the chest, a black Korean gat hat with a very wide flat translucent horsehair brim, tall cylindrical crown and a long bead chin strap, an elegant black lacquered half-mask covering eyes and nose` |
| **@HWAN_WEDDING** | 아청 × 금 | @HWAN과 동일한 한국 곤룡포 + 익선관, 가례 당일 버전 (`gold dragon badges gleaming, a red silk ribbon at the jade belt`) |
| **@HWARYEONG** | 연노랑 × 장미분홍 | `a 21-year-old Korean noble maiden, round pretty Korean face, sweet bright smile that does not reach her eyes, black hair center-parted in one long single braid with a rose-pink daenggi ribbon, wearing a very short cropped butter-yellow Korean jeogori with a thin gold-leaf border, rose-pink goreum ribbon bow on the right chest and white collar strip, and a full rose-pink chima skirt gathered high under the arms, no belt, a small red knotted Korean silk hyangnang perfume pouch hanging at her side` |
| **@HWARYEONG_NAIN** | 연두 × 남 | 같은 얼굴, `disguised as a Joseon palace maid (nain): short pale green Korean jeogori with white collar strip, full navy chima, hair braided and pinned in a simple low Korean court bun with a small black ribbon` |
| **@LADYMIN** | 회청 × 쪽빛 | `a 45-year-old Korean noble matriarch, elegant but cold narrow eyes, thin smile, hair in a low flat married Korean chignon at the nape with a jade binyeo, wearing a short slate-blue Korean jeogori with indigo goreum ribbon and white collar strip and a full deep indigo chima, carved jade ring` |
| **@DALI** | 생성 × 남 | `a 16-year-old Korean servant girl of Joseon, bright round eyes, freckles, cheerful face, hair center-parted in one long braid with a faded red daenggi, plain undyed cotton Korean jeogori with short ties and a navy cotton chima hitched up, white cotton apron` |
| **@EUNUCH_PARK** | 청록 | `a 50-year-old Joseon palace eunuch, kind smiling wrinkled Korean face, beardless, teal-green Korean danryeong official robe with round collar and a black Korean samo official hat with two horizontal side wings` |
| **@JO** | 홍 | `a 60-year-old Joseon high official, gaunt Korean face, grey goatee, deep red Korean danryeong official robe with a square crane insignia badge on the chest, black Korean samo hat with two horizontal side wings` |
| **@DOWAGER** / **@DOWAGER_HAND** | 진남 × 금 | `a 65-year-old Korean Queen Dowager, regal and icy, large formal court wig (eoyeomeori) with gold ornaments, deep navy Korean dangui ceremonial jacket — a short Korean jacket with long curved front and back panels — with gold-leaf phoenix pattern over a full navy chima, carved green jade dragon ring` / 손 클로즈업만: `elderly royal hand with a carved green jade dragon ring, navy Korean dangui sleeve with white inner cuff and gold-leaf border` |
| **@SHAMAN** | 오방색 | `an ageless Korean female shaman (mudang), long white hair, Korean shaman's hanbok with layered garments in the five Korean obangsaek colors (blue, red, yellow, white, black), brass bells in hand, piercing kind eyes` |
| **@YOUNG_SEOYEON** / **@YOUNG_HWAN** | | `8-year-old Korean girl in a short Korean saekdong jeogori with rainbow-striped sleeves and a pink chima, one braid with a red daenggi` / `14-year-old Korean boy prince in a pale blue Korean durumagi coat and black Korean bokgeon cloth hat, tear-stained face` |

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
