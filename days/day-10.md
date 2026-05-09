# 🎯 Day 10 — Composition & Framing: 5 Quy Tắc Bố Cục Kinh Điển

> **Level:** 🟣 Advanced (có chỗ 🔵 cho intermediate)
> **Thời gian đọc:** ~17 phút | **Thực hành:** ~55 phút
> **Ngày 10/30** | Tuần 2 — Master Skills

---

## 🎬 Mở đầu — Tại sao composition quan trọng hơn model?

Day 8-9 mình đã so sánh 3 model AI hàng đầu và thấy: **chất lượng ảnh phụ thuộc 50% vào model, 50% vào cách prompt**. Nhưng còn 1 yếu tố quan trọng hơn cả 2 thứ trên — đó là **bố cục (composition)**.

Bằng chứng: 1 ảnh chụp iPhone bố cục đẹp **vẫn hơn** 1 ảnh DSLR Sony A7IV bố cục lộn xộn. AI cũng vậy:
- 🚨 Ảnh AI ở model rẻ + composition tốt → đẹp + share-worthy
- 🚨 Ảnh AI ở model đắt + composition lộn xộn → đẹp về kỹ thuật nhưng "không có hồn"

Day 10 hôm nay mình deep dive **5 quy tắc composition kinh điển** — mà 90% ảnh AI bỏ qua. Demo qua 3 chủ đề thực tế (chân dung Sài Gòn + phố cổ Hội An + sản phẩm) trên **GPT Image 2** — model đắt nhất nhóm flagship để xem có "tự động" composition đẹp không.

> **🔥 Spoiler:** Sau bài này, ảnh AI của Linh sẽ bỏ được "AI flat look" — vibe phẳng đặc trưng mà ai nhìn cũng biết là AI generate.

---

## 🎯 Mục tiêu hôm nay

- ✅ Master 5 quy tắc composition: **Rule of Thirds, Leading Lines, Symmetry, Negative Space, Foreground/Mid/Bg**
- ✅ Biết keyword chính xác để prompt từng quy tắc
- ✅ Hiểu khi nào dùng quy tắc nào (cheatsheet 1 trang)
- ✅ Test giả thuyết: GPT Image 2 có "tự động" composition đẹp khi không nói gì không?
- ✅ Tránh **5 lỗi composition** AI hay mắc phải

---

## 📚 Phần 1 — 5 Quy Tắc Composition Kinh Điển

### 🎯 Quy tắc 1: Rule of Thirds (1/3)

**Khái niệm:** Chia ảnh thành lưới 3×3 bằng 2 đường dọc + 2 đường ngang. Đặt subject tại 1 trong 4 **giao điểm** (mạnh hơn để giữa).

```
+---+---+---+
|   |   |   |
+---●---+---●---+
|   |   |   |
+---●---+---●---+    ← ● là 4 giao điểm
|   |   |   |
+---+---+---+
```

**Vibe:** Tự nhiên, dynamic, không cứng nhắc
**Khi dùng:** Chân dung, phong cảnh, product flat lay
**Keyword:** `rule of thirds composition`, `subject at intersection`, `subject positioned at right third`

---

### 📐 Quy tắc 2: Leading Lines

**Khái niệm:** Dùng đường nét trong ảnh (đường, hàng cột, cầu thang, ruộng bậc thang) để **dẫn mắt người xem** vào subject chính.

**Loại đường thường gặp:**
- 📏 Đường thẳng → mạnh mẽ, formal
- 🌊 Đường cong → mềm mại, organic
- 🔺 Đường chéo (diagonal) → dynamic, dramatic
- ⛓️ Đường hội tụ (converging) → tạo chiều sâu mạnh

**Vibe:** Có hướng, có chiều sâu
**Khi dùng:** Đường phố, kiến trúc, ruộng bậc thang
**Keyword:** `leading lines toward subject`, `converging lines`, `diagonal lines`

---

### 🪞 Quy tắc 3: Symmetry (Đối xứng)

**Khái niệm:** Bố cục cân bằng tuyệt đối — trái = phải, trên = dưới, hoặc đối xứng tâm.

