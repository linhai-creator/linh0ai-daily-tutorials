# 🎯 Day 8 — Seedream 4.5: Vũ khí bí mật cho chân dung & da người

> **Level:** 🔵 Intermediate (có chỗ 🟢 cho newbie)
> **Thời gian đọc:** ~12 phút | **Thực hành:** ~45 phút
> **Ngày 8/30** | Tuần 2 — Khám phá Model Universe trên 0ai.vn

---

## 🎬 Mở đầu — Tại sao tuần này quan trọng?

Tuần 1 mình đã quen mặt với 2 anh "trùm cuối" Nano Banana 2 (NBN2) và GPT Image 2. Nhưng nếu chỉ dùng 2 model này thì... 0ai.vn lãng phí lắm. Nền tảng có **6+ model AI tạo ảnh** mỗi anh có 1 thế mạnh riêng — và nếu mình chọn đúng model cho đúng tác vụ, **chất lượng ảnh tăng rõ rệt mà credit thì tiết kiệm hơn**.

Tuần 2 (Day 8-14) mình sẽ "thử việc" từng model một, chấm điểm thực tế, tìm ra **mỗi model giỏi nhất ở việc gì**.

Hôm nay mở đầu với một anh khá "chìm" với cộng đồng người Việt: **Seedream 4.5** của ByteDance (cùng nhà với TikTok, CapCut). Spoiler nhẹ: anh này là vũ khí bí mật cho **chân dung biểu cảm phong cách thời trang** — và đặc biệt **rẻ nhất trong nhóm flagship** trên 0ai.vn (350 credit/ảnh, vs 900 của GPT Image 2). 👀

> **🔥 Tại sao Linh chọn 4.5 mà không phải 5.0?**
> Seedream 5.0 là bản mới nhất (2/2026) có tính năng search web + reasoning, nhưng còn beta nhiều, kết quả không ổn định. **Seedream 4.5 (12/2025) đã được tối ưu, production-ready, character consistency cực mạnh, chi phí rẻ**. Cho mục đích **chân dung & ảnh thương mại**, 4.5 là lựa chọn chuẩn chỉnh hơn.

---

## 🎯 Mục tiêu hôm nay

- ✅ Hiểu Seedream 4.5 là gì, mạnh/yếu ở đâu so với NBN2 và GPT Image 2
- ✅ Test 9 ảnh thực tế (3 chủ đề × 3 model) để thấy sự khác biệt
- ✅ Biết **khi nào** nên dùng Seedream 4.5 thay vì model khác
- ✅ Học prompt template chuyên cho chân dung Việt Nam
- ✅ Có cheatsheet 1 trang quyết định nhanh
- ✅ Biết **giá thật** của từng model — không bị giật mình khi hết credit

---

## 💰 Bảng giá thực tế trên 0ai.vn (Day 8 cập nhật)

Trước khi vào nội dung, đây là **giá min cho 1 ảnh** mình test thực tế:

| Model | Giá min/ảnh | So sánh |
|-------|-------------|---------|
| **Seedream 4.5** | **350 credit** | 🥇 Rẻ nhất nhóm flagship |
| Nano Banana 2 (NBN2) | 400 credit | 🥈 |
| **GPT Image 2** | **900 credit** | 🥉 Đắt nhất, gấp 2.57x Seedream |

> **💡 Insight Linh:** Đây là lý do tại sao **chọn đúng model = tiết kiệm credit**. Nếu mỗi ngày bạn tạo 50 ảnh chân dung, dùng GPT Image 2 (45,000 credit) vs Seedream 4.5 (17,500 credit) chênh **27,500 credit/ngày = ~27,500đ/ngày = ~825,000đ/tháng**. Đủ mua thêm 1 gói Image Starter rồi!

---

## 📚 Phần 1 — Seedream 4.5 là ai?

