# Day 25 — Pipeline Practice 3 Ngành + Risk Matrix Verification

> Tuần 4 Day 4. Sau khi master pipeline image-to-video Day 24 (1 ad cà phê 15s), Day 25 là **practice session** với 3 briefs khác nhau để verify pipeline universal. Đặc biệt: **test image-to-video có FIX được branded products issue** (Day 22 sneaker fail) — đây là **scientific verification** của Risk Matrix Tuần 4.

---

## Mục tiêu bài học

Sau bài này, các bạn sẽ:

- Áp dụng pipeline storyboard-to-video cho 3 ngành khác nhau (Fashion / Beauty / Wellness)
- Verify image-to-video FIX được vấn đề branded products (Day 22 sneaker fail pattern)
- Master 2 patterns prompt Seedance Omni 2.0 mới: "Anti-grid output" + "Strict panel order"
- Distribute VFX combo 2-per-brief (không nhồi tất cả VFX trong 1 video)
- Compliance VN cho wellness/health products (no medical claims)

## Output cuối bài

- 3 storyboards 4x4 (16 panels mỗi cái) — GPT Image 2
- 3 videos × 15s — Seedance Omni 2.0 image-to-video
- 4 insights mới verified cho khóa học Tuần 4

---

## Phần 1 — Vì sao 3 briefs khác nhau?

Day 24 mình verified pipeline với 1 brief cà phê (LOW risk, F&B). Câu hỏi mở:

- Pipeline có work cho **branded fashion** (HIGH risk theo Risk Matrix Day 22)?
- Pipeline có work cho **beauty** với skin texture authentic?
- Pipeline có work cho **wellness products** mà không vi phạm regulation VN?

Day 25 chọn 3 briefs target từng câu hỏi:

| Brief | Industry | Risk Matrix Day 22 | Mục đích test |
|-------|----------|---------------------|---------------|
| **Sneaker high-end** | Fashion branded | 🔴 HIGH risk (text-to-video FAIL) | Image-to-video CÓ FIX được không? |
| **Serum dưỡng da** | Beauty generic | 🟢 LOW risk | Pipeline work cho beauty với natural skin? |
| **Trà thảo mộc** | Wellness | 🟢 LOW risk | Compliance VN có dễ apply? |

→ 3 briefs cover 3 cases khác nhau, không duplicate Day 24.

---

## Phần 2 — Workflow tổng pipeline Day 25

Sync với Day 24 nhưng input đổi từ **9 keyframes rời** sang **1 storyboard 4x4 grid**:

```
Day 24 pattern:                Day 25 pattern:
─────────────────             ─────────────────
9 keyframes rời                1 storyboard 4x4 (16 panels)
        │                              │
        ▼                              ▼
3 phân cảnh × 3 @image refs    1 @image1 = storyboard grid
        │                              │
        ▼                              ▼
3 videos × 15s                  1 video × 15s
```

**Lý do dùng pattern Day 25 (single grid):**
- Cost thấp hơn (1 storyboard vs 9 keyframes = ~900 vs ~8K)
- Composition planning rõ hơn (16 panels visualize toàn bộ 15s)
- Verified Day 19 pattern (short film) — giờ apply commercial

**Trade-off:**
- Mất character consistency (vì không có Character Master riêng làm reference)
- Phù hợp cho **product-focused ads** (không nhân vật anchor) hơn

→ 3 briefs Day 25 đều **product-focused** (sneaker / serum bottle / tea cup) — pattern phù hợp.

---

## Phần 3 — 2 Patterns Prompt Mới cho Seedance Omni 2.0

Day 24 mình verified template 11 section Day 22 cho image-to-video commercial. Day 25 add **2 patterns mới** xử lý storyboard 4x4 input:

### Pattern A — Anti-grid output (Sneaker)

```
@image1 仅作为分镜结构、镜头节奏、构图方向和视觉氛围参考。
不要把@image1直接生成成storyboard拼图，不要出现grid、panel边框、
分镜线、文字、编号、拼贴效果。
```

**Dùng khi:** Storyboard 4x4 chỉ là **reference structure**, model có flexibility tạo narrative theo phase-based.

**Phù hợp:** Briefs có scene transitions phức tạp (studio → urban → studio cho sneaker), không strict panel-by-panel.

### Pattern B — Strict panel order (Serum + Wellness tea)