**3 loại đối xứng:**
- ↔️ **Vertical (dọc)** — mirror trái-phải (kiến trúc, mặt người)
- ↕️ **Horizontal (ngang)** — phản chiếu trên mặt nước
- 🌀 **Radial (tâm)** — tỏa từ tâm (mandala, vòng xoay)

**Vibe:** Formal, ổn định, "weighty"
**Khi dùng:** Kiến trúc, sản phẩm trang trọng, phản chiếu nước
**Keyword:** `symmetrical composition`, `perfect mirror symmetry`, `radial symmetry`

> ⚠️ **Cảnh báo:** Symmetry là quy tắc **KHÓ NHẤT** cho AI — chỉ lệch 1-2 pixel là trông "kệch cỡm". Cần model có geometric precision cao.

---

### ⚪ Quy tắc 4: Negative Space (Khoảng trống)

**Khái niệm:** Để **80% ảnh là không gian trống**, subject nhỏ chiếm 20%. Tăng impact + minimal vibe.

**Vibe:** Yên tĩnh, contemplative, modern minimal
**Khi dùng:** Quảng cáo cao cấp, mood ảnh, branding tối giản
**Keyword:** `negative space`, `minimalist composition`, `isolated subject`, `vast empty space around subject`

> 💡 **Tip pro:** Đây là phong cách **Apple/Muji/COS** dùng — vibe "premium minimal" cực thịnh hành 2026.

---

### 🎬 Quy tắc 5: Foreground / Midground / Background (FG/MG/BG)

**Khái niệm:** Chia ảnh thành **3 lớp chiều sâu**:
- **Foreground** (gần camera, blur) → tạo "frame" tự nhiên
- **Midground** (subject chính, sharp focus)
- **Background** (xa, soft blur)

**Vibe:** Cinematic, có chiều sâu thật, không "phẳng"
**Khi dùng:** Mọi ảnh muốn bỏ "AI flat look"
**Keyword:** `foreground bokeh + midground subject + background blur`, `three-layer depth composition`

> 🔥 **Insight Linh:** Đây là **cách số 1 để bỏ AI flat look** — ảnh AI mặc định bị flat vì model không tự thêm foreground. Bạn phải prompt rõ.

---

## ⚙️ Phần 2 — Setup test

### Quy tắc kiểm soát biến số
- ✅ Cùng 1 model: **GPT Image 2** (test xem model đắt có composition tốt không)
- ✅ Mỗi quy tắc test trên **3 chủ đề**: chân dung + cảnh + sản phẩm
- ✅ KHÔNG cherry-pick — mỗi prompt chạy 1 lần

### 15 ảnh test = 5 quy tắc × 3 chủ đề × 1 model

| Chủ đề | Aspect | Setting |
|--------|--------|---------|
| **Chân dung** | 3:4 | Cô gái casual + Thảo Điền Sài Gòn |
| **Phong cảnh** | 16:9 | Phố cổ Hội An |
| **Sản phẩm** | 1:1 | Đồng hồ luxury (generic) |

### 💰 Chi phí
**15 ảnh × 900 credit = 13,500 credit (~13.5k VND, ~1.2% gói Ultra Member 1 triệu)**

---

## 🧪 Phần 3 — Test Quy Tắc 1: Rule of Thirds

### 📝 Prompt Pattern

```
[subject], (rule of thirds composition:1.4),
subject positioned at right intersection of grid,
[setting], [lighting], photorealistic, [lens].
```

### 🖼️ Kết quả 3 chủ đề

**Chân dung — Cô gái casual Thảo Điền:**
![Day 10 — Thirds Portrait](../assets/images/day-10-thirds-portrait.png)

**Phong cảnh — Phố cổ Hội An:**
![Day 10 — Thirds Landscape](../assets/images/day-10-thirds-landscape.png)

**Sản phẩm — Đồng hồ luxury:**
![Day 10 — Thirds Product](../assets/images/day-10-thirds-product.png)

### 🔍 Phân tích