### 🏢 Thông tin cơ bản
- **Nhà phát hành:** ByteDance (cha đẻ TikTok, CapCut)
- **Phát hành:** Tháng 12/2025 — đã ổn định, production-ready
- **Native resolution:** 2048×2048 (4MP, gần 4K) — cao hơn nhiều model khác
- **Aspect ratio hỗ trợ:** Linh hoạt từ 1:1, 16:9, 9:16, 4:3, 3:4, 2:3, 3:2, **21:9** (cinematic)
- **Xếp hạng:** #10 trên LM Arena (1147 điểm) — top-tier toàn cầu

### 💪 4 điểm mạnh độc nhất của 4.5

**1. Cinematic Lighting + Realistic Skin 🎬**
Đây là điểm nâng cấp lớn nhất so với Seedream 4.0. Trong khi 4.0 còn bị "flat lighting" (ánh sáng phẳng giả AI), 4.5 mô phỏng **ánh sáng phim điện ảnh**: bóng đổ tự nhiên, sương khối (volumetric fog), texture da chân thật có lỗ chân lông và phản chiếu ánh sáng.

> **🔥 Insight Linh:** Ngay cả khi prompt không nói gì về ánh sáng, Seedream 4.5 tự auto-render kiểu cinematic — bạn không cần phải prompt nhiều keyword về lighting như với NBN2 hoặc GPT Image 2.

**2. Chân dung biểu cảm phong cách thời trang 👗**
Đây là use case mà cộng đồng creator Châu Á khen Seedream 4.5 nhiều nhất — và mình test thực cũng thấy đúng. Nếu bạn cần ảnh chân dung **tone tạp chí Vogue/Elle, glamour, biểu cảm cuốn hút**, Seedream 4.5 vượt trội rõ so với NBN2 và GPT Image 2 ở **biểu cảm + body language tự nhiên**. Hợp với:
- Ảnh đại diện cá nhân branding
- Lookbook thời trang
- Beauty product visual
- Editorial portrait

**3. Character Consistency với 14 reference images 🎭**
Seedream 4.5 là model **mạnh nhất hiện tại** về giữ nguyên gương mặt nhân vật qua nhiều ảnh. Bạn có thể upload tới **14 ảnh tham chiếu** cùng lúc, model sẽ giữ face structure, tone da, biểu cảm nhất quán — cực hữu ích cho làm bộ ảnh portrait, storyboard, hoặc nhân vật quảng cáo. Đổi background/trang phục/mùa nhưng gương mặt vẫn là **cùng một người**.

**4. Text Rendering xuất sắc + Native tiếng Trung ✍️🇨🇳**
Đây là 2-trong-1 USP độc nhất:
- **Text trong ảnh chuẩn** kể cả tiếng Việt có dấu (cái mà NBN2 hay viết sai)
- **Prompt tiếng Trung native** — vì model train chính bằng data tiếng Trung, prompt tiếng Trung cho kết quả **TỐT NHẤT** (tốt hơn cả tiếng Anh!). Nếu bạn biết tiếng Trung hoặc làm content cho thị trường TQ → đây là vũ khí lớn.

### ⚠️ Điểm yếu đã ghi nhận

- **Tốc độ chậm hơn GPT Image 2** — đây là điểm đáng cân nhắc. GPT Image 2 là model nhanh nhất trên 0ai.vn từ test thực tế của Linh
- **Yếu hơn NBN2 ở phong cách hoạt hình/anime**
- **Prompt tiếng Việt thuần** đôi khi hiểu sai → vẫn nên dùng hybrid (VI+EN), hoặc tiếng Trung nếu biết
- **Sweet spot prompt: 30-100 từ** — ngắn hơn các model khác. Nếu viết dài quá, model "scatter" và bỏ sót chi tiết
- **Earlier keyword được nhấn mạnh hơn** — phải đặt subject lên đầu prompt
- **Đôi khi cảm giác "thương mại"** — không "hồn nghệ thuật" như NBN2 ở phong cách trừu tượng

---

## ⚙️ Phần 2 — Setup test trên 0ai.vn

### Bước 1: Vào Image Generator
Dashboard → **AI Image** → chọn model **Seedream 4.5** từ dropdown.