```
必须严格按照@image1的分镜顺序执行：从左到右、从上到下，依次推进，
不得跳镜，不得省略开头分镜，不得打乱顺序。
```

**Dùng khi:** Cần model **follow exact panel order** của storyboard, mỗi panel = 1 micro moment.

**Phù hợp:** Briefs có narrative tuyến tính (drop → bottle → application → hero cho serum).

**Combined với 16 panels description explicit:**

Mỗi panel 1-16 có description riêng:

```
Panel 1: 极近景，滴管头部形成一滴淡金色精华液...
Panel 2: 极近景，液滴被拉长下坠，慢动作...
...
Panel 16: Final hero shot...右侧与上方留干净空间，方便后期添加CTA文字
```

→ Model có **1-1 mapping** với storyboard, không bị guess.

### Quy tắc chọn pattern

| Brief type | Recommend pattern |
|------------|-------------------|
| Multi-scene transitions (studio + outdoor + indoor) | **A — Anti-grid output** |
| Single-scene tuyến tính narrative | **B — Strict panel order** |
| Product-focused minimal motion | **B — Strict panel order** |
| Character-focused dynamic action | **A — Anti-grid output** |

---

## Phần 4 — 3 Storyboards Kết quả Thực tế

### 🎨 Storyboard 1 — Sneaker High-End