> ⚠️ **CẦN UPDATE SAU KHI TEST**

**Câu hỏi cần đánh giá:**
- Subject có đúng ở vị trí **giao điểm 1/3** không, hay vẫn ở giữa?
- GPT Image 2 có hiểu keyword `rule of thirds composition` không?
- Có cần prompt cụ thể vị trí (vd `right intersection`, `upper third`) không?

---

## 🧪 Phần 4 — Test Quy Tắc 2: Leading Lines

### 📝 Prompt Pattern

```
[subject], (leading lines composition:1.4),
[describe lines that lead to subject — diagonal/converging/curved],
[setting], [lighting], photorealistic, [lens].
```

### 🖼️ Kết quả 3 chủ đề

**Chân dung:**
![Day 10 — Lines Portrait](../assets/images/day-10-lines-portrait.png)

**Phong cảnh — Phố cổ Hội An:**
![Day 10 — Lines Landscape](../assets/images/day-10-lines-landscape.png)

**Sản phẩm:**
![Day 10 — Lines Product](../assets/images/day-10-lines-product.png)

### 🔍 Phân tích

> ⚠️ **CẦN UPDATE SAU KHI TEST**

**Điểm dự đoán:**
- Hội An sẽ thắng ở quy tắc này (đường phố hẹp + đèn lồng song song = leading lines tự nhiên)
- Sản phẩm khó hơn — cần chủ động tạo lines từ strap/marble veins
- Chân dung Thảo Điền có thể ra "modern industrial lines" đẹp

---

## 🧪 Phần 5 — Test Quy Tắc 3: Symmetry

### 📝 Prompt Pattern

```
[subject], (perfect symmetrical composition:1.4),
[describe symmetry type — mirror/radial/reflection],
[setting with symmetric elements], photorealistic, [lens].
```

### 🖼️ Kết quả 3 chủ đề

**Chân dung:**
![Day 10 — Symmetry Portrait](../assets/images/day-10-symmetry-portrait.png)

**Phong cảnh — Hội An reflection:**
![Day 10 — Symmetry Landscape](../assets/images/day-10-symmetry-landscape.png)

**Sản phẩm:**
![Day 10 — Symmetry Product](../assets/images/day-10-symmetry-product.png)

### 🔍 Phân tích

> ⚠️ **CẦN UPDATE SAU KHI TEST — đây là quy tắc KHÓ NHẤT**

**Điểm cần đánh giá:**
- GPT có làm symmetry **chính xác** không, hay lệch 5-10%?
- Reflection trong nước Hội An có chuẩn không?
- Symmetric lighting (shadow trái = shadow phải) có hoạt động không?

---

## 🧪 Phần 6 — Test Quy Tắc 4: Negative Space

### 📝 Prompt Pattern

```
[subject] small in frame, (negative space composition:1.4),
(minimalist composition:1.3), 80% empty space,
subject occupies only [position], photorealistic, [lens].
```

### 🖼️ Kết quả 3 chủ đề

**Chân dung:**
![Day 10 — Negative Portrait](../assets/images/day-10-negative-portrait.png)

**Phong cảnh:**
![Day 10 — Negative Landscape](../assets/images/day-10-negative-landscape.png)

**Sản phẩm:**
![Day 10 — Negative Product](../assets/images/day-10-negative-product.png)

### 🔍 Phân tích

> ⚠️ **CẦN UPDATE SAU KHI TEST**

**Điểm dự đoán:**
- Negative space là quy tắc **AI hay từ chối nhất** — model có xu hướng "fill" không gian trống
- Có thể phải prompt rõ `80% empty`, `vast empty`, `isolated subject`
- Sản phẩm dễ nhất, chân dung khó nhất

---

## 🧪 Phần 7 — Test Quy Tắc 5: Foreground/Midground/Background ⭐

### 📝 Prompt Pattern (QUAN TRỌNG NHẤT BÀI)

```
[subject scene]. (Three-layer depth composition:1.4):
(foreground:1.2) [blurred element close to camera],
(midground:1.3) [subject sharp focus mid-frame],
(background:1.2) [environment soft blur far behind].
photorealistic, [lens with shallow DOF].
```