### Bước 2: Setting cố định cho cả 3 test
| Test | Aspect Ratio | Resolution | Lý do |
|------|--------------|------------|-------|
| Chân dung | 3:4 | 2K | Tỷ lệ chân dung dọc chuẩn, 2K đủ thấy lỗ chân lông |
| Phong cảnh | 21:9 | 2K | Cinematic — tận dụng lợi thế Seedream về cảnh rộng |
| Sản phẩm | 1:1 | 2K | Vuông cho mạng xã hội, 2K đủ chi tiết kim loại |

> **💡 Tip:** Seedream 4.5 native lên tới 2048×2048 (gần 4K), nên 2K bạn vẫn còn dư "đất" để upscale sau nếu cần. Không cần generate 4K ngay từ đầu (tốn credit gấp đôi).

### Bước 3: Quy tắc kiểm soát biến số 🧪
Để so sánh **công bằng** giữa Seedream 4.5, NBN2, GPT Image 2:
- ✅ Dùng **chính xác cùng 1 prompt** cho cả 3 model
- ✅ Dùng **cùng aspect ratio** và **cùng resolution**
- ✅ KHÔNG dùng image-to-image (chỉ text-to-image)
- ✅ Chấp nhận **mỗi model có seed riêng** (đây là biến không kiểm soát được)
- ✅ Mỗi prompt chạy **1 lần duy nhất** — không cherry-pick
- ✅ **Bấm đồng hồ** xem model nào generate nhanh nhất

> **💡 Tip pro:** Đây là phương pháp **A/B/C test chuẩn**. Nhiều người Việt review AI bằng cách chạy 5-10 lần rồi chọn ảnh đẹp nhất → kết quả không trung thực.

### 💰 Chi phí test 9 ảnh hôm nay
| Model | 3 ảnh × giá | Tổng |
|-------|-------------|------|
| Seedream 4.5 | 3 × 350 | **1,050 credit** |
| NBN2 | 3 × 400 | **1,200 credit** |
| GPT Image 2 | 3 × 900 | **2,700 credit** |
| **TỔNG** | | **4,950 credit (~5k VND)** |

Tương đương ~**0.45% gói Ultra Member 1 triệu** (1.1tr credits) — quá rẻ cho data nghiên cứu thực tế!

---

## 🧪 Phần 3 — Test 1: Chân dung (Trọng tâm Day 8) ⭐

### 📝 Prompt sử dụng (hybrid VI + EN, ~60 từ — chuẩn sweet spot Seedream 4.5)
```
Close-up portrait of a 28-year-old Vietnamese woman, natural sun-kissed
skin with visible pores, light freckles, deep brown eyes, natural lashes,
long black hair loosely tied. Soft golden hour window light from left,
gentle shadow falloff on right cheek. Blurred coffee shop bokeh background.
Photorealistic, 85mm f/1.4, shallow depth of field.

Negative: plastic skin, oversaturated, cartoon, deformed eyes,
smooth airbrushed face, watermark, low quality
```

### 🖼️ Kết quả 3 model

**Seedream 4.5:** *(350 credit)*
![Day 8 — Seedream 4.5 chân dung](../assets/images/day-08-seedream-portrait.png)

**Nano Banana 2:** *(400 credit)*
![Day 8 — NBN2 chân dung](../assets/images/day-08-nbn2-portrait.png)

**GPT Image 2:** *(900 credit)*
![Day 8 — GPT Image 2 chân dung](../assets/images/day-08-image2-portrait.png)

### 🔍 Phân tích chi tiết
> ⚠️ **CẦN UPDATE SAU KHI TEST** — đây là dự đoán dựa trên đặc điểm model:

| Tiêu chí | Seedream 4.5 | NBN2 | GPT Image 2 |
|----------|--------------|------|-------------|
| Lỗ chân lông trên da | ⏳ TBD | ⏳ TBD | ⏳ TBD |
| Mắt (chi tiết tròng đen, lông mi) | ⏳ TBD | ⏳ TBD | ⏳ TBD |
| Bóng đổ trên má (cinematic lighting) | ⏳ TBD | ⏳ TBD | ⏳ TBD |
| Tóc (sợi rời, độ rối tự nhiên) | ⏳ TBD | ⏳ TBD | ⏳ TBD |
| Cảm giác "người Việt" (face structure) | ⏳ TBD | ⏳ TBD | ⏳ TBD |
| Biểu cảm cuốn hút | ⏳ TBD | ⏳ TBD | ⏳ TBD |
| ⏱️ Tốc độ generate (giây) | ⏳ TBD | ⏳ TBD | ⏳ TBD |

