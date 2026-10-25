# Flow 제작 패키지 — *The Bride Who Died Twice* EP.1

## 0. 사용법
1. **STEP A — 레퍼런스(Ingredients) 이미지부터 생성**: 아래 §1 프롬프트로 인물 5종 + 장소 5종 이미지를 만들고, Flow 프로젝트에 이름 그대로 저장(`@SEOYEON`, `@HWAN` …).
2. **STEP B — 컷 생성**: §3의 각 컷을 *Ingredients to Video*(옴니 레퍼런스)로 생성. 표기된 `@` 레퍼런스를 첨부하고 프롬프트를 붙여넣는다. 컷당 8초.
3. **STEP C — 연결 컷**: `→ EXTEND` 표시는 직전 컷의 마지막 프레임에서 *Extend / Frames to Video*로 이어 붙여 연속성 유지.
4. **STEP D — 편집**: Flow Scenebuilder에서 순서대로 배치, 0:24 타이틀 카드와 자막 삽입. 총 36컷 × 8초 ≈ 4분 48초 + 타이틀 ≈ **5분**.

**대사 언어**: 글로벌 타깃이므로 프롬프트 내 대사는 영어. 한국어 버전은 각 컷의 `KR` 대사로 더빙/자막 처리.
**화면비**: 롱폼 5분 → 16:9 권장 (쇼츠 재가공 시 9:16 리프레임).

### 공통 스타일 접미사 (모든 컷 끝에 붙임) `[STYLE]`
```
Cinematic Joseon-dynasty Korean period drama, shot on 35mm anamorphic lens, shallow depth of field, soft volumetric light, historically accurate hanbok silk textures, color palette of jade green, deep crimson, antique gold and ink black, subtle film grain, elegant slow camera movement, 4K, no text, no subtitles, no watermark.
```

### 공통 네거티브 `[NEG]`
```
Chinese or Japanese costume, kimono, modern objects, Western faces, distorted hands, extra fingers, text, logo, cartoon style
```

---

## 1. 레퍼런스(Ingredients) 이미지 프롬프트

### 인물
**@SEOYEON** — 
```
Character reference sheet, front view and three-quarter view, a 19-year-old Korean noblewoman of the Joseon dynasty, delicate oval face, clear dark-brown eyes, calm intelligent gaze, black hair in a low chignon held by a single plain silver binyeo hairpin, wearing a pale jade-green jeogori with a deep indigo chima skirt, neutral grey background, soft studio light, photorealistic.
```
변형 저장: `@SEOYEON_WHITE` (흰 저고리 + 진홍 치마), `@SEOYEON_BRIDE` (녹원삼 + 금박 화관, 연지곤지)

**@HWAN** —
```
Character reference sheet, front and three-quarter view, a 24-year-old Korean crown prince of the Joseon dynasty, sharp jawline, deep cold eyes, composed expressionless face, wearing a crimson gonryongpo royal robe with golden dragon roundels on chest and shoulders, black ikseongwan winged cap, jade belt, neutral grey background, photorealistic.
```
변형 저장: `@HWAN_MASK` (검은 도포 + 흑립 + 눈가를 가린 검은 반가면)

**@HWARYEONG** —
```
Character reference sheet, a 21-year-old Korean noblewoman of the Joseon dynasty, round soft face, sweet innocent smile that does not reach her eyes, ornate gold tteoljam hairpins, peach-pink jeogori with a pale green chima, a small red knotted silk perfume pouch (hyangnang) tied at her sleeve, neutral grey background, photorealistic.
```

**@LADYMIN** —
```
Character reference sheet, a 45-year-old Korean noble matriarch of the Joseon dynasty, cold narrow eyes, thin lips, hair in a formal chignon with a gold binyeo, deep purple dangui ceremonial jacket, jade ring, neutral grey background, photorealistic.
```

**@DOWAGER_HAND** —
```
Close-up reference of an elderly royal woman's wrinkled hand, wearing a large carved jade ring with a dragon motif, gold-embroidered crimson silk sleeve cuff, dark background, photorealistic.
```