### 🖼️ Kết quả 3 chủ đề

**Chân dung:**
![Day 10 — Depth Portrait](../assets/images/day-10-depth-portrait.png)

**Phong cảnh:**
![Day 10 — Depth Landscape](../assets/images/day-10-depth-landscape.png)

**Sản phẩm:**
![Day 10 — Depth Product](../assets/images/day-10-depth-product.png)

### 🔍 Phân tích — QUAN TRỌNG NHẤT

> ⚠️ **CẦN UPDATE SAU KHI TEST**

**Tại sao đây là phần quan trọng nhất:**
Foreground/Mid/Bg là **cách số 1 để bỏ "AI flat look"**. Nếu Linh học được 1 thứ duy nhất hôm nay → học cái này.

**Điểm cần đánh giá:**
- 3 lớp depth có rõ ràng không?
- Foreground bokeh có chính xác không (blur đúng cách)?
- Subject midground có đủ sharp không?
- Background có blur "tự nhiên" hay bị fake?

---

## 📊 Phần 8 — Bảng tổng kết: GPT Image 2 vs 5 quy tắc

> ⚠️ **CẦN UPDATE SAU KHI TEST**

| Quy tắc | Chân dung | Phong cảnh | Sản phẩm | Tổng |
|---------|-----------|------------|----------|------|
| Rule of Thirds | ⏳ TBD | ⏳ TBD | ⏳ TBD | ⏳ TBD |
| Leading Lines | ⏳ TBD | ⏳ TBD | ⏳ TBD | ⏳ TBD |
| Symmetry | ⏳ TBD | ⏳ TBD | ⏳ TBD | ⏳ TBD |
| Negative Space | ⏳ TBD | ⏳ TBD | ⏳ TBD | ⏳ TBD |
| FG/MG/BG | ⏳ TBD | ⏳ TBD | ⏳ TBD | ⏳ TBD |

**🎯 Dự đoán Linh:**
- GPT Image 2 sẽ **dễ dàng làm Rule of Thirds + Leading Lines**
- **Symmetry** sẽ là điểm yếu (model AI nói chung kém ở geometric precision)
- **Negative Space** có thể bị "AI lo lắng filling" — model thêm object phụ
- **FG/MG/BG** sẽ là quy tắc cải thiện ảnh **nhiều nhất** — fix hoàn toàn AI flat look

---

## 🚨 Phần 9 — 5 Lỗi Composition AI Hay Mắc Phải (BONUS)

### Lỗi 1: 🎯 Subject ở giữa cứng nhắc (default behavior)
**Nguyên nhân:** AI training data có nhiều ảnh portrait centered (selfie, ID photo).
**Fix:** Luôn thêm `(rule of thirds composition:1.4)` + chỉ rõ vị trí (`right intersection`, `upper third`).

### Lỗi 2: 🟦 Thiếu foreground (ảnh "phẳng")
**Nguyên nhân:** AI prefer 2-layer (subject + background) cho đơn giản.
**Fix:** Prompt cụ thể `foreground: [object] blurred close to camera`.

### Lỗi 3: 📐 Leading lines ngẫu nhiên không dẫn về subject
**Nguyên nhân:** AI hiểu "leading lines" nhưng không biết "lead to where".
**Fix:** Prompt rõ `lines converging toward subject`, `lines pointing to [subject location]`.

### Lỗi 4: ⚪ Negative space bị spam object
**Nguyên nhân:** AI có xu hướng fill không gian trống bằng birds, clouds, leaves.
**Fix:** Negative weight: `(empty sky:0.7), (cluttered:1.5)` chặn fill.

### Lỗi 5: 🪞 Symmetry lệch nhẹ → "kệch cỡm"
**Nguyên nhân:** AI khó render geometric perfect.
**Fix:** Dùng setting đối xứng tự nhiên (cửa, hành lang, water reflection) — dễ hơn build symmetry từ đầu.

---

## 🎁 Phần 10 — Cheatsheet "Khi nào dùng quy tắc nào?"

