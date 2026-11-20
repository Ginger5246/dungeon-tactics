# 地城戰棋 立繪 v3（武士 A 畫風）

畫家產線輸出。遊戲檔路徑維持原欄位 id（**不要改檔名**）：

- 原英雄欄：`assets/heroes_v3/<id>.webp`
- 原敵人欄：`assets/enemies_v3/<id>.webp`

本輪起全數為**同一角色池**，不再分英雄／敵人陣營。本輪**沒有編輯** `index.html`（顯示名稱請開發者自行改）。

預覽圖：`shots/v3_preview_<id>.png`（1024×1536 PNG）。聯絡表：`shots/art_v3_sheet.jpg`（統一編號 No.001–027，無英雄／敵人分區）。

風格已由使用者於 2026-11-20 認可：`heroes_v3/samurai.webp`（version A），紀錄在 `assets/ART_V3_APPROVED.txt`。

## 給開發者：欄位身分變更

- **全體為同一角色池。** 檔案仍放在 `heroes_v3/` 與 `enemies_v3/`，只是為了對上現有 id，不是陣營分類。
- **`samurai` 欄是紅髮雙匕首騎士**（已認可；不是 v2 黑短髮拔刀少年）。
- 使用者要求人類角色約減半、改以神話／鬼怪替代。原約 12 名人類保留 6 名，另 6 欄**改種但保留同一檔名**：

| 檔名 id（勿改） | 舊人類（備份預覽） | 現在 |
| --- | --- | --- |
| `ninja` | 足輕忍者 | **轆轤首**（長頸女妖，潛行刺客） |
| `naginata` | 薙刀武女 | **雷神**（鼓圈雷神，攻擊手） |
| `sohei` | 僧兵 | **牛鬼**（牛頭蜘蛛身，坦克） |
| `ronin` | 浪人劍客 | **鵺**（猿面、狸身、虎肢、蛇尾，近戰） |
| `onmyoji` | 陰陽見習 | **座敷童子**（小屋童子，輔助／幸運） |
| `kagenin` | 影之忍 | **夜叉**（雙刀鬼武者，SSR） |

舊人類全身預覽保留在 `shots/v3_preview_<id>_human_old.png`，遊戲檔已被新稿覆寫。

- 保留的 6 名人類／人型：`samurai`（放逐騎士）、`kyudo`（弓道少女）、`miko`（巫女）、`grandonmyoji`（大陰陽師）、`kagura`（神樂櫻巫女）、`ryujin`（龍神武者）。
- **`goblin`（河童）** 仍是盲龜長老衍生（波浪披肩、荷花青玉杖、殼上樹蛙），不是 v2 黃瓜河童。
- **`orochi`（八岐大蛇）** 仍是端莊蛇女王衍生（高領黑金長袍、八顆黑金蛇頭），覆蓋 v2 非人形八頭蛇。
- **ref3 覆盆子、ref5 蘑菇催眠大師** 仍未入列。這次 6 個替代欄已指定妖怪，**沒有改用蘑菇妖**。若之後要加新欄再畫。

## 規格與產線

- 風格：2010s 日系手機卡牌手繪風；清晰墨線、變化線寬、賽璐璐上色。避免塑料光澤、過度閃粉、融化細節。
- 構圖：直向 2:3 全身，暖金奶油天空、連續菱格舞台（由上延伸天空補成 2:3，不另外補地板）。
- 預覽：1024×1536 PNG（Lanczos + UnsharpMask r0.8 / 70%）。
- 遊戲檔：768×1152 WebP quality 85、method 6，皆 < 200KB。原子寫入。
- 生成：`GenerateImage` 3:4，風格參考一律為認可的 samurai A；goblin／orochi 另加過對應 ref 裁切。waifu2x-ncnn-vulkan（models-cunet, noise 0, scale 2, lavapipe）後補天。
- 硬條件：無文字／浮水印／UI；手與武器／肢體正確；臉要能彼此分辨；服裝端莊。
- **不要覆寫**已認可的 `heroes_v3/samurai.webp`。

