# Day 24 — Storyboard Thương mại & Keyframe + Video Generation

> Tuần 4 Day 3. Sau khi có brief + kịch bản 15s (Day 22) và 5 craft knowledge (Day 23), Day 24 là **full pipeline pre-production** cho 1 ad cà phê commercial — từ 9 keyframes GPT Image 2 đến 3 videos Seedance image-to-video. Đây là bài kết hợp ảnh tĩnh + video động trong 1 ngày.

---

## Mục tiêu bài học

Sau bài này, các bạn sẽ:

- Hiểu sự khác biệt giữa storyboard thương mại (Day 24) và storyboard 4x4 animation (Day 18)
- Tạo được 4 loại Master Images cho commercial production (Character / Product / Scene / Shot Keyframes)
- Áp dụng workflow image-to-video multi-reference với Seedance Omni 2.0
- Sản xuất full pipeline 1 ad cà phê 15s từ keyframe đến video

## Output cuối bài

- 9 keyframes (1 Character Master + 1 Product Master + 1 Scene Master + 6 Shot Keyframes)
- 3 videos × 15s = 45s raw để Day 26 ghép trong CapCut
- 1 set prompts tiếng Việt cho GPT Image 2 + 3 prompts tiếng Trung cho Seedance Omni 2.0

> 📋 **Prompts đầy đủ trong bài**: [`prompts/day-24-prompts.txt`](../prompts/day-24.txt)
> Copy/download nguyên văn về paste vào 0ai.vn — không phải gõ lại từ trong bài.

---

## Phần 1 — Storyboard Thương mại vs Storyboard 4x4 Day 18

Day 18 mình đã làm storyboard 4x4 cho short film "Đôi Kiếm Tiên" — 16 panels grid với motion lines + action notes + camera direction. Đây là pattern **animation production**.

Storyboard thương mại Day 24 khác hoàn toàn:

| Aspect | Day 18 (Animation) | Day 24 (Commercial) |
|--------|--------------------|--------------------|
| Số panels | 16 panels grid 4x4 | 5-8 panels rời |
| Mục đích | Action choreography | Product showcase + brand moment |
| Composition | Dynamic, motion lines | Static, clean, polished |
| Anchor | Character sheet (1 master) | 3 masters (Character + Product + Scene) |
| Pacing | Beat-by-beat narrative | Hook → Product → Benefit → Emotion → CTA |
| Input cho video | 1 grid image làm reference | Mỗi keyframe = 1 reference riêng |

**Quy tắc khác biệt quan trọng:** Storyboard commercial **KHÔNG upload grid 4x4 làm input video** — mỗi keyframe phải là **ảnh rời độc lập** để dùng làm @image reference cho Seedance image-to-video.

---

## Phần 2 — 4 loại Master Images

Pre-production commercial cần 4 loại ảnh:

### 1. Character Master

Ảnh nhân vật chuẩn — outfit, hair, face cố định. Là anchor cho mọi shot có nhân vật xuất hiện.

Trong Day 24 mình dùng nhân vật **Lan, barista 28 tuổi** — face oval, skin warm brown, hair black low ponytail, tạp dề beige + áo trắng.

### 2. Product Master

Ảnh sản phẩm chuẩn — shape, color, state cố định. Là anchor cho mọi shot có product.

Ly cà phê sữa đá Việt Nam — glass thủy tinh trong, cà phê nâu đậm + sữa, đá viên, condensation drops.

### 3. Scene Master

Ảnh bối cảnh chuẩn — mood, lighting, color palette. **KHÔNG có người, KHÔNG có sản phẩm chính** — chỉ là environment reference cho consistency tone.

Quán cafe Sài Gòn ấm cúng — quầy gỗ, đèn thả hổ phách, plants, ánh sáng warm morning.

### 4. Shot Keyframes (5-8 ảnh)

Ảnh từng shot trong kịch bản — đã có pose + product + composition cụ thể. Mỗi keyframe = 1 reference riêng cho Seedance image-to-video.

Day 24 này có 6 shot keyframes match 5 thành phần kịch bản Day 22 (Hook → Product → Benefit → Emotion → CTA).

---

## Phần 3 — Workflow GPT Image 2: 9 Keyframes

### Setup chung

| Tham số | Giá trị |
|---------|---------|
| Model | GPT Image 2 (trên 0ai.vn) |
| Ratio | 9:16 dọc (cho TikTok/Reels native) |
| Resolution | Medium 2K |
| Language | **Tiếng Việt thuần** (Day 16 đã verify GPT Image 2 hiểu tốt) |
| Cost | 9 × ~900 = ~8,100 VND |