### ✅ DÙNG Rule of Thirds khi:
- 📸 Chân dung casual, tự nhiên
- 🌅 Phong cảnh nói chung
- 🛒 Product flat lay đơn giản

### ✅ DÙNG Leading Lines khi:
- 🛤️ Đường phố, kiến trúc có lines rõ
- 🌾 Ruộng bậc thang, hàng cây
- 🎢 Cầu thang, hàng cột

### ✅ DÙNG Symmetry khi:
- 🏛️ Kiến trúc trang trọng (đền, dinh, cầu)
- 💎 Sản phẩm trang trọng (luxury)
- 🌊 Phản chiếu mặt nước phẳng

### ✅ DÙNG Negative Space khi:
- 📢 Ảnh quảng cáo cao cấp (Apple/Muji vibe)
- 🌫️ Mood ảnh contemplative
- 🎨 Branding tối giản

### ✅ DÙNG FG/MG/BG khi:
- 🎬 Mọi ảnh muốn cinematic
- 🎯 Mọi ảnh muốn bỏ "AI flat look"
- → **Recommend dùng cho HẦU HẾT ảnh**

---

## 💎 Phần 11 — 5 Insights Pro chỉ Linh0AI chia sẻ

> ⚠️ **CẦN VERIFY SAU KHI TEST** — một số là dự đoán

**1. Composition > Model — bằng chứng từ test**
Cùng GPT Image 2, prompt composition tốt → ảnh đẹp gấp 3 lần prompt không nói gì. **Cảnh báo:** Đừng đầu tư model đắt nếu chưa làm chủ composition.

**2. FG/MG/BG là "thuốc tiên" chữa AI flat look**
Sau Day 10, Linh sẽ thấy 90% ảnh AI từ trước bị flat → vì thiếu foreground. Add 1 keyword `foreground bokeh` là khác hẳn.

**3. Symmetry là "stress test" cho model**
Cùng prompt symmetry, GPT Image 2 vs Seedream 4.5 vs NBN2 sẽ ra kết quả KHÁC NHAU rõ rệt về geometric precision. → Có thể Linh test thêm để so sánh.

**4. Negative Space đi ngược lại "AI nature"**
AI thích fill detail. Phải **chặn mạnh** bằng negative + low weight cho fill keywords.

**5. Combo composition: hơn 1 quy tắc/ảnh**
Quy tắc kinh điển: ảnh đẹp thường dùng **2-3 quy tắc cùng lúc**. Vd: Rule of Thirds + Leading Lines + FG/MG/BG → ảnh "siêu phẩm". Đừng giới hạn 1 quy tắc.

---

## 🎯 Thử thách hôm nay

### 🟢 Cho Newbie (15 phút, ~1,800 credit)
1. Test Rule of Thirds + Negative Space trên Seedream 4.5 (rẻ hơn): 1 chân dung Linh
2. So sánh 2 ảnh → cảm nhận khác biệt

### 🔵 Cho Intermediate (55 phút, ~13,500 credit)
1. Test full 15 ảnh trên GPT Image 2
2. Soi kỹ: GPT có làm Symmetry chuẩn không?
3. Đăng kết quả Facebook với hashtag `#Day10Composition`

### 🟣 Cho Pro (90 phút, ~20,000 credit)
1. Full 15 ảnh GPT + 15 ảnh Seedream 4.5 (cùng prompt) → so sánh
2. Tự design prompt **combo 3 quy tắc** cho 1 chủ đề Việt Nam khác
3. Viết review 500 từ về quy tắc nào "khó" nhất với AI

---

## 💬 Câu hỏi cho cộng đồng

Trong 5 quy tắc trên, **bạn thấy quy tắc nào hay bị AI làm sai nhất**?
- Mình đặt cược: **Symmetry** (do geometric precision yếu) hoặc **Negative Space** (do AI thích fill).

Comment cho mình biết — kết quả test có thể khác mình dự đoán!

---

## ❓ FAQ