### 장소
| 이름 | 프롬프트 |
|---|---|
| **@LOC_BRIDAL** | `Joseon royal bridal chamber at night, red silk bedding, folding screen painted with peonies, many tall red candles, paper doors, wooden lattice, warm flickering light` |
| **@LOC_HOUSE** | `Joseon noble family hanok courtyard at dawn, a blooming white plum tree, stone steps, tiled roofs, morning mist` |
| **@LOC_PLUMGARDEN** | `Plum blossom garden at night, hundreds of paper lanterns hanging from branches, falling petals, moonlight, stone path` |
| **@LOC_TEAHALL** | `Grand Joseon palace hall for a royal tea ceremony, red lacquered pillars, dancheong painted beams, low tea tables, rows of court ladies, golden afternoon light through paper windows` |
| **@LOC_PAVILION** | `Royal pavilion over a lotus pond at night, full moon reflected on water, lanterns, dancheong eaves` |
| **@LOC_PRISON** | `Dark Joseon royal prison cell, wooden bars, straw floor, single torch, cold blue moonlight` |

---

## 2. 타임라인 요약
| 구간 | 컷 | 내용 |
|---|---|---|
| 0:00–0:24 | 01–03 | 콜드 오픈: 혼례 밤 독살 |
| 0:24–0:30 | 타이틀 | **THE BRIDE WHO DIED TWICE / 두 번 죽은 세자빈** |
| 0:30–0:54 | 04–06 | 회귀 각성 |
| 0:54–1:42 | 07–12 | 화령의 위선, 향낭 독약 탈취 |
| 1:42–2:30 | 13–18 | 매화원 가면 사내 |
| 2:30–3:42 | 19–27 | 간택 다례 공개 처단 |
| 3:42–4:30 | 28–33 | 이중 회귀 고백 |
| 4:30–5:00 | 34–36 | 흑막 클리프행어 |

---

## 3. 컷별 Flow 프롬프트
> 형식: **[컷] 시간 | 숏 | 레퍼런스** → 프롬프트 → 대사(EN / KR) → 사운드

### ACT 0 — 죽음 (콜드 오픈)

**01** 0:00 | ECU → 풀샷 | @SEOYEON_BRIDE @HWARYEONG @LOC_BRIDAL
```
Extreme close-up of a porcelain teacup trembling in a bride's hand, the tea ripples, then the cup falls and shatters on the wooden floor in slow motion. Camera pulls back to reveal the young bride in a green wonsam and gold flower crown collapsing onto red silk, candlelight flickering. Her elder stepsister stands above her, smiling softly. [STYLE]
```
- EN (Hwa-ryeong, whisper): "Sleep well, Your Highness."
- KR: "편히 잠드세요, 세자빈 마마."
- SFX: 도자기 깨지는 소리 → 심장 박동

**02** 0:08 | CU | @SEOYEON_BRIDE @HWARYEONG
```
Close-up of the dying bride lying on red silk, a thin line of blood at the corner of her lips, tears in her eyes, looking up in betrayal. The stepsister leans down and gently removes the silver hairpin from the bride's hair, admiring it. Candle flames bend as a cold wind enters. [STYLE]
```
- EN (Hwa-ryeong): "This place was always meant to be mine."
- KR: "이 자리는 원래 내 것이었어."

**03** 0:16 | 탑뷰 → ECU 눈 | @SEOYEON_BRIDE @LOC_BRIDAL
```
Top-down shot of the bride lying motionless, white plum petals drifting down from nowhere and landing on her face. Slow push in to an extreme close-up of her eye as the light fades, the reflection of a candle going out. [STYLE]
```
- EN (Seo-yeon, VO, breaking): "Heaven… if you give me one more day… I will never kneel again."
- KR: "하늘이시여… 단 하루만 더 주신다면… 다시는 무릎 꿇지 않겠습니다."
- SFX: 촛불 꺼짐 → 무음 → **타이틀 카드 (0:24–0:30)**

### ACT 1 — 회귀

**04** 0:30 | CU | @SEOYEON @LOC_HOUSE
```
A young Korean noblewoman gasps awake on a simple floor mattress in a sunlit hanok room at dawn, sitting up abruptly, hand on her throat, breathing hard. Soft morning light through paper doors. [STYLE]
```
- SFX: 거친 숨 → 새소리

**05** 0:38 | MCU | @SEOYEON
```
The young woman looks down at her own hands in disbelief, then touches her hair and finds the single silver hairpin still there. Her expression shifts from shock to quiet, cold determination. [STYLE]
```
- EN (VO): "Three days before the wedding. I'm alive."
- KR: "혼례 사흘 전… 살아 있어."