**🎯 Dự đoán của Linh trước khi test:**
- **Seedream 4.5** sẽ thắng ở **biểu cảm + cinematic lighting + da** (mạnh chân dung phong cách thời trang)
- **NBN2** thắng ở **face structure tự nhiên + hồn người Việt**
- **GPT Image 2** sẽ **nhanh nhất + chất lượng tổng thể ổn định nhất**, nhưng dễ bị "AI plastic skin"

---

## 🌄 Phần 4 — Test 2: Phong cảnh

### 📝 Prompt
```
Mu Cang Chai rice terraces at golden harvest, soft morning mist over
fields, distant H'Mong farmers in traditional clothing harvesting rice.
Golden sunrise piercing clouds, layered mountains backdrop. National
Geographic style, ultra-detailed, warm natural color grading, cinematic.
```

### 🖼️ Kết quả 3 model

**Seedream 4.5:** *(350 credit)*
![Day 8 — Seedream 4.5 phong cảnh](../assets/images/day-08-seedream-landscape.png)

**Nano Banana 2:** *(400 credit)*
![Day 8 — NBN2 phong cảnh](../assets/images/day-08-nbn2-landscape.png)

**GPT Image 2:** *(900 credit)*
![Day 8 — GPT Image 2 phong cảnh](../assets/images/day-08-image2-landscape.png)

### 🔍 Phân tích
> ⚠️ **CẦN UPDATE SAU KHI TEST**

**Điểm cần đánh giá:**
- Có "ra Việt Nam" không, hay sang... Nepal?
- Người H'Mông có đúng trang phục không?
- Sương mù có overlay tự nhiên hay bị giả?
- Tỷ lệ 21:9 có sử dụng tốt không gian không?
- **Cinematic lighting** (USP của Seedream 4.5) có thực sự nổi bật?

---

## 🛍️ Phần 5 — Test 3: Sản phẩm

### 📝 Prompt
```
Luxury men's watch, brown leather strap, white dial with rose gold hands,
stainless steel case. 45-degree angle on white marble with gray veining.
Studio softbox lighting from upper right, subtle sapphire glass reflection.
Soft green leaves bokeh background. Luxury product photography,
tack-sharp details, shallow DOF.
```

### 🖼️ Kết quả 3 model

**Seedream 4.5:** *(350 credit)*
![Day 8 — Seedream 4.5 sản phẩm](../assets/images/day-08-seedream-product.png)

**Nano Banana 2:** *(400 credit)*
![Day 8 — NBN2 sản phẩm](../assets/images/day-08-nbn2-product.png)

**GPT Image 2:** *(900 credit)*
![Day 8 — GPT Image 2 sản phẩm](../assets/images/day-08-image2-product.png)

### 🔍 Phân tích
> ⚠️ **CẦN UPDATE SAU KHI TEST**

**Điểm cần đánh giá:**
- Phản chiếu trên mặt kính sapphire có "thật" không?
- Vân đá cẩm thạch có tự nhiên hay bị "AI pattern"?
- Texture dây da có thấy sợi không?
- Kim đồng hồ có chỉ đúng 10:10 (chuẩn ngành) không?
- **Realistic textures** (USP của Seedream 4.5) có vượt trội?
- GPT Image 2 đắt 2.5x — có xứng đáng cho ảnh sản phẩm không?

---

## 📊 Phần 6 — Bảng tổng kết "Ai thắng cái gì?"

> ⚠️ **CẦN UPDATE SAU KHI TEST** — đây là dự đoán