## 統一編號 No.001–027

聯絡表與下表順序相同。路徑仍依原資料夾。

| No. | id | 名稱 | 路徑 | 備註 |
| ---: | --- | --- | --- | --- |
| 001 | samurai | 放逐騎士 | heroes_v3 | 已認可；紅髮雙匕首 |
| 002 | kyudo | 弓道少女 | heroes_v3 | 保留人類 |
| 003 | onmyoji | 座敷童子 | heroes_v3 | 原陰陽見習 |
| 004 | ninja | 轆轤首 | heroes_v3 | 原足輕忍者 |
| 005 | naginata | 雷神 | heroes_v3 | 原薙刀武女 |
| 006 | sohei | 牛鬼 | heroes_v3 | 原僧兵 |
| 007 | tengu | 天狗射手 | heroes_v3 | |
| 008 | miko | 巫女 | heroes_v3 | 保留人類 |
| 009 | kitsune | 狐火術士 | heroes_v3 | |
| 010 | ronin | 鵺 | heroes_v3 | 原浪人劍客 |
| 011 | yukionna | 雪女 | heroes_v3 | |
| 012 | ryujin | 龍神武者 | heroes_v3 | 保留（人型龍神） |
| 013 | grandonmyoji | 大陰陽師 | heroes_v3 | 保留人類 |
| 014 | kagenin | 夜叉 | heroes_v3 | 原影之忍 |
| 015 | okami | 白狼神使 | heroes_v3 | |
| 016 | kagura | 神樂櫻巫女 | heroes_v3 | 保留人類 |
| 017 | slime | 提燈小僧 | enemies_v3 | |
| 018 | goblin | 河童 | enemies_v3 | 盲龜長老衍生 |
| 019 | skel | 亡靈弓手 | enemies_v3 | |
| 020 | bat | 鎌鼬 | enemies_v3 | 檔名仍是 bat |
| 021 | brute | 赤鬼 | enemies_v3 | |
| 022 | onibi | 鬼火 | enemies_v3 | |
| 023 | tanuki | 化け狸 | enemies_v3 | |
| 024 | orochi | 八岐大蛇 | enemies_v3 | 蛇女王衍生 |
| 025 | gashadokuro | 餓者髏 | enemies_v3 | |
| 026 | shuten | 酒吞童子 | enemies_v3 | |
| 027 | kyubi | 九尾妖狐 | enemies_v3 | |

`ward` 沿用 brute 圖，沒有單獨 v3 檔。

---

## 角色設定（現行稿）

### No.001 samurai — 放逐騎士（已認可）
- 檔案：`assets/heroes_v3/samurai.webp`（97,230 bytes）
- 設定：紅長髮女騎士，合領白襯衫、深藍短褲、紅內襯短斗篷、雙手短劍／匕首。**不是** v2 黑髮拔刀武士。
- 備註：使用者 2026-11-20 認可 version A。舊像素修圖：`shots/v3_preview_samurai_edit_old.png`；備選 D2：`shots/v3_preview_samurai_alt.png`。

### No.002 kyudo — 弓道少女
- 檔案：`assets/heroes_v3/kyudo.webp`（82,214 bytes）
- 設定：黑高馬尾、淡藍髮帶，白／淺藍弓道服＋藏青袴，持長弓。

### No.003 onmyoji — 座敷童子
- 檔案：`assets/heroes_v3/onmyoji.webp`（66,944 bytes）
- 設定：約七歲小屋童子，深棕齊瀏海短髮，端莊淡薄荷綠與米色小和服，手持手毬，腰間松梅紋福袋（無文字）。輔助／幸運。
- 舊人類（陰陽見習）：`shots/v3_preview_onmyoji_human_old.png`。

### No.004 ninja — 轆轤首
- 檔案：`assets/heroes_v3/ninja.webp`（55,998 bytes）
- 設定：深紫黑髮髻、金琥珀瞳的女妖怪，頸項明顯拉長並呈 S 彎，端莊靛藍和服，持苦無，潛行刺客姿態。
- 舊人類（足輕忍者）：`shots/v3_preview_ninja_human_old.png`。