**06** 0:46 | 와이드 | @SEOYEON @LOC_HOUSE → EXTEND 없음
```
She slides open the paper door. In the courtyard a white plum tree is in full bloom, petals falling in slow motion, morning mist. She steps out barefoot onto the wooden porch, framed by the door, her back to camera. [STYLE]
```
- 음악: 가야금 테마 시작

### ACT 2 — 복수의 설계

**07** 0:54 | 투샷 | @SEOYEON @HWARYEONG @LOC_HOUSE
```
In the courtyard under the plum tree, the sweet-faced stepsister in peach-pink hanbok hurries toward the young woman with an exaggerated warm smile and takes her hands affectionately. [STYLE]
```
- EN (Hwa-ryeong): "Little sister! You look pale — were you dreaming again?"
- KR: "동생! 얼굴이 창백하네, 또 악몽 꿨니?"

**08** 1:02 | CU (서연) | @SEOYEON
```
Close-up of the young woman smiling back gently, but her eyes are ice-cold and calculating. Shallow focus, the stepsister blurred in the foreground. [STYLE]
```
- EN: "A very long dream, sister. It ended with you."
- KR: "아주 긴 꿈이었어요, 언니. 끝에 언니가 있었죠."

**09** 1:10 | ECU 인서트 | @HWARYEONG
```
Extreme close-up of a small red knotted silk perfume pouch tied to the stepsister's sleeve, a corner of folded white paper peeking out of it. Slow rack focus. [STYLE]
```
- SFX: 낮은 현악 긴장음

**10** 1:18 | MS | @SEOYEON @HWARYEONG @LADYMIN
```
The cold stepmother in a deep purple dangui appears on the porch. The stepsister turns away to bow to her. In that moment, the young woman's fingers slip into the red silk pouch with a quick, graceful movement and palm the folded paper packet. [STYLE]
```
- EN (Lady Min): "Hwa-ryeong. The palace has summoned both of you for the final selection."
- KR: "화령아. 궁에서 너희 둘을 최종 간택에 부르셨다."

**11** 1:26 | CU (서연, 홀로) | @SEOYEON
```
Alone behind a folding screen, the young woman unfolds the small paper packet; fine grey powder inside. She smells it and her eyes harden. She folds it into her own sleeve. [STYLE]
```
- EN (VO): "Wolfsbane. The same bitter scent as that night."
- KR (VO): "부자. 그날 밤과 같은 쓴 향."

**12** 1:34 | MCU | @SEOYEON_WHITE
```
Transformation beat: the young woman stands before a bronze mirror now dressed in a pure white jeogori and a deep crimson chima, sliding the single silver hairpin firmly into her chignon. Candlelight, determined gaze into the mirror. [STYLE]
```
- EN: "This time, the poison will find its owner."
- KR: "이번엔 독이 주인을 찾아갈 거야."

### ACT 2-b — 매화원의 가면 사내

**13** 1:42 | 와이드 | @SEOYEON_WHITE @LOC_PLUMGARDEN
```
Night. The young woman in white and crimson walks alone along a stone path through a plum blossom garden hung with hundreds of glowing paper lanterns, petals drifting in the moonlight. [STYLE]
```

**14** 1:50 | MS | @SEOYEON_WHITE @HWAN_MASK
```
A tall man in a black dopo robe, black gat hat and a black half-mask steps out from behind a blossoming tree, blocking her path. She stops, unafraid, her hand moving to her silver hairpin. [STYLE]
```
- EN (Hwan): "A noble lady walking alone at night. Either brave… or hunting."
- KR: "밤에 홀로 걷는 규수라. 용감하거나… 사냥 중이거나."

**15** 1:58 | 오버숄더 | @SEOYEON_WHITE @HWAN_MASK
```
Over-the-shoulder shot of the masked man; the young woman lifts her chin defiantly, lantern light on her face, petals falling between them. [STYLE]
```
- EN (Seo-yeon): "Then step aside, sir, before you become the prey."
- KR: "그럼 비키시지요. 사냥감이 되기 전에."

**16** 2:06 | CU (가면) | @HWAN_MASK
```
Close-up of the masked man; a faint smile at the corner of his lips. He holds out a small cup of tea he was carrying, steam rising. [STYLE]
```
- EN: "Chrysanthemum tea. For the cold."
- KR: "국화차요. 밤이 차니."