| Tiêu chí | Seedream 4.5 | NBN2 | GPT Image 2 |
|----------|--------------|------|-------------|
| 👤 Chân dung biểu cảm thời trang | 🥇 Dự đoán nhất | 🥈 | 🥉 |
| 🌄 Phong cảnh thiên nhiên | 🥈 | 🥇 Dự đoán nhất | 🥉 |
| 🛍️ Ảnh sản phẩm/thương mại | 🥇 Dự đoán nhất | 🥉 | 🥈 |
| ⚡ Tốc độ generate | 🥈 | 🥈 | 🥇 (nhanh nhất) |
| 💰 Giá min/ảnh | 🥇 350 credit | 🥈 400 credit | 🥉 900 credit |
| 🏆 Chất lượng tổng thể (consistent) | 🥈 | 🥈 | 🥇 (ổn định nhất) |
| ✍️ Text rendering trong ảnh | 🥇 (vô địch) | 🥉 | 🥈 |
| 🎭 Character consistency | 🥇 (14 ref images) | 🥈 | 🥉 |
| 🇨🇳 Prompt tiếng Trung | 🥇 (native) | 🥈 | 🥉 |
| 🇻🇳 Prompt tiếng Việt thuần | 🥉 | 🥇 | 🥈 |
| 🎨 Phong cách hoạt hình/anime | 🥉 | 🥇 | 🥈 |

> **🤔 Câu hỏi đáng suy ngẫm:** GPT Image 2 nhanh nhất + chất lượng tổng thể tốt nhất — nhưng đắt **gấp 2.57x Seedream 4.5**. Bạn có sẵn sàng chi thêm để có "model auto-pilot" không? Hay chấp nhận học cách chọn model phù hợp để tiết kiệm? Đây là quyết định kinh doanh, không có câu trả lời đúng/sai.

---

## 🎁 Phần 7 — Cheatsheet "Khi nào dùng Seedream 4.5?"

### ✅ DÙNG Seedream 4.5 khi:
- 📸 **Chân dung biểu cảm phong cách thời trang/glamour** — tone tạp chí Vogue/Elle
- 🛒 **Ảnh sản phẩm cao cấp** cần realistic textures (kim loại, kính, da, đá)
- 🎭 **Bộ ảnh nhân vật/nhân vật quảng cáo** — character consistency số 1
- ✍️ **Ảnh có text** trong tranh (biển hiệu tiếng Việt có dấu, logo, packaging)
- 🎬 **Cinematic 21:9** cho ảnh điện ảnh, poster phim, concept art
- 📦 **E-commerce** — sản phẩm + text giá + label cùng lúc
- 💸 **Production volume cao + ngân sách hạn chế** — rẻ nhất nhóm flagship
- 🇨🇳 **Bạn biết tiếng Trung** hoặc làm content cho thị trường TQ

### ❌ KHÔNG dùng Seedream 4.5 khi:
- ⚡ **Cần tốc độ tuyệt đối** (livestream, draft nhanh) → dùng GPT Image 2
- 🏆 **Cần "auto-pilot" reliability** không muốn miss prompt → dùng GPT Image 2
- 🎨 **Phong cách anime/hoạt hình/illustration** → dùng NBN2
- 🇻🇳 **Prompt 100% tiếng Việt** không muốn dịch → dùng NBN2
- 🌐 **Cần content thời sự, search web** → dùng Seedream 5.0 (Day sau)

---

## 💎 Phần 8 — 5 Insights Pro chỉ Linh0AI chia sẻ

> ⚠️ **CẦN VERIFY SAU KHI TEST** — một số là dự đoán dựa trên đặc điểm model

**1. Prompt 30-100 từ là sweet spot — KHÁC các model khác**
Nhiều người tưởng prompt càng dài càng chi tiết. Sai với Seedream 4.5! Nó "scatter" và bỏ sót khi prompt quá dài. **Sweet spot: 30-100 từ**, đặt **chủ thể (subject) lên đầu** vì keyword đầu được nhấn mạnh nhất.

**2. Hierarchy ngôn ngữ: 中文 > Hybrid VI+EN > Tiếng Việt thuần**
Seedream 4.5 train chính bằng data tiếng Trung → **prompt tiếng Trung cho kết quả TỐT NHẤT** (vượt cả tiếng Anh!). Nếu bạn biết tiếng Trung, đây là cheat code. Đa số người Việt không biết Trung → **hybrid VI+EN vẫn là default an toàn**, vẫn cho kết quả ngon. Tránh prompt 100% tiếng Việt thuần với model này.