### No.005 naginata — 雷神
- 檔案：`assets/heroes_v3/naginata.webp`（179,670 bytes）
- 設定：藍髮雷神，深藍金雲紋武服（有袖有褲，不是只圍腰布），身後太鼓圈與巴紋鼓面、閃電，雙手持鼓槌，攻擊手。與赤鬼、酒吞明顯不同。
- 舊人類（薙刀武女）：`shots/v3_preview_naginata_human_old.png`。

### No.006 sohei — 牛鬼
- 檔案：`assets/heroes_v3/sohei.webp`（108,924 bytes）
- 設定：牛頭、紅瞳、灰黑肌，蜘蛛腹與多隻節肢，持鐵金棒，坦克站姿。
- 舊人類（僧兵）：`shots/v3_preview_sohei_human_old.png`。

### No.007 tengu — 天狗射手
- 檔案：`assets/heroes_v3/tengu.webp`（120,214 bytes）
- 設定：銀髮女射手，黑羽翼、赤天狗面具、山伏綠衣，持弓。靴款偏現代。

### No.008 miko — 巫女
- 檔案：`assets/heroes_v3/miko.webp`（71,128 bytes）
- 設定：黑長髮、較小紅緞帶，紅白巫女服、御幣；褐瞳、表情較靜，與弓道少女區隔。
- 備選：`shots/v3_preview_miko_alt.png`（臉較接近 kyudo，未採用）。

### No.009 kitsune — 狐火術士
- 檔案：`assets/heroes_v3/kitsune.webp`（132,302 bytes）
- 設定：橘紅髮、狐耳單尾、琥珀瞳，橙白火紋和服＋藍帶，藍色狐火。
- 備選：`shots/v3_preview_kitsune_alt.png`（開衩偏高，未採用）。

### No.010 ronin — 鵺
- 檔案：`assets/heroes_v3/ronin.webp`（102,686 bytes）
- 設定：日本獼猴面、奶油色圓腹（狸身意味）、虎紋四肢、一條綠蛇尾（尾端蛇頭），近戰撲擊。雙臂雙腿，無多餘肢體。
- 舊人類（浪人劍客）：`shots/v3_preview_ronin_human_old.png`。

### No.011 yukionna — 雪女
- 檔案：`assets/heroes_v3/yukionna.webp`（119,778 bytes）
- 設定：銀白長髮、冰藍瞳，端莊淡藍雪紋和服至踝，冰晶杖。

### No.012 ryujin — 龍神武者
- 檔案：`assets/heroes_v3/ryujin.webp`（156,874 bytes）
- 設定：暗紅長髮男性，金色龍角，金藍龍鱗甲與青披風，背後青龍魂。

### No.013 grandonmyoji — 大陰陽師
- 檔案：`assets/heroes_v3/grandonmyoji.webp`（145,410 bytes）
- 設定：銀白長髮成年男性，深藍金星辰袍，背後巨大金月牙與浮空符咒（抽象印文）。

### No.014 kagenin — 夜叉
- 檔案：`assets/heroes_v3/kagenin.webp`（123,286 bytes）
- 設定：青綠色皮膚的夜叉武者，紫髮、雙角、尖耳、獠牙與金紋，紅金甲，雙彎刀（只兩臂兩刀）。SSR 鬼武者，不是人類忍者，也與赤鬼、酒吞不同。
- 舊人類（影之忍）：`shots/v3_preview_kagenin_human_old.png`。

### No.015 okami — 白狼神使
- 檔案：`assets/heroes_v3/okami.webp`（114,630 bytes）
- 設定：銀白長髮、狼耳金瞳、白金社殿甲與長袴，紅注連繩，白金太刀。
- 備選：`shots/v3_preview_okami_alt.png`（短裙露腿，未採用）。

### No.016 kagura — 神樂櫻巫女
- 檔案：`assets/heroes_v3/kagura.webp`（148,592 bytes）
- 設定：粉長髮、金櫻花簪、粉白神樂裝、持鈴，與紅白巫女區隔。