**Q1: 5 quy tắc này có dùng được trên model rẻ như Seedream 4.5 không?**
**Có** — composition là **kỹ năng prompt**, không phụ thuộc model. Seedream 4.5 với prompt composition đúng có thể vượt GPT Image 2 prompt sơ sài. Test giả thuyết này ở Day 11+.

**Q2: Có phải mỗi ảnh chỉ dùng 1 quy tắc?**
**Không** — ảnh đẹp thường combo 2-3 quy tắc. Vd: Rule of Thirds + Leading Lines + FG/MG/BG cùng lúc.

**Q3: Cú pháp `(keyword:1.4)` có cần thiết cho composition không?**
**Có** — composition keyword hay bị AI "bỏ qua" nếu không weight. Recommend `(rule of thirds:1.4)`, `(symmetry:1.4)`.

**Q4: GPT Image 2 đắt 13,500 credit cho 15 ảnh — có đáng không?**
Tùy mục đích. Nếu Linh muốn **insight cho cộng đồng** → đáng (data thuần GPT có giá trị viral). Nếu chỉ học cho bản thân → Seedream 4.5 đủ (5,250 credit cho 15 ảnh).

**Q5: Foreground/Mid/Bg khác Bokeh thông thường thế nào?**
Bokeh chỉ là **kỹ thuật blur**, FG/MG/BG là **structure 3 lớp**. Bokeh có thể tồn tại trong cả 3 lớp. FG/MG/BG mới là composition.

**Q6: Nếu prompt 1 quy tắc nhưng AI không làm được, phải sao?**
3 cách fix:
1. Tăng weight: `(:1.4)` → `(:1.5)`
2. Mô tả cụ thể vị trí thay vì khái niệm chung
3. Đổi setting có sẵn quy tắc đó (vd: chọn chỗ có symmetry tự nhiên thay vì build)

**Q7: GPT Image 2 có tự thêm brand vào ảnh đồng hồ Day 10 không?**
**Khả năng cao** — Day 8 + Day 9 đều thấy. Mình đã thêm vào negative `Audemars, Vincero, Rolex, designer logo`. Sẽ verify sau khi test.

---

## 🎬 Recap & Day 11

### Ghi nhớ chính
- ✅ **5 quy tắc:** Rule of Thirds, Leading Lines, Symmetry, Negative Space, FG/MG/BG
- ✅ **Composition > Model** — kỹ năng prompt quan trọng hơn model đắt
- ✅ **FG/MG/BG = thuốc tiên** chống AI flat look
- ✅ **Symmetry là điểm yếu** của AI (geometric precision)
- ✅ **Negative Space đi ngược AI nature** — phải chặn mạnh fill
- ✅ Combo 2-3 quy tắc/ảnh = ảnh "siêu phẩm"

### 🔮 Day 11 — Sneak peek
Ngày mai mình deep dive **Lighting Mastery** — golden hour, blue hour, rim lighting, Rembrandt, split lighting... Học cách prompt từng kiểu lighting cụ thể. Spoiler: 70% ảnh AI bị "lighting trung tính" — fix bằng 1 từ khóa lighting cụ thể là khác hẳn!

---

## 📍 Navigation
[⬅️ Day 9: Prompt Engineering Nâng Cao](./day-09.md) | [🏠 README](../README.md) | [➡️ Day 11: Lighting Mastery](./day-11.md)

## 🏷️ Tags
`#0aiVN #Day10Linh0AI #Composition #RuleOfThirds #LeadingLines #Symmetry #NegativeSpace #ComposionAI #GPTImage2 #HoiAn #ThaoDien`

---

> **💌 Có ý kiến hoặc trải nghiệm khác?**
> Comment vào [bài Facebook Day 10](https://facebook.com/daclinh.tran) hoặc nhắn vào [Zalo group](https://zalo.me/g/umthmp096). Đặc biệt nếu bạn test thấy quy tắc nào AI làm tốt/tệ nhất → share để cộng đồng cùng học!

---

*Nhật ký Day 10 by **Linh0AI** — chuỗi 30 ngày làm chủ AI tạo ảnh & video trên 0ai.vn 🇻🇳*