**3. "Visible pores" là magic word cho da**
Thêm cụm "**natural skin with visible pores**" hoặc "**realistic skin texture**" vào prompt → Seedream render da thật hơn rõ rệt. Combined với cinematic lighting tự động của 4.5, kết quả ngang ảnh chụp Sony A7IV thật.

**4. Bài toán kinh tế: GPT Image 2 vs Seedream 4.5**
Đây là quyết định **business** không phải kỹ thuật. GPT Image 2 nhanh + tốt + đắt 2.57x. Seedream 4.5 chậm hơn chút + tốt ở niche + rẻ hơn 65%. **Best practice của Linh:** dùng GPT Image 2 cho ảnh khách hàng quan trọng (thuê 200k 1 ảnh đáng), dùng Seedream 4.5 cho test ý tưởng + chân dung thời trang + production volume.

**5. Character consistency = vũ khí ít người Việt biết**
Đây là **USP độc nhất** mà cộng đồng Việt chưa khai thác. Upload 1-14 ảnh chân dung của bạn (hoặc 1 nhân vật), Seedream 4.5 sẽ giữ nguyên gương mặt qua nhiều ảnh khác nhau (đổi outfit, background, mùa, mood). Cực hữu ích cho:
- Bộ ảnh thời trang cá nhân
- Nhân vật mascot cho brand
- Storyboard nội dung dài hạn
- Ảnh đại diện social media nhất quán

---

## 🎯 Thử thách hôm nay

### 🟢 Cho Newbie (15 phút, ~350 credit)
1. Generate 1 ảnh chân dung của chính mình (mô tả ngoại hình bạn, ~50 từ)
2. Dùng Seedream 4.5, aspect 3:4, 2K
3. Đăng kết quả vào group Zalo với hashtag `#Day8Linh0AI`

### 🔵 Cho Intermediate (45 phút, ~5,000 credit)
1. Test cả 3 prompt (chân dung + cảnh + sản phẩm) trên cả 3 model
2. **Bấm đồng hồ** xem model nào nhanh nhất
3. So sánh và viết 3 câu insight của riêng bạn
4. Tag mình trên Facebook với hashtag `#Day8Seedream45`

### 🟣 Cho Pro (90 phút, ~10,000 credit)
1. Tạo 1 bộ ảnh **5 chân dung khác nhau** dùng Seedream 4.5 + reference image (test character consistency)
2. Thử 1 prompt **bằng tiếng Trung** (Google Translate cũng OK) — so với hybrid VI+EN xem khác nhau ra sao
3. Viết review ngắn so với MidJourney/DALL-E nếu bạn từng dùng

> 🏆 **Mini Challenge "Phong cảnh Việt Nam"** vẫn đang chạy đến Day 14 (13/05/2026)! Top 3 sẽ được mention trong bài Day 14.

---

## ❓ FAQ

**Q1: Seedream 4.5 có miễn phí không? Giá thật là bao nhiêu?**
Không miễn phí. Trên 0ai.vn, **giá min 1 ảnh Seedream 4.5 là 350 credit** (~350đ). So sánh: NBN2 400 credit, GPT Image 2 900 credit. Seedream 4.5 là **rẻ nhất nhóm flagship**. Nếu dùng gói Ultra Member 1tr (1.1tr credits) thì đủ test ~3,143 ảnh Seedream 4.5.

**Q2: Seedream 4.5 vs Seedream 5.0 — chọn cái nào?**
- **Chọn 4.5** nếu: làm chân dung, sản phẩm thương mại, cần character consistency, tiết kiệm credit, muốn kết quả ổn định production-ready.
- **Chọn 5.0** nếu: cần search web cho content thời sự, cần logical reasoning cho infographic phức tạp, chấp nhận chậm + đắt + kết quả không nhất quán.
- **Tóm lại: 90% trường hợp 4.5 là chuẩn.**

