# 📖 0ai.vn Models Cheatsheet — 1 Trang Chọn Đúng Model

> **Bản 1.3** — Cập nhật ngày 09/05/2026 (sau Day 11 — GPT Image 2 BIG WIN)
> **Tác giả:** [Linh0AI](https://facebook.com/daclinh.tran)
> **Repo:** [linh0ai-daily-tutorials](https://github.com/linhai-creator/linh0ai-daily-tutorials)
> **Data dựa trên test thực tế** — không phải copy info marketing từ web

---

## 🎯 Cheatsheet này dành cho ai?

- ✅ Bạn dùng **0ai.vn** và phân vân không biết chọn model nào
- ✅ Bạn muốn **tiết kiệm credit** mà vẫn có ảnh chất lượng
- ✅ Bạn cần **quick reference** khi đang work — không có thời gian đọc tutorial dài
- ✅ Bạn từ Việt Nam và muốn biết model nào hiểu prompt Việt tốt nhất

> **⚠️ Lưu ý:** Cheatsheet này hiện cover **3 model flagship đã test** (Seedream 4.5, NBN2, GPT Image 2). Các model khác trên 0ai.vn (NBN Pro, Z-Image, Kling, Seedance...) sẽ được thêm vào bản v2.0 sau khi mình test thật.

---

## 🥇 Bảng so sánh tổng (xem 30 giây là đủ)

| Tiêu chí | 🟦 Seedream 4.5 | 🟨 NBN2 | 🟪 GPT Image 2 |
|----------|-----------------|---------|----------------|
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

> ⚠️ **CẢNH BÁO BẢN QUYỀN — VERIFIED 4 LẦN, BULLETPROOF SOLUTION:** GPT Image 2 hay tự chèn brand thật vào ảnh sản phẩm — Day 8 (Vincero), Day 9 (Dior). **Day 10 + Day 11 ĐÃ FIX hoàn toàn (0/11 ảnh đồng hồ có brand)** bằng negative prompt liệt kê tên brand cụ thể: `brand name, logo, text on dial, watermark, Audemars, Vincero, Rolex, Dior, LV, Gucci, Chanel, Hermes, designer logo`. **Solution chính thức bulletproof — áp dụng cho mọi shop online dùng AI làm ảnh sản phẩm.**
### ❌ Skip when
- **Test ý tưởng / draft / nháp** → Seedream 4.5 (rẻ 2.57x, đủ tốt)
- **Production volume cao** — sẽ cháy credit nhanh → Seedream 4.5
- **Prompt tiếng Việt thuần** không muốn dịch → NBN2
- **Phong cách anime/illustration** → NBN2
- **Cần character consistency với nhiều reference** → Seedream 4.5

### 🔑 Prompt strategy
- **Hierarchy ngôn ngữ:** 🇬🇧 Tiếng Anh > 🇻🇳🇬🇧 Hybrid > 🇻🇳 Tiếng Việt thuần
- **Sweet spot độ dài:** 100-200 từ (cho phép prompt chi tiết hơn)
- **Magic words:** Mention specific camera/lens (`shot on Sony A7IV, 85mm f/1.4`), mood/atmosphere words
- **Negative prompt cần có:** Ít cần hơn 2 model trên — model tự filter tốt

### 💰 Giá trị thực tế
**Gói Ultra Member 1.000.000đ (1.1 triệu credit) = 1,222 ảnh GPT Image 2**

⚠️ **Chỉ bằng 39% so với Seedream 4.5** — cân nhắc trước khi dùng cho mọi ảnh.

---

## 🌳 Decision Tree — Tôi nên dùng model nào?

```
🤔 Bạn cần tạo ảnh gì?
│
├── 📸 Chân dung thời trang / biểu cảm cuốn hút / glamour
│   └── ✅ Seedream 4.5
│
├── 🛒 Ảnh sản phẩm cao cấp (đồng hồ, mỹ phẩm, trang sức)
│   ├── 💰 Ngân sách rộng + cần xuất sắc → ✅ GPT Image 2
│   └── 💸 Ngân sách hạn chế + đủ tốt → ✅ Seedream 4.5
│
├── 🌄 Phong cảnh Việt Nam (Hà Nội, Hội An, Sapa, miền Tây)
│   └── ✅ NBN2
│
├── ✍️ Ảnh có text tiếng Việt có dấu (biển hiệu, poster, packaging)
│   └── ✅ Seedream 4.5
│
├── 🎨 Anime / hoạt hình / illustration / chibi
│   └── ✅ NBN2
│
├── 🎭 Bộ ảnh cùng 1 nhân vật (storyboard, lookbook, mascot)
│   └── ✅ Seedream 4.5 (upload 14 reference images)
│
├── ⚡ Cần ảnh GẤP cho khách hàng quan trọng
│   └── ✅ GPT Image 2 (nhanh + ít rủi ro miss)
│
├── 💡 Test ý tưởng nháp / draft, không cần đẹp
│   └── ✅ Seedream 4.5 (rẻ nhất)
│
├── 🎬 Ảnh cinematic 21:9 (concept art, poster phim)
│   └── ✅ Seedream 4.5
│
└── 🇻🇳 Prompt 100% tiếng Việt không muốn dịch
    └── ✅ NBN2
```

---

## 💰 1 Triệu credit làm được gì? (Strategy phân bổ)

Giả sử bạn mua **Ultra Member 1.000.000đ → 1.100.000 credits** (+10% bonus).

| Strategy | Phân bổ | Tổng ảnh ước tính | Phù hợp ai? |
|----------|---------|-------------------|-------------|
| 💚 **Tiết kiệm** | 80% Seedream + 20% NBN2 | ~3,065 ảnh | Newbie học tập, content creator volume cao |
| 🟡 **Cân bằng (Linh recommend)** | 50% Seedream + 30% NBN2 + 20% GPT | ~2,545 ảnh | Đa số người dùng, mix project |
| 🔴 **Premium quality** | 60% GPT + 40% Seedream | ~2,000 ảnh | Freelancer/agency làm khách hàng |
| 🇻🇳 **Tiếng Việt focus** | 70% NBN2 + 20% Seedream + 10% GPT | ~2,592 ảnh | Content sáng tạo nội dung Việt |
| 📸 **Chân dung pro** | 70% Seedream + 30% GPT | ~2,567 ảnh | Photographer, fashion creator |

> **🔥 Insight Linh:** Đừng dùng 100% GPT Image 2! Chỉ ~1,222 ảnh / 1tr — tốn nhanh. Dùng GPT cho 20% ảnh quan trọng, còn lại cho Seedream/NBN2 sẽ tiết kiệm 60%+ credit.

---

## ⚙️ Quick Setting Reference

### Aspect Ratio + Resolution recommend

| Tác vụ | Seedream 4.5 | NBN2 | GPT Image 2 |
|--------|--------------|------|-------------|
| Chân dung dọc | **3:4 @ 2K** | 3:4 @ 2K | 3:4 @ 2K |
| Cảnh ngang chuẩn | 16:9 @ 2K | 16:9 @ 2K | 16:9 @ 2K |
| Cinematic rộng | **21:9 @ 2K** ⭐ | 16:9 (yếu hơn) | 16:9 @ 2K |
| Vuông MXH | 1:1 @ 2K | 1:1 @ 2K | 1:1 @ 2K |
| Story dọc | 9:16 @ 2K | 9:16 @ 2K | 9:16 @ 2K |

### Negative Prompt template (universal — copy paste cho mọi model)
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

---

## 📊 Update log — Mỗi model đã test khi nào?

| Thời điểm | Model | Day liên quan | Số ảnh đã test | Status |
| --- | --- | --- | --- | --- |
| Tuần 1 (đến 08/05/2026) | NBN2 | Day 1-7 | ~50+ | ✅ Done |
| Tuần 1 (đến 08/05/2026) | GPT Image 2 | Day 1-7 | ~50+ | ✅ Done |
| 08/05/2026 | Seedream 4.5 | Day 8 | 10 ảnh (3 chủ đề × 3 model + 1 bonus 中文) | ✅ Done |
| 09/05/2026 | Seedream 4.5 + GPT Image 2 | Day 9 | 12 ảnh (3 cấp × 2 variation × 2 model) | ✅ Done |
| 09/05/2026 | GPT Image 2 | Day 10 | 15 ảnh (5 quy tắc × 3 chủ đề) — verified KHÔNG có điểm yếu | ✅ Done |
| 09/05/2026 | GPT Image 2 | Day 11 | 18 ảnh (6 lighting × 3 chủ đề) — verified BIG WIN cả 6 lighting | ✅ Done |

> **📝 Cách Linh test:** Mỗi model dùng cùng prompt + cùng aspect ratio + cùng resolution để so sánh công bằng (A/B/C testing). Mỗi prompt chạy 1 lần — KHÔNG cherry-pick ảnh đẹp.

---

## 🤝 Đóng góp cheatsheet

Cheatsheet này là **living document** — sẽ được cập nhật sau mỗi Day quan trọng.

Nếu bạn:
- 🐛 Phát hiện thông tin sai → mở Issue trên GitHub
- 💡 Có insight mới về model nào đó → comment dưới bài Day liên quan
- 📊 Có data test khác mình → share trong [Zalo group](https://zalo.me/g/umthmp096)

Repo: [github.com/linhai-creator/linh0ai-daily-tutorials](https://github.com/linhai-creator/linh0ai-daily-tutorials)

---

## 📍 Related Resources

- 🌐 **0ai.vn:** https://0ai.vn
- 💰 **Pricing chi tiết (22 gói):** [PRICING.md](./PRICING.md)
- 📖 **Curriculum 30 ngày:** [CURRICULUM.md](./CURRICULUM.md)
- 📝 **Bài Day 8 (Seedream 4.5 deep dive):** [days/day-08.md](./days/day-08.md)
- 🚀 **Bắt đầu từ đâu?** [START-HERE.md](./START-HERE.md)
- 🟣 **Bài Day 9 (Prompt Engineering Nâng Cao):** [days/day-09.md](https://github.com/linhai-creator/linh0ai-daily-tutorials/blob/main/days/day-09.md)
- 🎬 **Bài Day 10 (Composition & Framing):** [days/day-10.md](https://github.com/linhai-creator/linh0ai-daily-tutorials/blob/main/days/day-10.md)
- 💡 **Bài Day 11 (Lighting Mastery):** [days/day-11.md](https://github.com/linhai-creator/linh0ai-daily-tutorials/blob/main/days/day-11.md)
---

## 📚 Glossary nhanh

- **Credit:** đơn vị tiền tệ trên 0ai.vn. 1 credit ≈ 1đ VND
- **Native resolution:** độ phân giải gốc model tạo, không tính upscale
- **Character consistency:** giữ nguyên gương mặt nhân vật qua nhiều ảnh
- **Hybrid prompt:** trộn tiếng Việt + tiếng Anh trong cùng 1 prompt
- **Negative prompt:** từ khóa CHẶN — nói model "đừng tạo cái này"
- **Cherry-pick:** chạy nhiều lần rồi chọn ảnh đẹp nhất → kết quả review không trung thực

---

*Made with ❤️ by **Linh0AI** — chuỗi 30 ngày làm chủ AI tạo ảnh & video trên 0ai.vn 🇻🇳*

*Cập nhật lần cuối: 09/05/2026 | Phiên bản 1.3*
