# 📖 0ai.vn Models Cheatsheet — 1 Trang Chọn Đúng Model

> **Bản 2.0** — Cập nhật ngày 15/05/2026 (sau 4 tuần 28 ngày)
> **Tác giả:** [Linh0AI](https://facebook.com/daclinh.tran)
> **Data dựa trên test thực tế** — không phải copy info marketing từ web

---

## 🎯 Cheatsheet này dành cho ai?

- ✅ Bạn dùng **0ai.vn** và phân vân không biết chọn model nào
- ✅ Bạn muốn **tiết kiệm credit** mà vẫn có ảnh/video chất lượng
- ✅ Bạn cần **quick reference** khi đang work — không có thời gian đọc tutorial dài
- ✅ Bạn từ Việt Nam và muốn biết model nào hiểu prompt Việt tốt nhất

> **⚠️ Lưu ý:** Cheatsheet này cover **3 model image flagship** (Seedream 4.5, NBN2, GPT Image 2) + **1 model video flagship** (Seedance Omni 2.0). Các model khác trên 0ai.vn (NBN Pro, Z-Image, Kling, VEO 3.1...) sẽ được thêm vào bản v3.0 sau khi mình test thật.

---

## 🥇 Bảng so sánh tổng — Image models (xem 30 giây là đủ)

| Tiêu chí | 🟦 Seedream 4.5 | 🟨 NBN2 | 🟪 GPT Image 2 |
| --- | --- | --- | --- |
| 💰 **Giá min/ảnh** | **350 credit** 🥇 | 400 credit 🥈 | 900 credit 🥉 |
| ⚡ **Tốc độ generate** | Trung bình | Nhanh | **Nhanh nhất** 🥇 |
| 🏆 **Chất lượng tổng thể** | Tốt (specific) | Tốt (đa dụng) | **Tốt nhất** 🥇 |
| 📐 **Native resolution** | 2048×2048 | 2K | ~2K |
| 📏 **Aspect ratio 21:9** | ✅ Native | ⚠️ Yếu | ✅ Hỗ trợ |
| 🌐 **Ngôn ngữ tốt nhất** | 🇨🇳 > Hybrid > 🇻🇳 | 🇻🇳 > Hybrid > 🇬🇧 | 🇬🇧 > Hybrid > 🇻🇳 |
| 🎭 **Character consistency** | **🥇** (14 ref ảnh) | 🥈 | 🥉 |
| ✍️ **Text trong ảnh** | **🥇** vô địch | 🥉 hay sai | 🥈 khá ổn |
| 🎨 **Photo realistic** | 🥈 | 🥉 | **🥇** |
| 🎨 **Anime / hoạt hình** | 🥉 | **🥇** | 🥈 |
| 👤 **Chân dung thời trang** | **🥇** | 🥈 | 🥉 |
| 🌄 **Phong cảnh Việt Nam** | 🥈 | **🥇** | 🥉 |
| 🛍️ **Sản phẩm thương mại** | **🥇** | 🥉 | 🥈 |
| 📋 **Storyboard 4×4 grid** | **🥇** (verified Day 18) | 🥈 | 🥉 |
| 🎬 **Character sheet cinematic** | **🥇** (Day 17 + Day 27 multi-age) | 🥈 | 🥈 |

---

## 🟦 Seedream 4.5 — "Nhà thiết kế thời trang"

**Nhà phát hành:** ByteDance (cha đẻ TikTok, CapCut)
**Ra mắt:** Tháng 12/2025 — đã ổn định production
**Giá min:** **350 credit/ảnh** (rẻ nhất nhóm flagship)

### ✅ Best for

- 📸 **Chân dung biểu cảm phong cách thời trang/glamour** — tone tạp chí Vogue/Elle
- 🛒 **Ảnh sản phẩm cao cấp** — chi tiết kim loại, kính, da, đá cẩm thạch
- 🎭 **Bộ ảnh nhân vật** — character consistency số 1 (upload 14 reference images)
- ✍️ **Ảnh có text tiếng Việt có dấu** — biển hiệu, logo, packaging label
- 🎬 **Cinematic 21:9** — concept art, poster phim, lookbook
- 💸 **Production volume cao** — rẻ nhất, scale được tốt
- 📋 **Storyboard 4×4 grid** (16 panels) — verified Day 18 short film pipeline
- 🎭 **Multi-age character sheet** — verified Day 27 (4 ages × 2 views work)

### ❌ Skip when

- Cần **tốc độ tuyệt đối** (livestream, demo) → GPT Image 2
- Phong cách **anime/hoạt hình/illustration** → NBN2
- Prompt **100% tiếng Việt thuần** không muốn dịch → NBN2
- Cần **"auto-pilot" reliability** không miss prompt → GPT Image 2

### 🔑 Prompt strategy

- **Hierarchy ngôn ngữ:** 🇨🇳 中文 > 🇻🇳🇬🇧 Hybrid VI+EN > 🇻🇳 Tiếng Việt thuần
- **Sweet spot độ dài:** 30-100 từ (ngắn hơn các model khác — đừng viết dài quá!)
- **Cấu trúc:** SUBJECT lên đầu → STYLE → COMPOSITION → LIGHTING
- **Magic words:** `natural skin with visible pores`, `cinematic lighting`, `editorial portrait`
- **Negative prompt cần có:** `plastic skin, smooth airbrushed face, oversaturated`

### 💰 Giá trị thực tế

**Gói Ultra Member 1.000.000đ (1.1 triệu credit) = 3,143 ảnh Seedream 4.5**

---

## 🟨 Nano Banana 2 (NBN2) — "Người Việt giỏi mọi nghề"

**Nhà phát hành:** Google (Gemini family)
**Giá min:** **400 credit/ảnh**

### ✅ Best for

- 🇻🇳 **Prompt 100% tiếng Việt** — model hiểu sâu ngôn ngữ Việt nhất
- 🎨 **Phong cách anime / hoạt hình / illustration / chibi**
- 🌄 **Phong cảnh Việt Nam** — ruộng bậc thang, áo dài, nón lá, phố cổ Hội An...
- 🎯 **Đa dụng** — không xuất sắc ở 1 thứ nhưng làm tốt ở mọi thứ
- 💸 **Tiết kiệm vừa phải** — đắt hơn Seedream 4.5 chút, rẻ hơn GPT 55%
- ⚡ **Nhanh** — tốc độ generate khá, gần với GPT Image 2

### ❌ Skip when

- Cần **text trong ảnh chuẩn** (NBN2 hay viết sai chữ) → Seedream 4.5
- Cần **character consistency** cho bộ ảnh → Seedream 4.5
- Cần **chất lượng "AI auto-pilot"** ổn định nhất → GPT Image 2
- Cần **ảnh sản phẩm cao cấp** với chi tiết kim loại/kính → Seedream 4.5

### 🔑 Prompt strategy

- **Hierarchy ngôn ngữ:** 🇻🇳 Tiếng Việt > 🇻🇳🇬🇧 Hybrid > 🇬🇧 Tiếng Anh thuần
- **Sweet spot độ dài:** 80-150 từ (linh hoạt hơn Seedream)
- **Magic words:** Tên cụ thể địa điểm Việt Nam (Hội An, Sapa, Phú Quốc...), tên truyền thống (áo dài, nón lá, đèn lồng...)
- **Negative prompt cần có:** `low quality, blurry, distorted, watermark`

### 💰 Giá trị thực tế

**Gói Ultra Member 1.000.000đ (1.1 triệu credit) = 2,750 ảnh NBN2**

---

## 🟪 GPT Image 2 — "Auto-pilot premium"

**Nhà phát hành:** OpenAI
**Giá min:** **900 credit/ảnh** (đắt nhất, gấp 2.57x Seedream)

### ✅ Best for

- 🏆 **Ảnh quan trọng** — khách hàng deadline gấp, thumbnail cần viral
- ⚡ **Cần tốc độ tuyệt đối** — model nhanh nhất trên 0ai.vn
- 🎯 **Chất lượng ổn định nhất** — ít miss prompt, ít artifact, ít "AI weirdness"
- 🌍 **Prompt tiếng Anh dài chi tiết** — model mạnh nhất với English
- 🎨 **Photo-realistic chuẩn** — face structure, perspective, lighting đều tốt
- 🎭 **Hooded figure / atmospheric still** — verified Day 27 (peaceful tone, no skull/scythe)

### ❌ Skip when

- **Test ý tưởng / draft / nháp** → Seedream 4.5 (rẻ 2.57x, đủ tốt)
- **Production volume cao** — sẽ cháy credit nhanh → Seedream 4.5
- **Prompt tiếng Việt thuần** không muốn dịch → NBN2
- **Phong cách anime/illustration** → NBN2
- **Cần character consistency với nhiều reference** → Seedream 4.5
- **Multi-age character sheet 4+ ages** → trigger filter #c455 "real person" (verified Day 27)

### 🔑 Prompt strategy

- **Hierarchy ngôn ngữ:** 🇬🇧 Tiếng Anh > 🇻🇳🇬🇧 Hybrid > 🇻🇳 Tiếng Việt thuần
- **Sweet spot độ dài:** 100-200 từ (cho phép prompt chi tiết hơn)
- **Magic words:** Mention specific camera/lens (`shot on Sony A7IV, 85mm f/1.4`), mood/atmosphere words
- **Negative prompt cần có:** Ít cần hơn 2 model trên — model tự filter tốt

### 💰 Giá trị thực tế

**Gói Ultra Member 1.000.000đ (1.1 triệu credit) = 1,222 ảnh GPT Image 2**

⚠️ **Chỉ bằng 39% so với Seedream 4.5** — cân nhắc trước khi dùng cho mọi ảnh.

---

## 🟧 Seedance Omni 2.0 — "Video AI flagship" 🎬

**Nhà phát hành:** ByteDance (cùng nhà với Seedream 4.5)
**Ra mắt:** Tháng 4/2026 — verified production-ready
**Giá min:** **~15,000-20,000 credit/segment** (cho 9:16 video 15s với refs)
**Duration cap:** **15 giây/segment** (verified Day 27 — không thể quá)

### ✅ Best for

- 🎬 **Text-to-video** clip ngắn 10-15s cho concept exploration
- 🎞️ **Image-to-video** animate ảnh tĩnh thành clip emotional
- 🎭 **Multi-reference video** (3 refs đồng thời `@image_1/2/3`)
- 📋 **Storyboard-to-video** pipeline (verified Day 19 xianxia + Day 24 commercial)
- 🎬 **Cinema trailer 30s** (2 segments × 15s ghép CapCut — verified Day 26)
- 🎥 **Cinema narrative 70s** (5 segments × 15s — verified Day 27 "Cậu và Bơ")
- 🎨 **Cinematic camera moves** Pan/Zoom/Tracking (verified Day 25)
- 🛒 **Commercial ad TikTok/Reels** F&B + beauty generic + street food (LOW risk per Risk Matrix Day 22)
- 🇨🇳 **Prompt tiếng Trung** cho cinematic VN context (richer vocab than EN)

### ❌ Skip when

- Cần video **>15s 1 segment** — Seedance cap 15s, phải split + ghép CapCut
- **Multi-age character detailed faces** trong 1 video → trigger filter #c455 (Day 27 verified mitigation)
- **Branded products HIGH risk** (sneaker Nike, electronics Apple, xe hơi) → text-to-video FAIL do training bias. Mitigation: image-to-video pipeline (Day 25 verified fix sneaker)
- Cần **"TOTAL SILENCE"** trong audio — Seedance ignore instruction, phải edit CapCut manual (Day 27 insight 8)
- Cần **camera movement complex motion library** (multi-step choreography) — Kling Motion mạnh hơn

### 🔑 Prompt strategy

- **Hierarchy ngôn ngữ:** 🇨🇳 中文 > 🇬🇧 Tiếng Anh > 🇻🇳 (kém support)
- **Sweet spot độ dài:** 200-400 từ với 5 elements (Subject + Action + Setting + Camera + Audio)
- **Magic structure:** 21-shot Hollywood narrative cho cinema, 5-shot story arc cho commercial
- **Multi-ref pattern:** `@image_1 = Character`, `@image_2 = Style/Storyboard`, `@image_3 = Props/Hooded Figure`
- **Anti-patterns:**
  - ❌ Multi-age numerical "30岁/45岁/55岁" → filter #c455
  - ❌ Storyboard refs có text labels → bleed gibberish into video
  - ❌ "Total silence" instruction → not respected, edit CapCut manual
  - ✅ Soften aging: "middle-aged with gray temples" thay "45 years old"
  - ✅ "Absolutely no readable text" front-load avoid text bleed
  - ✅ Mute audio Memorable Moment manually trong CapCut

### 💰 Giá trị thực tế

**Gói Ultra Member 1.000.000đ (1.1 triệu credit) = ~55-73 video segments × 15s**

→ **Commercial 30s** = 2 segments × ~17K = **~34K credit** = **~25-30 ads từ 1tr credit**
→ **Cinema 70s narrative** = 5 segments × ~20K = **~100-140K credit** = **~8-10 phim từ 1tr credit**

### 📊 Risk Matrix Seedance (verified Day 22 + Day 25)

| Category | Text-to-Video | Image-to-Video |
|---|---|---|
| 🟢 F&B (cà phê, bún bò...) | ✅ PASS | ✅ PASS |
| 🟢 Beauty generic (serum, dưỡng da...) | ✅ PASS | ✅ PASS |
| 🟢 Street food (bánh mì, phở...) | ✅ PASS | ✅ PASS |
| 🟢 Pháp phục / spiritual (Day 26) | ✅ PASS | ✅ PASS |
| 🟢 Cinema narrative emotional (Day 27) | ✅ PASS | ✅ PASS |
| 🔴 Sneaker branded (Nike, Adidas) | ❌ FAIL (training bias) | ✅ PASS (Day 25 verified FIX) |
| 🔴 Electronics (iPhone, MacBook) | ❌ FAIL | ⚠️ Cần test |
| 🔴 Xe hơi branded | ❌ FAIL | ⚠️ Cần test |

---

## 🌳 Decision Tree — Tôi nên dùng model nào?

```
🤔 Bạn cần tạo gì?
│
├── 🖼️ ẢNH (static)
│   │
│   ├── 📸 Chân dung thời trang / biểu cảm cuốn hút / glamour
│   │   └── ✅ Seedream 4.5
│   │
│   ├── 🛒 Ảnh sản phẩm cao cấp (đồng hồ, mỹ phẩm, trang sức)
│   │   ├── 💰 Ngân sách rộng + cần xuất sắc → ✅ GPT Image 2
│   │   └── 💸 Ngân sách hạn chế + đủ tốt → ✅ Seedream 4.5
│   │
│   ├── 🌄 Phong cảnh Việt Nam (Hà Nội, Hội An, Sapa, miền Tây)
│   │   └── ✅ NBN2
│   │
│   ├── ✍️ Ảnh có text tiếng Việt có dấu (biển hiệu, poster, packaging)
│   │   └── ✅ Seedream 4.5
│   │
│   ├── 🎨 Anime / hoạt hình / illustration / chibi
│   │   └── ✅ NBN2
│   │
│   ├── 🎭 Character sheet multi-age (cho video narrative)
│   │   └── ✅ Seedream 4.5 (Day 27 verified 4 ages × 2 views)
│   │
│   ├── 📋 Storyboard grid 4×4 hoặc 4-panel
│   │   └── ✅ Seedream 4.5 (Day 18 verified)
│   │
│   ├── ⚡ Cần ảnh GẤP cho khách hàng quan trọng
│   │   └── ✅ GPT Image 2 (nhanh + ít rủi ro miss)
│   │
│   ├── 💡 Test ý tưởng nháp / draft, không cần đẹp
│   │   └── ✅ Seedream 4.5 (rẻ nhất)
│   │
│   ├── 🎬 Ảnh cinematic 21:9 (concept art, poster phim)
│   │   └── ✅ Seedream 4.5
│   │
│   ├── 👻 Hooded figure / atmospheric still (peaceful tone)
│   │   └── ✅ GPT Image 2 (Day 27 verified)
│   │
│   └── 🇻🇳 Prompt 100% tiếng Việt không muốn dịch
│       └── ✅ NBN2
│
└── 🎬 VIDEO (motion)
    │
    ├── 🎞️ Text-to-video clip 10-15s từ prompt
    │   └── ✅ Seedance Omni 2.0
    │
    ├── 🖼️ Image-to-video animate ảnh tĩnh
    │   └── ✅ Seedance Omni 2.0 (multi-ref 3 @image refs)
    │
    ├── 📢 Commercial ad TikTok/Reels 15s
    │   ├── 🟢 LOW risk category (F&B, beauty, street food) → Seedance text-to-video
    │   └── 🔴 HIGH risk branded (sneaker, electronics) → Seedance image-to-video pipeline
    │
    ├── 🎬 Cinema trailer 30s (commercial high-emotion)
    │   └── ✅ Seedance Omni 2.0 — 2 segments × 15s + CapCut hybrid (Day 26 pattern)
    │
    ├── 🎥 Cinema narrative 60-70s (storytelling dài form)
    │   └── ✅ Seedance Omni 2.0 — 5 segments × 15s + CapCut edit (Day 27 pattern)
    │
    └── 🎬 Camera movement (Pan/Zoom/Tracking/Dolly)
        └── ✅ Seedance Omni 2.0 (Day 25 verified 6 movements)
```

---

## 💰 1 Triệu credit làm được gì? (Strategy phân bổ)

Giả sử bạn mua **Ultra Member 1.000.000đ → 1.100.000 credits** (+10% bonus).

| Strategy | Phân bổ | Tổng output ước tính | Phù hợp ai? |
| --- | --- | --- | --- |
| 💚 **Tiết kiệm image** | 80% Seedream + 20% NBN2 | ~3,065 ảnh | Newbie học tập, content creator volume cao |
| 🟡 **Cân bằng image** | 50% Seedream + 30% NBN2 + 20% GPT | ~2,545 ảnh | Đa số người dùng, mix project |
| 🔴 **Premium image** | 60% GPT + 40% Seedream | ~2,000 ảnh | Freelancer/agency làm khách hàng |
| 🇻🇳 **Tiếng Việt focus** | 70% NBN2 + 20% Seedream + 10% GPT | ~2,592 ảnh | Content sáng tạo nội dung Việt |
| 📸 **Chân dung pro** | 70% Seedream + 30% GPT | ~2,567 ảnh | Photographer, fashion creator |
| 🎬 **Video commercial** | 80% Seedance + 20% Seedream (storyboard) | ~50 ads commercial 15-30s | Creator commercial ad, brand marketing |
| 🎥 **Cinema narrative** | 70% Seedance + 30% Seedream (multi-age refs) | ~6-8 phim cinema 60-70s | Creator storytelling, personal brand |

> **🔥 Insight mình rút ra:** Đừng dùng 100% GPT Image 2! Chỉ ~1,222 ảnh / 1tr — tốn nhanh. Dùng GPT cho 20% ảnh quan trọng, còn lại cho Seedream/NBN2 sẽ tiết kiệm 60%+ credit.
>
> 🔥 **Video:** 1 video commercial 15s = ~17K credit, 1 cinema 70s = ~100K credit. Plan trước số ad/phim cần làm tháng → ngân sách credit chính xác.

---

## ⚙️ Quick Setting Reference

### Aspect Ratio + Resolution recommend

| Tác vụ | Seedream 4.5 | NBN2 | GPT Image 2 | Seedance 2.0 |
| --- | --- | --- | --- | --- |
| Chân dung dọc | **3:4 @ 2K** | 3:4 @ 2K | 3:4 @ 2K | 9:16 video |
| Cảnh ngang chuẩn | 16:9 @ 2K | 16:9 @ 2K | 16:9 @ 2K | 16:9 video |
| Cinematic rộng | **21:9 @ 2K** ⭐ | 16:9 (yếu hơn) | 16:9 @ 2K | 21:9 video |
| Vuông MXH | 1:1 @ 2K | 1:1 @ 2K | 1:1 @ 2K | 1:1 video |
| Story dọc TikTok/Reels | 9:16 @ 2K | 9:16 @ 2K | 9:16 @ 2K | **9:16 @ 15s** ⭐ |

### Negative Prompt template (universal — copy paste cho mọi model image)

```
plastic skin, oversaturated, deformed eyes, extra fingers,
extra limbs, watermark, low quality, blurry, jpeg artifacts
```

Thêm cho ảnh photo realistic:

```
+ cartoon, anime, painting, illustration
```

Thêm cho ảnh chân dung:

```
+ smooth airbrushed face, doll-like skin, fake makeup
```

### Avoid list template cho Seedance video (verified Day 22-27)

```
absolutely no readable text, no subtitles, no captions, no logos,
no watermarks, no banner labels, fast cuts, MTV-style effects,
grid output, character drift, modern skyscrapers (if vintage era),
LED hospital lighting (if vintage hospital)
```

---

## 📊 Update log — Mỗi model đã test khi nào?

| Thời điểm | Model | Day liên quan | Số ảnh/video đã test | Status |
| --- | --- | --- | --- | --- |
| Tuần 1 (đến 08/05/2026) | NBN2 | Day 1-7 | ~50+ ảnh | ✅ Done |
| Tuần 1 (đến 08/05/2026) | GPT Image 2 | Day 1-7 | ~50+ ảnh | ✅ Done |
| Tuần 2 (08-09/05/2026) | Seedream 4.5 | Day 8-9 | 21+ ảnh | ✅ Done |
| Tuần 3 (10-12/05/2026) | Seedance 2.0 text-to-video | Day 12-13 | 6+ video | ✅ Done |
| Tuần 3 (13/05/2026) | Storyboard pipeline | Day 18-20 | 2 short films | ✅ Done |
| Tuần 4 (Day 22-25) | Seedance commercial production | Day 22-25 | 4+ commercial ads | ✅ Done |
| Tuần 4 (Day 26) | Seedance Cinema Trailer 30s | Day 26 | 1 trailer + 4 ảnh foundation | ✅ Done |
| Tuần 4 (Day 27) | Seedance Cinema Narrative 70s | Day 27 | 1 phim 70s + 8 ảnh foundation | ✅ Done |
| Tuần 4 (Day 28) | Recap + Mini Challenge launch | Day 28 | — | ✅ Done |

> **📝 Cách mình test:** Mỗi model dùng cùng prompt + cùng aspect ratio + cùng resolution để so sánh công bằng (A/B/C testing). Mỗi prompt chạy 1 lần — KHÔNG cherry-pick ảnh đẹp.

---

## 📍 Related Resources

- 🌐 **0ai.vn:** <https://0ai.vn>
- 💰 **Pricing chi tiết (22 gói):** [PRICING.md](https://github.com/linhai-creator/linh0ai-daily-tutorials/blob/main/PRICING.md)
- 📖 **Curriculum 28 ngày:** [CURRICULUM.md](https://github.com/linhai-creator/linh0ai-daily-tutorials/blob/main/CURRICULUM.md)
- 📝 **Bài Day 8 (Seedream 4.5 deep dive):** [days/day-08.md](https://github.com/linhai-creator/linh0ai-daily-tutorials/blob/main/days/day-08.md)
- 🎬 **Bài Day 27 (Cinema 70s narrative):** [days/day-27.md](https://github.com/linhai-creator/linh0ai-daily-tutorials/blob/main/days/day-27.md)
- 🚀 **Bắt đầu từ đâu?** [START-HERE.md](https://github.com/linhai-creator/linh0ai-daily-tutorials/blob/main/START-HERE.md)

---

## 📚 Glossary nhanh

- **Credit:** đơn vị tiền tệ trên 0ai.vn. 1 credit ≈ 1đ VND
- **Native resolution:** độ phân giải gốc model tạo, không tính upscale
- **Character consistency:** giữ nguyên gương mặt nhân vật qua nhiều ảnh
- **Hybrid prompt:** trộn tiếng Việt + tiếng Anh trong cùng 1 prompt
- **Negative prompt:** từ khóa CHẶN — nói model "đừng tạo cái này"
- **Cherry-pick:** chạy nhiều lần rồi chọn ảnh đẹp nhất → kết quả review không trung thực
- **Multi-ref hybrid:** upload nhiều ảnh ref đồng thời cho video (Day 24 verified)
- **Filter #c455:** trigger filter của 0ai.vn khi prompt detail face + age + ethnic (Day 27 verified)
- **Memorable Moment:** 1 khoảnh khắc 3-6s static design cho cry-trigger (Day 26-27 pattern)
- **Risk Matrix:** bảng phân loại HIGH/LOW risk category cho Seedance branded products (Day 22 + Day 25)

---

*Made with ❤️ by **Linh0AI** — chuỗi 28 ngày làm chủ AI tạo ảnh & video trên 0ai.vn 🇻🇳*

*Cập nhật lần cuối: 15/05/2026 | Phiên bản 2.0*