**17** 2:14 | ECU (서연) | @SEOYEON_WHITE
```
Extreme close-up of the young woman freezing, eyes widening in shock, a single tear catching the lantern light. [STYLE]
```
- EN (VO): "Only one person ever knew I hate chrysanthemum… and he held me as I died."
- KR (VO): "내가 국화차를 싫어하는 걸 아는 건… 내가 죽을 때 날 안고 있던 그 사람뿐인데."

**18** 2:22 | 와이드 | @HWAN_MASK @LOC_PLUMGARDEN
```
She looks up but the masked man has vanished; only the steaming teacup remains on a stone lantern, plum petals swirling where he stood. [STYLE]
```
- SFX: 바람 → 북소리 전환

### ACT 3 — 간택 다례 (공개 처단)

**19** 2:30 | 설정 와이드 | @LOC_TEAHALL
```
Grand establishing shot of the palace tea ceremony hall, rows of court ladies kneeling, red pillars, dancheong beams, golden afternoon light; at the far end an empty royal seat behind a sheer silk screen. Slow crane down. [STYLE]
```
- SFX: 궁중 정악, 편종

**20** 2:38 | MS | @HWARYEONG @SEOYEON_WHITE @LOC_TEAHALL
```
The stepsister kneels gracefully before the young woman and pours tea from a celadon pot into a celadon cup, offering it with both hands and a sweet smile, court ladies watching. [STYLE]
```
- EN (Hwa-ryeong): "Sister, the first cup must be yours. For luck."
- KR: "동생, 첫 잔은 네가 들어야지. 복을 빌며."

**21** 2:46 | ECU 인서트 | @SEOYEON_WHITE
```
Extreme close-up: the young woman slowly draws the silver hairpin from her hair and dips its tip into the tea. The silver blackens instantly, a dark stain creeping up the metal. [STYLE]
```
- SFX: 쨍 — 정적

**22** 2:54 | 와이드 리액션 | @LOC_TEAHALL
```
The whole hall gasps; court ladies recoil, teacups rattle, a lady-in-waiting drops a tray. Camera whips to the stepsister, whose smile collapses. [STYLE]
```
- EN (court lady): "Poison!"
- KR: "독이다!"

**23** 3:02 | MCU | @HWARYEONG @LADYMIN
```
The stepsister points a trembling finger, faking tears, while the stepmother rises behind her with a cold, commanding face. [STYLE]
```
- EN (Hwa-ryeong): "She did it! She poisoned her own cup to frame me!"
- EN (Lady Min): "Seize that wicked girl!"
- KR: "쟤가 한 거예요! 저를 모함하려고!" / "저 요망한 것을 끌어내라!"

**24** 3:10 | CU | @SEOYEON_WHITE
```
The young woman, perfectly calm, takes a folded paper packet from her sleeve and holds it up; the red silk thread of the stepsister's pouch is still wrapped around it, embroidered with the character of her name. [STYLE]
```
- EN: "Then tell me, sister, why your perfume pouch carries wolfsbane?"
- KR: "그럼 언니, 언니 향낭에서 왜 부자가 나왔을까요?"

**25** 3:18 | ECU | @HWARYEONG
```
Extreme close-up of the stepsister's face draining of color, lips trembling, her hand instinctively grabbing at her now-empty sleeve pouch. [STYLE]
```

**26** 3:26 | 와이드 → 로우앵글 | @HWAN @LOC_TEAHALL
```
The silk screen is pulled aside. The crown prince in crimson dragon robe and winged cap rises from the royal seat; the entire hall bows to the floor. Low-angle shot, majestic and cold. [STYLE]
```
- EN (Hwan): "Enough. Arrest them both."
- KR: "그만. 둘 다 포박하라."

**27** 3:34 | MS | @HWARYEONG @LADYMIN
```
Royal guards in dark uniforms seize the screaming stepsister and the stunned stepmother, dragging them out across the polished floor; a gold hairpin falls and clatters. [STYLE]
```
- EN (Hwa-ryeong, screaming): "Your Highness! Your Highness, it's a lie!"
- KR: "저하! 저하, 모함이옵니다!"

### ACT 4 — 이중 회귀 반전