![Storyboard Sneaker](https://github.com/linhai-creator/linh0ai-daily-tutorials/raw/main/assets/images/day-25-storyboard-sneaker.png)

**Layout 16 panels:**
- Hàng 1 (Panels 1-4): Hook macro detail — đế giày / mesh / dây giày / gót pad
- Hàng 2 (Panels 5-8): Product reveal — Studio 3/4 với line lights
- Hàng 3 (Panels 9-12): **Levitation VFX** — Giày bay với halo backlight
- Hàng 4 (Panels 13-16): Urban tracking + hero ending

**Quality:** ✅ Excellent. Tone dark + neon accent cohesive. KHÔNG có brand logo bịa (fix Day 22 sneaker fail pattern).

### 🎨 Storyboard 2 — Serum Dưỡng da

![Storyboard Serum](https://github.com/linhai-creator/linh0ai-daily-tutorials/raw/main/assets/images/day-25-storyboard-serum.png)

**Layout 16 panels:**
- Hàng 1 (Panels 1-4): Hook **slow-mo drop** — Pipette → drop → landing → ripple
- Hàng 2 (Panels 5-8): Product reveal — Bottle marble với light scan
- Hàng 3 (Panels 9-12): Application — Drop on skin → spread → texture
- Hàng 4 (Panels 13-16): Use case + hero ending

**Quality:** ✅ Excellent. Marble + cream + gold tone signature beauty premium. Skin texture **NATURAL không over-smooth** (Panel 12) — fix Day 22 Beauty anti-pattern.

### 🎨 Storyboard 3 — Trà Thảo Mộc Wellness

![Storyboard Wellness Tea](https://github.com/linhai-creator/linh0ai-daily-tutorials/raw/main/assets/images/day-25-storyboard-wellness-tea.png)

**Layout 16 panels:**
- Hàng 1 (Panels 1-4): Hook **particle effects** — Hoa cúc bay với sunlight rays
- Hàng 2 (Panels 5-8): Product reveal — Tách trà với steam + golden hour
- Hàng 3 (Panels 9-12): **Slow-mo pour** — Pour macro với swirl + leaves
- Hàng 4 (Panels 13-16): Use case + hero ending

**Quality:** ✅ Excellent. Organic warm tone. NO medical hint, NO doctor — chỉ wellness lifestyle drink.

**Cost 3 storyboards:** ~2,700 VND (3 × ~900).

---

## Phần 5 — 3 Videos Kết quả Thực tế

### 🎬 Video 1 — Sneaker High-End (15s)

[![Sneaker thumbnail](https://github.com/linhai-creator/linh0ai-daily-tutorials/raw/main/assets/images/day-25-video-sneaker-thumbnail.jpg)](https://github.com/linhai-creator/linh0ai-daily-tutorials/raw/main/assets/videos/day-25-video-sneaker-15s.mp4)
> 👆 Click thumbnail để xem video MP4 (15s, ~6MB) — **Risk Matrix Day 22 sneaker fail FIXED**

**Highlight frames:**

| Time | Mô tả |
|------|-------|
| 0s | Split-screen macro (sole + mesh) — Hook dramatic |
| 6s | Medium 3/4 sneaker dark studio + line lights blue |
| 10s | **Levitation VFX** với light rays + smoke — VFX moment đỉnh |
| 14s | Hero shot dark background, right side clean cho text CTA |

**Honest assessment:**

| Aspect | Day 22 sneaker (text-to-video) | Day 25 sneaker (image-to-video) |
|--------|-------------------------------|--------------------------------|
| Brand logo bịa | ❌ Render "BIOTOR" trên giày | ✅ KHÔNG có logo bịa |
| Brand swap giữa scenes | ❌ NB → ASICS giữa video | ✅ Cùng 1 design xuyên suốt |
| Frankenstein effect | ❌ 2 chiếc khác nhau cùng frame | ✅ Single shoe cohesive |
| VFX Levitation quality | ⚠️ OK nhưng bị logo conflict | ✅ Levitation cinematic premium |

→ **Risk Matrix Day 22 sneaker fail FIXED bởi image-to-video pipeline.** Đây là insight verified quan trọng nhất Tuần 4.

### 🎬 Video 2 — Serum Dưỡng da (15s)

[![Serum thumbnail](https://github.com/linhai-creator/linh0ai-daily-tutorials/raw/main/assets/images/day-25-video-serum-thumbnail.jpg)](https://github.com/linhai-creator/linh0ai-daily-tutorials/raw/main/assets/videos/day-25-video-serum-15s.mp4)
> 👆 Click thumbnail để xem video MP4 (15s, ~6MB) — **Clean beauty với skin texture authentic**

**Highlight frames:**

| Time | Mô tả |
|------|-------|
| 0s | Macro slow-mo droplet ở dropper tip với sparkle stars — Hook đỉnh |
| 4s | Bottle hero trên marble với golden light rays — Product reveal |
| 8s | Drop landing trên hand skin, natural texture không over-smooth |
| 14s | Hero ending bottle với marble + sunlight rays, right side clean |

**Honest assessment:**

- ✅ Slow-mo macro signature đẹp cinematic
- ✅ Light scan trên chai consistent qua các frames
- ✅ Skin texture NATURAL không bị "plastic feel" (đã prompt `保留真实毛孔，不要塑料感`)
- ✅ Marble + cream + gold tone signature
- ✅ NO medical hint, NO doctor, NO brand logo

### 🎬 Video 3 — Trà Thảo Mộc Wellness (15s)

[![Wellness Tea thumbnail](https://github.com/linhai-creator/linh0ai-daily-tutorials/raw/main/assets/images/day-25-video-wellness-tea-thumbnail.jpg)](https://github.com/linhai-creator/linh0ai-daily-tutorials/raw/main/assets/videos/day-25-video-wellness-tea-15s.mp4)
> 👆 Click thumbnail để xem video MP4 (15s, ~6MB) — **Compliance VN wellness ad**

**Highlight frames:**

| Time | Mô tả |
|------|-------|
| 0s | Particle hoa cúc bay với sunlight rays — Hook particle VFX đỉnh |
| 6s | Tách trà với steam + golden hour + lá thảo mộc visible |
| 12s | Cô gái uống trà nhắm mắt smile mãn nguyện, natural wellness moment |
| 14s | Hero ending với rays + steam + lá thảo mộc decorate |

**Honest assessment:**

- ✅ Particle effects (frame 0) đẹp natural — hoa cúc bay realistic
- ✅ Steam + golden hour atmospheric (frame 6, 14)
- ✅ NO medical claim, NO doctor — chỉ wellness lifestyle drink
- ✅ Compliance VN respect: pattern này safe cho **thực phẩm chức năng, trà thảo mộc, nước uống organic**

**Cost 3 videos:** ~108,000 VND (3 × 36K).

---

## Phần 6 — 4 Insights Mới Verified ở Day 25

### Insight 1: Storyboard 4x4 → Seedance video pattern UNIVERSAL cho commercial

Day 19 verified pattern này cho short film (animation). Day 25 verify cho **3 industries commercial khác nhau**:

| Industry | Brief | Pattern work? |
|----------|-------|---------------|
| Fashion branded | Sneaker | ✅ PASS |
| Beauty generic | Serum | ✅ PASS |
| Wellness drink | Trà thảo mộc | ✅ PASS |

→ Pattern **Storyboard 4x4 → Seedance image-to-video** universal cho commercial production.

### Insight 2: Risk Matrix Day 22 — Branded Products FIXED 🎯

**Đây là insight quan trọng nhất Tuần 4.**

Day 22 đã document Risk Matrix với 4 tests (cost 144K data thực):

| Category | Text-to-video result |
|----------|---------------------|
| F&B (cà phê) | ✅ PASS |
| Beauty generic (serum) | ✅ PASS |
| Street food (bánh mì) | ✅ PASS |
| **Branded fashion (sneaker)** | ❌ **FAIL** — logo bịa + brand swap + Frankenstein |

Day 25 test **image-to-video pipeline** cho cùng category HIGH risk (sneaker):

| Test approach | Result |
|---------------|--------|
| Day 22 text-to-video | ❌ FAIL (3 issues) |
| Day 25 image-to-video (storyboard 4x4 ref) | ✅ **PASS** — clean, no brand logo bịa, premium VFX |

→ **Verified hypothesis:** Image-to-video với keyframe/storyboard reference **fix được branded products issue** mà text-to-video không làm được.

**Implication cho khóa học:** Học viên nhận job ad branded products (sneaker shop, brand nhỏ VN) → **bắt buộc** dùng pipeline image-to-video, không dùng text-to-video.

### Insight 3: 2 Prompt patterns cho Seedance Omni 2.0 với @image1 = storyboard

Day 25 phát triển 2 patterns prompt tiếng Trung mới:

**Pattern A — Anti-grid output:**
```
@image1 仅作为分镜结构...参考。
不要把@image1直接生成成storyboard拼图，不要出现grid、panel边框...
```

**Pattern B — Strict panel order:**
```
必须严格按照@image1的分镜顺序执行：从左到右、从上到下...
不得跳镜，不得省略开头分镜，不得打乱顺序。
```

→ Cộng với 16 panels descriptions explicit, model có **1-1 mapping** với storyboard. Pattern này extends Master Template 11-section Day 22.

### Insight 4: Compliance VN cho Wellness products work seamlessly

Quảng cáo wellness/health VN bị regulate chặt (Luật Quảng cáo 2012). Day 25 test prompt explicit:

```
不要任何医疗暗示、治愈、药效暗示
不要医生、药剂师、白大褂
不要药瓶包装
```

→ Output Video 3 (wellness tea) **clean** — không có medical hint, không có doctor, không có pharmacy bottle. Pattern này áp dụng được cho:
- Trà thảo mộc
- Nước uống organic
- Wellness drinks
- Beauty supplements (cẩn thận hơn)

→ Học viên nhận job ad **thực phẩm chức năng** safe với pattern này.

---

## Phần 7 — VFX Combo Distribution

Day 25 demo cách **distribute 2 VFX/brief** thay vì nhồi tất cả VFX trong 1 video:

| Brief | VFX Signature | Lý do |
|-------|---------------|-------|
| **Sneaker** | Levitation + Light scan | Premium urban fashion — dramatic + dynamic |
| **Serum** | Slow-mo macro + Light scan | Clean beauty — clinical + premium |
| **Wellness tea** | Particle effects + Slow-mo pour | Organic natural — peaceful + cinematic |

**Quy tắc:**
- 2 VFX/brief tối đa, không nhồi 4 VFX
- Mỗi VFX chiếm 1 phase rõ ràng (vd: Hook = particle, Benefit = slow-mo)
- VFX phải match brand identity (luxury fashion ≠ organic wellness)

**Trade-off với "nhồi tất cả VFX":**

| Approach | Pros | Cons |
|----------|------|------|
| Combo 2/brief (Day 25) | Mỗi VFX execution clean, brand identity rõ | Mỗi video không "wow" tất cả VFX |
| Nhồi tất cả VFX | "Showcase" technical capability | Video bị overload, brand identity lẫn lộn |

→ Day 25 chọn **Combo 2/brief** — production-ready cho commercial real, không phải showcase demo.

---

## Phần 8 — Lỗi thường gặp khi practice pipeline với brief mới

**Skip storyboard, gen video trực tiếp.** Mỗi brief cần storyboard 4x4 trước để model có composition reference. Skip = video bị random composition.

**Dùng tiếng Anh prompt Seedance.** Day 19-22 đã verify tiếng Trung hiệu quả hơn. Day 25 sync pattern.

**Quên section 【参考图像】.** Nếu không direct model cách dùng storyboard (anti-grid output HOẶC strict panel order), model có thể render lỗi.

**Nhồi tất cả VFX trong 1 video.** Vi phạm quy tắc Day 22 "1 shot = 1 action chính". Distribute 2 VFX/brief.

**Skip compliance check cho wellness/health products.** VN regulation chặt — bịa medical claim = vi phạm Luật Quảng cáo 2012 + Nghị định 54/2017.

**Force pipeline image-to-video cho mọi brief.** F&B generic (cà phê / bánh mì / trà) text-to-video đã PASS Day 22 — không cần image-to-video. Chỉ dùng image-to-video cho HIGH risk (branded products).

---

## Bài tập thực hành

Chọn 1 brief của riêng bạn (sản phẩm shop, dịch vụ, brand nhỏ) và áp dụng pipeline Day 25:

**Bước 1 — Brief + Risk assessment:**
- Sản phẩm có branded logo cần lock? → HIGH risk, dùng image-to-video
- Sản phẩm generic (F&B, beauty no-brand)? → LOW risk, có thể text-to-video Day 22

**Bước 2 — Storyboard 4x4 (GPT Image 2):**
- Tiếng Việt prompt với 16 panels match 5-phase kịch bản 15s
- Ratio 16:9 horizontal
- Cost ~900 VND

**Bước 3 — Video Seedance Omni 2.0:**
- Tiếng Trung prompt với 1 trong 2 patterns (Anti-grid output / Strict panel order)
- @image1 = storyboard từ Bước 2
- Cost ~36K VND

**Bước 4 — Review honest:**
- Brand logo có lock không?
- Skin texture / liquid state / character consistency OK?
- CTA frame có clean space cho text overlay?
- VFX signature match brand identity?

---

## Tiêu chí đạt bài

- [ ] 1 storyboard 4x4 generated với 16 panels match kịch bản 15s
- [ ] 1 video 15s từ storyboard với Seedance image-to-video
- [ ] Áp dụng đúng 1 trong 2 prompt patterns (Anti-grid / Strict panel order)
- [ ] VFX distribute 2/brief, không nhồi
- [ ] Compliance check (no medical claims cho wellness/health)
- [ ] CTA frame có space cho text overlay

---

## Cost summary Day 25

| Item | Cost |
|------|------|
| 3 storyboards × ~900 | ~2,700 VND |
| 3 videos Seedance × 36K | ~108,000 VND |
| **Tổng Day 25** | **~110,700 VND** |

→ Day 25 cost similar Day 24 (~116K). Output: 3 ads commercial từ 3 ngành khác nhau, ready cho portfolio.

---

## Sang Day 26

Day 26 sẽ là **Rough cut & Edit phase** — ghép Day 24 + Day 25 ads thành **portfolio packages**:

- Audio mixing (3 layers BGM/VO/SFX từ Day 23)
- Text overlay (typography + timing từ Day 23)
- Color grading + final export
- Multi-platform versions (9:16 TikTok / 16:9 YouTube / 1:1 Instagram)

Sau Day 26, các bạn có **4 ads commercial production-ready** cho portfolio freelance:
- 1 cà phê (Day 24)
- 1 sneaker (Day 25)
- 1 serum (Day 25)
- 1 wellness tea (Day 25)

---

## 📍 Navigation

[⬅️ Day 24: Storyboard + Keyframe + Image-to-Video](https://github.com/linhai-creator/linh0ai-daily-tutorials/blob/main/days/day-24.md) | [🏠 README](https://github.com/linhai-creator/linh0ai-daily-tutorials/blob/main/README.md) | [➡️ Day 26: Rough Cut + CapCut Edit](https://github.com/linhai-creator/linh0ai-daily-tutorials/blob/main/days/day-26.md)

---

## 🏷️ Tags

#0aiVN #Day25Linh0AI #PipelinePractice #Storyboard4x4 #ImageToVideo #SeedanceOmni #RiskMatrixVerified #BrandedProductsFixed #ComplianceVN #VFXCombo #Tuan4

---

*Linh0AI Daily Tutorials — Day 25/30 (83%) Tuần 4 Day 4: 3 storyboards + 3 videos × 15s (Fashion + Beauty + Wellness) + 4 insights mới verified (storyboard 4x4 universal / Risk Matrix sneaker FIXED / 2 prompt patterns / Compliance VN seamless) + 110K VND cost actual*