### Thứ tự generate

1. **Character Master** Lan TRƯỚC — làm anchor cho Shot 2 và Shot 4
2. **Product Master + Scene Master** độc lập
3. **Shot 1, 3, 5, 6** (không có Lan) — standalone
4. **Shot 2, 4** (có Lan) — upload Character Master làm `@image1` để giữ consistency

Prompts cụ thể cho 9 keyframes nằm trong `day-24-prompts.txt` Phần A.

### 9 Keyframes thực tế (đã generate)

**Character Master — Lan barista:**

![Character Master Lan](https://github.com/linhai-creator/linh0ai-daily-tutorials/raw/main/assets/images/day-24-character-master-lan.png)

**Product Master + Scene Master:**

| Product Master | Scene Master |
|----------------|--------------|
| ![Product Master](https://github.com/linhai-creator/linh0ai-daily-tutorials/raw/main/assets/images/day-24-product-master-coffee.png) | ![Scene Master](https://github.com/linhai-creator/linh0ai-daily-tutorials/raw/main/assets/images/day-24-scene-master-cafe.png) |

**6 Shot Keyframes (match kịch bản Day 22):**

| Shot | Time | Phase | Keyframe |
|------|------|-------|----------|
| 1 | 0-3s | Hook | ![Shot 1](https://github.com/linhai-creator/linh0ai-daily-tutorials/raw/main/assets/images/day-24-shot-1-keyframe-hook-macro.png) |
| 2 | 3-6s | Product prep (Lan rót) | ![Shot 2](https://github.com/linhai-creator/linh0ai-daily-tutorials/raw/main/assets/images/day-24-shot-2-keyframe-lan-pouring.png) |
| 3 | 6-10s | Benefit (macro swirl) | ![Shot 3](https://github.com/linhai-creator/linh0ai-daily-tutorials/raw/main/assets/images/day-24-shot-3-keyframe-macro-swirl.png) |
| 4 | 10-13s | Emotion (Lan cười) | ![Shot 4](https://github.com/linhai-creator/linh0ai-daily-tutorials/raw/main/assets/images/day-24-shot-4-keyframe-lan-smile.png) |
| 5 | 13-14s | Hero product | ![Shot 5](https://github.com/linhai-creator/linh0ai-daily-tutorials/raw/main/assets/images/day-24-shot-5-keyframe-product-hero.png) |
| 6 | 14-15s | CTA final (top space) | ![Shot 6](https://github.com/linhai-creator/linh0ai-daily-tutorials/raw/main/assets/images/day-24-shot-6-keyframe-cta-final.png) |

### Đánh giá honest 9 keyframes

**Strengths:**

- **Lan consistency XUẤT SẮC** — Character Master vs Shot 2 (Lan rót) vs Shot 4 (Lan cười) face/outfit/tóc gần như identical. @image1 reference workflow PASS.
- **Tone warm cohesive** across all 9 images
- **Quality 9:16 vertical** đẹp cinematic
- **Không có brand logo / text bịa**
- **Cost ~8,100 VND đúng dự kiến**

**Limitations:**

- **Image Shot 1 (Hook macro):** Model interpret "macro" thành medium close-up full glass, không phải "extreme macro" giọt nước đơn lẻ như prompt yêu cầu. Acceptable nhưng không hoàn toàn match design.
- **Ly cà phê có slight variation** giữa các shots: cao/thấp/layer khác nhau. Generic style commercial acceptable nhưng không lock 100%.
- **Scene cafe khác** giữa Scene Master (3 đèn hổ phách rõ) và các shots khác (do mỗi shot không upload Scene Master làm reference).

→ 9 keyframes đủ quality làm input cho Day 25 video generation.

---

## Phần 4 — Workflow Seedance Image-to-Video

### Setup chung

| Tham số | Giá trị |
|---------|---------|
| Model | Seedance 2.0-Omni (image-to-video mode) |
| Ratio | 16:9 horizontal (1280×720) |
| Duration | 15s/video |
| Language | **Tiếng Trung** (Day 19-22 đã verify) |
| Cost | 3 × 15s × 2,400 = ~108,000 VND |

### Cách chia 9 keyframes → 3 phân cảnh × 3 references

Match kịch bản cà phê 15s Day 22 (Hook → Product → Benefit → Emotion → CTA):

| Phân cảnh | Narrative | 3 References |
|-----------|-----------|--------------|
| **1 — Establishment + Hook** | Wide quán cafe → zoom macro → product reveal | Scene Master + Shot 1 + Product Master |
| **2 — Production (Lan pha cà phê)** | Lan tại quầy → Lan rót → macro swirl | Character Master + Shot 2 + Shot 3 |
| **3 — Emotion + CTA** | Lan cười → product hero → CTA final | Shot 4 + Shot 5 + Shot 6 |

Mỗi phân cảnh = 1 prompt Seedance Omni 2.0 tiếng Trung 11-section + 3 @image references → 1 video 15s.

### Quan trọng: Ratio 9:16 vs 16:9

Day 24 keyframes là **9:16 dọc** (TikTok/Reels native). Nhưng Seedance Omni 2.0 trong test này render **16:9 horizontal**.

→ Khi chuyển ratio, **prompt design phải adapt** theo ratio mới, không chỉ thay từ `9:16 竖屏` thành `16:9 横屏`. Đặc biệt là CTA frame layout (top 1/3 cho 9:16 ≠ right 1/3 cho 16:9).

Đây là insight quan trọng — chi tiết ở Phần 6.

---

## Phần 5 — 3 Videos kết quả thực tế

### 🎬 Scene 1 — Establishment + Hook (15s)

[![Scene 1 thumbnail](https://github.com/linhai-creator/linh0ai-daily-tutorials/raw/main/assets/images/day-24-video-scene-1-thumbnail.jpg)](https://github.com/linhai-creator/linh0ai-daily-tutorials/raw/main/assets/videos/day-24-video-scene-1-establishment-hook-15s.mp4)
> 👆 Click thumbnail để xem video MP4 (15s, ~6MB) — **Establishment + Product reveal**

**Highlight frames:**

| Time | Mô tả |
|------|-------|
| 0s | Wide quán cafe với ly cà phê visible trên bàn round bên phải |
| 2s | Camera tiếp tục show wide cafe với ly stable |
| 6s | Medium close-up ly cà phê centered, background cafe blur |
| 14s | Hero ending — ly cà phê centered trên bàn gỗ |

**Honest assessment:**

- ✅ **FIXED bug "materialize"** từ test trước — ly visible từ frame 0 nhờ prompt `不要突然出现`
- ✅ Wide cafe + product reveal smooth transition
- ⚠️ Ly cà phê **shape variation** giữa các phase (low → tall) — chưa lock 100%
- ⚠️ Scene cafe background **drift slight** giữa các phase

### 🎬 Scene 2 — Production / Lan pha cà phê (15s)

[![Scene 2 thumbnail](https://github.com/linhai-creator/linh0ai-daily-tutorials/raw/main/assets/images/day-24-video-scene-2-thumbnail.jpg)](https://github.com/linhai-creator/linh0ai-daily-tutorials/raw/main/assets/videos/day-24-video-scene-2-lan-production-15s.mp4)
> 👆 Click thumbnail để xem video MP4 (15s, ~6MB) — **Scene EXCELLENT — Lan consistency + smooth action**

**Highlight frames:**

| Time | Mô tả |
|------|-------|
| 0s | Lan đứng quầy cafe, smile thân thiện, setup bình cà phê + ly đá |
| 4s | Lan rót cà phê đậm vào ly có đá — action chính, motion smooth |
| 8s | Top-down macro: sữa hòa vào cà phê đậm, swirl realistic không abstract |
| 14s | Lan look down vào ly cà phê hoàn thành, satisfied smile — bookend |

**Honest assessment:**

- ✅ **Lan consistency XUẤT SẮC** — face/outfit/hair stable từ frame 0 → 14
- ✅ **Action sequence smooth**: setup → pour → swirl → completion
- ✅ **Macro swirl realistic** — đẹp natural fluid, không "abstract pattern" như prompt cảnh báo
- ✅ **Tay natural**, không warp, không extra fingers
- ⚠️ Signboard text bịa "Coffin Robo / COFFEE" trên menu board — minor, model render text trên signboards là phổ thông cho cafe context

→ **Scene 2 quality cao nhất trong 3 videos.** Đây là proof concept cho image-to-video pipeline work với human action commercial.

### 🎬 Scene 3 — Emotion + CTA (15s) — version 1

[![Scene 3 thumbnail](https://github.com/linhai-creator/linh0ai-daily-tutorials/raw/main/assets/images/day-24-video-scene-3-thumbnail.jpg)](https://github.com/linhai-creator/linh0ai-daily-tutorials/raw/main/assets/videos/day-24-video-scene-3-emotion-cta-15s.mp4)
> 👆 Click thumbnail để xem video MP4 (15s, ~6MB) — **CTA frame cần re-gen (ratio issue)**

**Highlight frames:**

| Time | Mô tả |
|------|-------|
| 0s | Lan giữ ly cà phê, microsmile, background cafe đẹp |
| 6s | Transition: focus shift Lan → product hero |
| 10s | Product hero shot centered trên bàn gỗ |
| 14s | CTA final frame — ly cà phê centered, top space có clock + lamps + arches |

**Honest assessment:**

- ✅ Lan consistency từ Scene 2
- ✅ Transition Lan → product smooth
- ✅ Product hero shot premium
- 🔴 **CTA frame top space KHÔNG clean** — có clock, multiple lamps, arches, architecture details → khó add text CTA overlay

**Root cause vấn đề Scene 3:**

Prompt designed cho 9:16 vertical (`上方 1/3 到 1/2 留白` = top 1/3 cho text). Nhưng render 16:9 horizontal — top 1/3 horizontal khác hoàn toàn về aspect, model fill bằng architectural elements thay vì clean blur.

→ **Lesson:** Ratio change KHÔNG simple swap. Prompt designed cho 9:16 phải redesign khi chuyển 16:9 — đặc biệt là CTA layout.

**Fix approach (cho test 2):**

Update prompt Scene 3:
- Đổi header `9:16 竖屏` → `16:9 横屏`
- CTA layout: ly cà phê **bên trái**, **right 1/3 clean** (thay vì top)
- Anti-pattern explicit: cấm clock, lamps, arches ở right side

Test 2 sẽ re-gen Scene 3 với layout mới (+36K VND).

---

## Phần 6 — 3 Insights quan trọng từ Day 24

### Insight 1: Multi-reference image-to-video pipeline WORK

Seedance Omni 2.0 image-to-video với 3 @image references work tốt cho production commercial. Scene 2 (Lan pha cà phê) đặc biệt thành công — Character Master + Action keyframe + Detail macro combine smooth thành 1 narrative 15s.

→ **Pattern reusable** cho mọi ad commercial có nhân vật + sản phẩm + chi tiết.

### Insight 2: Anti-pop-in instruction WORK cho image-to-video

Scene 1 test trước (mình đã viết) bị bug "ly materialize từ frame 0 → 2s" — ly hiện từ không có.

Scene 1 test này (Linh viết) FIXED bằng `不要突然出现` explicit trong section 3-6s. → **Anti-pop-in instruction explicit hiệu quả** chống bug materialize.

→ Quy tắc mới cho image-to-video commercial: **luôn ghi explicit "product visible from frame 0"** trong section đầu tiên.

### Insight 3: Ratio change KHÔNG simple swap

Day 24 keyframes 9:16, render Seedance 16:9 → prompt design 9:16 không transfer cleanly sang 16:9. Đặc biệt CTA layout:

| Layout | 9:16 (vertical) | 16:9 (horizontal) |
|--------|----------------|--------------------|
| CTA text position | Top 1/3 trống | Right 1/3 trống |
| Subject position | Bottom 2/3 | Left 1/3-2/3 |
| Anti-pattern | "Top không có vật cản" | "Right không có clock/lamps/arch" |

→ Khi chuyển ratio, **redesign prompt cho ratio mới**, không chỉ thay `9:16 竖屏` thành `16:9 横屏`.

---

## Phần 7 — Lỗi thường gặp khi làm pipeline keyframe → video

**Skip Character Master, generate keyframes riêng.** Mỗi shot có Lan khác mặt khác outfit → consistency fail. Always generate Character Master FIRST, sau đó dùng làm @image1 cho mọi shot có nhân vật.

**Upload storyboard grid 4x4 làm @image cho Seedance.** Sai pattern. Storyboard 4x4 là animation reference (Day 18). Commercial cần keyframe rời từng shot. Seedance interpret grid sẽ cố render multiple panels trong 1 video → fail.

**Prompt video bằng tiếng Việt.** Day 19-22 đã verify: Seedance hiểu tiếng Trung tốt hơn nhiều. Prompts Day 24 video phải tiếng Trung 11-section template Day 22.

**Skip lock liquid state.** Coffee, smoothie, juice không lock "稳定状态" → liquid evolve giữa các phase (insight Day 22 coffee test). Add `已经混合好的稳定状态` cho mọi liquid product.

**Ratio mismatch.** Keyframes 9:16, render video 16:9 mà không adapt prompt → composition fail (như Scene 3 CTA frame). Hoặc render same ratio với keyframes, hoặc redesign prompt cho ratio mới.

**Generate hết 9 keyframes 1 lần.** Nếu Character Master không như ý → mọi shot có Lan đều fail. **Luôn generate Character Master TRƯỚC, review OK rồi mới generate Shot 2 và Shot 4** dùng làm reference.

---

## Bài tập thực hành

Áp dụng pipeline Day 24 vào brief riêng của mình:

**Bước 1 — Pre-production planning (theo Day 22-23):**
- Có brief Creative Brief + Kịch bản 15s
- Quyết approach: single-clip Seedance HOẶC multi-shot 3 phân cảnh

**Bước 2 — Generate 4 loại Master Images (GPT Image 2):**
- 1 Character Master (nếu có nhân vật)
- 1 Product Master
- 1 Scene Master
- 5-8 Shot Keyframes

**Bước 3 — Generate 3 videos image-to-video (Seedance Omni 2.0):**
- Chia keyframes thành 3 phân cảnh × 3 references
- Prompt tiếng Trung 11-section template Day 22
- Cost: ~108K VND

**Bước 4 — Review honest:**
- Lan/character consistency OK không?
- Product shape lock không?
- Liquid state stable không?
- CTA frame có clean space cho text overlay không?

Nếu shot nào fail → re-gen với prompt tweak (cost 36K mỗi re-gen).

---

## Tiêu chí đạt bài

- [ ] 1 Character Master generated, quality cao
- [ ] 1 Product Master generated, quality cao
- [ ] 1 Scene Master generated, quality cao
- [ ] 5-8 Shot Keyframes generated với consistency
- [ ] 3 videos × 15s từ Seedance image-to-video
- [ ] Mỗi video lock được consistency core (nhân vật/sản phẩm/scene)
- [ ] CTA frame có clean space cho text overlay (top hoặc side tùy ratio)

---

## Cost summary Day 24

| Item | Cost |
|------|------|
| 9 keyframes GPT Image 2 | ~8,100 VND |
| 3 videos Seedance Omni 2.0 (test 1) | ~108,000 VND |
| **Tổng Day 24 (test 1 hoàn chỉnh)** | **~116,100 VND** |
| (Optional) Re-gen Scene 3 v2 với CTA fix | +36,000 VND |
| **Tổng nếu re-gen Scene 3** | **~152,100 VND** |

→ Day 24 là **bài đầu tư cao nhất Tuần 4** vì sản xuất full pipeline 1 ad commercial. Output là 3 videos sẵn sàng cho Day 26 ghép CapCut thành ad final.

---

## Sang Day 25

Day 25 là **bài tập thực hành pipeline khác** — học viên áp dụng workflow Day 24 với 1 brief khác (serum / bánh mì / sneaker / brief của mình). Mục đích: consolidate kỹ năng + verify pipeline universal cho nhiều ngành.

Sau Day 25, các bạn sẽ có **2 ads commercial production-ready** từ cùng pipeline → portfolio piece cho freelance work.

---

## 📍 Navigation

[⬅️ Day 23: 5 Craft Knowledge cho Ad AI 15s](https://github.com/linhai-creator/linh0ai-daily-tutorials/blob/main/days/day-23.md) | [🏠 README](https://github.com/linhai-creator/linh0ai-daily-tutorials/blob/main/README.md) | [➡️ Day 25: Pipeline Practice 3 Ngành + Risk Matrix Verification](https://github.com/linhai-creator/linh0ai-daily-tutorials/blob/main/days/day-25.md)

---

## 🏷️ Tags

#0aiVN #Day24Linh0AI #Storyboard #Keyframe #ImageToVideo #SeedanceOmni #CharacterMaster #ProductMaster #MultiReferencePipeline #CommercialProduction #Tuan4

---

*Linh0AI Daily Tutorials — Day 24/30 (80%) Tuần 4 Day 3: Full pipeline 9 keyframes + 3 videos × 15s + 3 insights mới (multi-ref work, anti-pop-in fix, ratio change rule) + 116K VND cost actual*