**28** 3:42 | 와이드 | @SEOYEON_WHITE @HWAN @LOC_PAVILION
```
Night. A royal pavilion over a lotus pond, full moon reflected in the water. The young woman stands at the railing; the crown prince walks up behind her slowly. [STYLE]
```

**29** 3:50 | 투샷 | @SEOYEON_WHITE @HWAN
```
She turns to face him and bows slightly, then lifts her eyes directly to his, searching. Moonlight between them. [STYLE]
```
- EN (Seo-yeon): "The chrysanthemum tea. How did you know?"
- KR: "국화차… 어떻게 아셨습니까?"

**30** 3:58 | CU (이환) | @HWAN
```
Close-up of the crown prince; his cold mask finally breaks, eyes glistening with restrained grief. [STYLE]
```
- EN: "Because last time, I arrived one breath too late. I held you while your hands went cold."
- KR: "지난번엔 한 호흡 늦었소. 식어가는 그대 손을 내가 잡고 있었지."

**31** 4:06 | ECU (서연) | @SEOYEON_WHITE
```
Extreme close-up of the young woman's face as realization hits, a tear running down her cheek, lantern light flickering. [STYLE]
```
- EN (whisper): "You… came back too."
- KR: "저하도… 돌아오셨군요."

**32** 4:14 | MS | @SEOYEON_WHITE @HWAN
```
The crown prince gently takes her hand and places the silver hairpin back into her palm, closing her fingers around it. Plum petals drift onto the surface of the lotus pond. [STYLE]
```
- EN: "This time, I will not be late."
- KR: "이번엔 늦지 않겠소."

**33** 4:22 | 와이드 실루엣 | @LOC_PAVILION
```
Wide silhouette shot of the two figures standing close in the pavilion against the enormous full moon, reflected perfectly in the still pond. Slow pull back. [STYLE]
```
- 음악: 러브 테마 정점

### ACT 5 — 클리프행어

**34** 4:30 | MS | @HWARYEONG @LOC_PRISON
```
A dark prison cell; the stepsister, hair undone, sits in the straw sobbing. Footsteps; she looks up toward the bars, hope on her face. [STYLE]
```

**35** 4:38 | ECU 손 | @DOWAGER_HAND @LOC_PRISON
```
Extreme close-up of an elderly royal hand with a carved dragon jade ring and gold-embroidered crimson sleeve reaching through the wooden bars, pressing a new paper packet of poison into the stepsister's palm. Torchlight. [STYLE]
```
- EN (Dowager, unseen, cold whisper): "Finish it. The bride must still die."
- KR: "끝내거라. 세자빈은 그래도 죽어야 한다."

**36** 4:46 | ECU → 블랙 | @SEOYEON_WHITE
```
Back in the pavilion, the young woman suddenly feels a chill and looks up; a single white plum petal falls onto her palm and slowly turns black from the edges inward. Smash cut to black. [STYLE]
```
- SFX: 심장 박동 1회 → 무음
- 텍스트 카드 (편집에서 삽입): **"EPISODE 2 — The Jade Ring"**

---

## 4. 일관성 체크리스트
- [ ] 모든 컷에 해당 `@인물` 레퍼런스를 반드시 첨부 (텍스트 묘사만으로는 얼굴이 흔들림)
- [ ] 서연의 **은비녀**는 컷 02(빼앗김)·21(꺼냄)·32(돌려받음)에서만 위치 변화 — 소품 연속성 핵심
- [ ] 의상 전환: 01–03 혼례복 → 04–11 옥색 → 12 이후 흰/진홍
- [ ] 화령의 **붉은 향낭**: 07·09·10에 보이고 24 이후 비어 있음
- [ ] 대사가 길면(8초 초과) 컷을 둘로 나누거나 VO로 후반 녹음
- [ ] 각 컷 3–4개 생성 후 베스트 테이크 선택, 손·얼굴 왜곡 컷 폐기

## 5. 글로벌 배포 팁
- 썸네일: 컷 21(검게 변하는 은비녀) 또는 컷 01(독차 잔)
- 제목 A/B: *The Bride Who Died Twice* / *Reborn to Destroy My Stepsister* / *The Cold Prince Remembers Me*
- 자막: EN 하드섭 + KR/ES/PT/ID 자막 파일 (숏드라마 주요 시장)