**Q3: GPT Image 2 đắt 2.5x — có nên dùng không?**
Có, **nhưng chọn lọc**. GPT Image 2 nhanh nhất + chất lượng tổng thể tốt nhất + ổn định nhất. Phù hợp cho: ảnh quan trọng (khách hàng, deadline gấp, thumbnail viral). KHÔNG phù hợp cho: test ý tưởng, production volume cao, ngân sách hạn chế. Linh recommend dùng **20% GPT Image 2 + 50% Seedream 4.5 + 30% NBN2** cho mix cân bằng.

**Q4: Seedream có hiểu prompt Việt Nam như "áo dài", "phở", "nón lá" không?**
Có, nhưng kém NBN2. Best practice: kết hợp keyword Việt với mô tả tiếng Anh. Ví dụ: `Vietnamese woman wearing áo dài (traditional long dress), holding a nón lá (conical hat)...` Hoặc nếu biết tiếng Trung → prompt thẳng tiếng Trung cho kết quả tốt nhất.

**Q5: Sao Seedream 4.5 native 2048×2048 mà 0ai.vn vẫn có option 4K?**
Vì 0ai.vn tích hợp tính năng **upscale** (Topaz/Real-ESRGAN) tự động. Generate 2K → upscale 4K cho kết quả tương đương generate native 4K mà tốn ít credit hơn.

**Q6: Test bao nhiêu credit là vừa cho Day 8 này?**
Dự kiến: **4,950 credit** (~5k VND) cho full 9 ảnh = 3 ảnh × 3 model:
- 3 × Seedream 4.5 (350) = 1,050 credit
- 3 × NBN2 (400) = 1,200 credit
- 3 × GPT Image 2 (900) = 2,700 credit

Tương đương ~0.45% gói Ultra Member 1 triệu — **rẻ kinh khủng** cho data nghiên cứu.

**Q7: Có thể dùng Seedream 4.5 cho ảnh thương mại không?**
Có. Theo điều khoản của ByteDance/0ai.vn, ảnh được generate có thể dùng commercial. Tuy nhiên luôn check terms cập nhật trước khi dùng cho dự án trả phí lớn.

---

## 🎬 Recap & Day 9

### Ghi nhớ chính
- ✅ Seedream 4.5 = vũ khí cho **chân dung thời trang, sản phẩm, ảnh có text**
- ✅ Native 2048×2048 (gần 4K), cinematic lighting tự động
- ✅ Character consistency số 1 với 14 reference images
- ✅ Text rendering vô địch (kể cả tiếng Việt có dấu)
- ✅ Sweet spot prompt 30-100 từ, đặt subject lên đầu
- ✅ **350 credit/ảnh** — rẻ nhất nhóm flagship trên 0ai.vn
- ✅ Tiếng Trung > Hybrid VI+EN > Tiếng Việt thuần

### 🔮 Day 9 — Sneak peek
Ngày mai mình sẽ thử **Z-Image** — model mạnh ở **text trong ảnh & 4K native**. Bạn sẽ học cách tạo ảnh có chữ tiếng Việt chuẩn, và làm poster/infographic 4K không cần Photoshop. Spoiler: Z-Image vs Seedream 4.5 sẽ có 1 trận đấu thú vị về text rendering!

---

## 📍 Navigation
[⬅️ Day 7: Tổng kết Tuần 1](./day-07.md) | [🏠 README](../README.md) | [➡️ Day 9: Z-Image](./day-09.md)

## 🏷️ Tags
`#0aiVN #Seedream45 #ByteDance #ChânDungAI #Day8Linh0AI #AIImage #PortraitAI #VietnameseAI #ProductPhotography #FashionAI`

---

> **💌 Có ý kiến hoặc trải nghiệm khác?**
> Comment vào [bài Facebook Day 8](https://facebook.com/daclinh.tran) hoặc nhắn vào [Zalo group](https://zalo.me/g/umthmp096). Mình rất muốn nghe bạn thấy Seedream 4.5 mạnh/yếu ở đâu khác mình!

---

*Nhật ký Day 8 by **Linh0AI** — chuỗi 30 ngày làm chủ AI tạo ảnh & video trên 0ai.vn 🇻🇳*