### No.017 slime — 提燈小僧
- 檔案：`assets/enemies_v3/slime.webp`（75,122 bytes）
- 設定：橙色紙燈籠頭的小孩妖怪。不是史萊姆。

### No.018 goblin — 河童（盲龜長老衍生）
- 檔案：`assets/enemies_v3/goblin.webp`（116,040 bytes）
- 設定：綠龜長老，波浪披肩，荷花座青玉杖，殼上金綠樹蛙。
- 備選：`shots/v3_preview_goblin_alt.png`。眼神偏睜開，不像原圖那麼「盲／細眼」。

### No.019 skel — 亡靈弓手
- 檔案：`assets/enemies_v3/skel.webp`（127,340 bytes）
- 設定：骷髏弓手，藍色魂火，殘破藍鐵甲。

### No.020 bat — 鎌鼬
- 檔案：`assets/enemies_v3/bat.webp`（79,142 bytes）
- 設定：白色直立鼬鼠風妖，鐮刀前肢。**不是蝙蝠**（id 仍為 `bat`）。

### No.021 brute — 赤鬼
- 檔案：`assets/enemies_v3/brute.webp`（122,556 bytes）
- 設定：紅膚雙角鬼，虎皮腰衣，鐵金棒。

### No.022 onibi — 鬼火
- 檔案：`assets/enemies_v3/onibi.webp`（106,506 bytes）
- 設定：藍白火焰人形，周圍青色鬼火球。

### No.023 tanuki — 化け狸
- 檔案：`assets/enemies_v3/tanuki.webp`（104,300 bytes）
- 設定：雙足狸，笠帽、葫蘆、大葉。

### No.024 orochi — 八岐大蛇（蛇女王衍生）
- 檔案：`assets/enemies_v3/orochi.webp`（161,654 bytes）
- 設定：白金長髮小角，高領黑金蛇紋長袍，八顆黑鱗金腹蛇頭。
- 備選：`shots/v3_preview_orochi_alt.png`（六頭，未採用）。

### No.025 gashadokuro — 餓者髏
- 檔案：`assets/enemies_v3/gashadokuro.webp`（143,452 bytes）
- 設定：巨顱骷髏，骨冠，紫色魂火，破爛紫袍。

### No.026 shuten — 酒吞童子
- 檔案：`assets/enemies_v3/shuten.webp`（141,552 bytes）
- 設定：紫長髮鬼王，金酒盞，紅金甲與金棒。

### No.027 kyubi — 九尾妖狐
- 檔案：`assets/enemies_v3/kyubi.webp`（107,914 bytes）
- 設定：白銀長髮、白狐耳、紫瞳，紫白端莊袴，紫狐火，多條白紫尾。
- 備選：`shots/v3_preview_kyubi_alt.png`（尾數較少）。尾扇細數時可能看成 8 或 9 條。

## 疑點總表

1. **轆轤首（ninja）** 長頸呈清楚 S 彎，但沒有極端盤繞到頭遠離身體很遠。
2. **雷神（naginata）** 鼓圈可見約 5 面鼓（不是 6–8 面），造形仍完整。
3. **牛鬼（sohei）** 蜘蛛足應為 8 隻，因透視有一兩隻較短，目測大致是 8，但不是每一隻都同等清楚。
4. **鵺（ronin）** 獼猴面、虎肢、單條蛇尾都清楚；軀幹是圓潤奶油腹，狸的「體態」有了，但不是花紋很重的狸背。
5. **座敷童子、夜叉** 各有棄用稿（福字袋；四臂四刀），定稿已避開。
6. **goblin** 眼神仍偏睜開。**kyubi** 尾數仍可能看成 8 或 9。
7. **2:3 補天** 做法與已認可的 samurai A 相同；部分圖頂端可能有極淡交界。
8. `bat`／`slime` 檔名未改，畫面是鎌鼬、提燈小僧。
9. **ref5 蘑菇未使用**；6 個替代欄皆依指定妖怪。
