# Day 28 — Tổng kết Tuần 4 + Mini Challenge #3 "Video Việt Nam"

---

**[← Day 27: Cinema 70s "Cậu và Bơ"](./day-27.md)** · **[📚 Mục lục 30 ngày](../README.md)** · **[Day 29: Capstone Quảng cáo 30s →](./day-29.md)**

> **Level:** 🟣 Advanced (recap)
> **Thời lượng đọc:** 15-20 phút
> **Thực hành:** 60-180 phút (làm Mini Challenge video)
> **Cost:** 0K cho recap · ~30-150K nếu join Mini Challenge

---

## 🎯 Mục tiêu bài học

Sau 6 ngày Tuần 4 từ Seedance basics đến Cinema 70s narrative, hôm nay mình:

1. **Recap** 6 milestones — hệ thống hóa skills đã học
2. **Cheatsheet 1 trang** — Linh tổng hợp công thức Tuần 4 in được
3. **Launch Mini Challenge "Video Việt Nam"** — các bạn áp dụng tất cả skills vào project tự chọn

---

## 📚 Recap Tuần 4 — 6 milestones (Day 22-27)

### Day 22 — Intro Seedance 2.0 + Video AI Ecosystem

**Skill key:** First impression Seedance Omni 2.0 trên 0ai.vn

**Insights:**
- Seedance Omni 2.0 là model video flagship của 0ai.vn (ByteDance-developed, native Chinese understanding)
- Pricing: ~15-20K VND/segment (9:16 với refs), ~10-12K/segment (no refs)
- So sánh với VEO 3.1 Google + Kling 2.0 — Seedance win về cost + native CN, lose về duration cap

**Lesson:** Bắt đầu video AI cần budget 50-100K cho 1 week practice + accept rằng output không perfect lần đầu.

### Day 23 — Text-to-Video Cơ Bản

**Skill key:** Prompt video đầu tiên không cần ảnh ref

**Insights:**
- Prompt video phải có 5 elements: Subject + Action + Setting + Camera + Audio
- Duration default 5-15s, không request quá dài
- Style descriptors quan trọng: "cinematic", "documentary", "anime style"

**Lesson:** Text-to-video tốt cho concept exploration, KHÔNG đủ control cho production. Cần image refs.

### Day 24 — Image-to-Video Workflow

**Skill key:** Animate ảnh tĩnh thành video — pillar của VN creator pipeline

**Insights:**
- 1 ảnh đẹp + Seedance prompt = video 10-15s emotional
- Critical: ảnh nguồn phải sharp, không blur, đúng aspect
- Movement intensity setting trên 0ai.vn (low / medium / high)

**Lesson:** Đây là workflow phổ biến nhất audience VN — chụp ảnh phong cảnh, đưa lên Seedance, có video viral.

### Day 25 — Camera Movement Trong Video

**Skill key:** Pan / Zoom / Tracking / Dolly / Crane shots qua prompt

**Insights:**
- 6 camera moves verified work với Seedance:
  - Pan left/right (horizontal)
  - Tilt up/down (vertical)
  - Zoom in/out
  - Dolly in/out (move toward/away)
  - Tracking (follow subject)
  - Crane (overhead descent)
- ⭐ **Risk Matrix sneaker FIXED pattern** — khi prompt camera bị drift, anchor bằng specific brand/model name + "no other angles"

**Lesson:** Camera movement = 50% emotional impact video. "static shot" cinematic-grade khó hơn dynamic shot.

### Day 26 — Cinema Trailer 30s "Pháp phục lam"

**Skill key:** Multi-ref hybrid pattern + 8 shots Hollywood structure trong 30s

**Insights:**
- Multi-ref hybrid: 3 refs (Character + Style + Storyboard) đồng thời pass vào Seedance
- 8-shot structure Hollywood trailer: Hook → Build → Climax → Reveal
- Memorable Moment 5 conditions (single subject + static + duration unusual + small visual cue + dappled light)
- Cost: 76K VND cho 30s commercial-grade
- ⭐ Off-curriculum decision — mình pivot từ "Character consistency test" sang "production-ready trailer"

**Lesson:** Day 26 demonstrate commercial AI video production workflow. Cinema commercial khả thi 100% với <100K VND.

### Day 27 ⭐ — Cinema 70s Narrative "Cậu và Bơ"

**Skill key:** Phim ngắn narrative 70s với multi-age character (4 ages) + multi-stage dog (3 stages) + 2 era jumps + 2 cry-trigger moments

**Insights mới Day 27 (8 insights):**
1. **0ai.vn Seedance duration cap = 15s/segment** (verified)
2. **Filter #c455 "real person" trigger** — multi-age character sheet + detailed numerical ages + ethnic descriptors. Mitigation: descriptive aging words
3. **Storyboard text labels bleed vào video** — gibberish text trên báo/biển. Mitigation: "no readable text" + drop refs có text
4. **Single F1 multi-age sheet work cho 5 segments** — cost giảm 50% vs Day 26
5. **Hooded Figure VN-adapted (no skull/scythe)** pass compliance + audience comfort
6. **Multi-ref selective per segment** — không phải càng nhiều refs càng tốt
7. **CN prompt > EN cho cinematic VN context** — bonus VN signage authentic
8. **Seedance KHÔNG respect "TOTAL SILENCE"** — phải edit CapCut manual mute 6s

**Cost:** 140K VND cho 70s — efficient ratio 2.0K/s (giảm 20% vs Day 26 2.5K/s)

**Lesson:** Đỉnh kỹ thuật production của Tuần 4. Cinema narrative dài form khả thi với pure Seedance + CapCut + 140K VND.

---

## 📋 Cheatsheet 1 trang Tuần 4 — Video AI Production

### 🎬 Seedance Omni 2.0 specs (verified Day 27)

| Param | Value |
|---|---|
| Duration cap | **15s/segment** (KHÔNG quá) |
| Ratio support | 9:16 (vertical), 16:9 (horizontal), 1:1 (square) |
| Refs max | 3 refs đồng thời (`@image_1/2/3`) |
| Language | CN tốt nhất cho cinema VN context · EN OK cho commercial |
| Cost | 15-20K/segment có refs · 10-12K không refs |
| Filter | #c455 "real person" — soften age/ethnic descriptors |

### 🛠️ Pipeline 4 phases (cinema-grade)

```
Phase 1 — Foundation Images (3 ảnh, ~25K)
  ├─ Character sheet multi-age
  ├─ Props collection
  └─ Setting/Style reference

Phase 2 — Storyboards (3-5 ảnh, ~15-25K)
  ├─ Hand-drawn watercolor pattern
  ├─ 4-5 panels per board
  └─ Shot number + type + action labels

Phase 3 — Video segments (3-5 × 15s, ~50-100K)
  ├─ Path B: 5 segments × 15s = 75s raw
  ├─ Multi-ref hybrid (F1 + storyboard per segment)
  └─ CN prompts cho cinema, EN cho commercial

Phase 4 — CapCut edit (0K, free tool)
  ├─ Trim đầu/cuối lỗi
  ├─ Transitions (crossfade / match-cut / hard cut)
  ├─ Audio: BGM + SFX + silence drops manual
  └─ Color grade 2-era (warm past / cool present)
```

### ✍️ Prompt patterns verified

**Multi-ref hybrid (3 refs):**
```
@image_1 = Character/Dog reference
@image_2 = Props/Style reference
@image_3 = Storyboard shot order
```

**Soften filter #c455:**
- ❌ "30岁/45岁/55岁 Vietnamese man"
- ✅ "Middle-aged male protagonist with visible gray temples"

**Anti text bleed:**
- Front-load: "Absolutely no readable text, no subtitles, no signs"
- Drop refs có text headers

### 🎯 5 Conditions Memorable Moment (cry-trigger)

1. **Single subject** — chỉ 1 nhân vật/object trong frame
2. **Static camera** — không movement
3. **Duration unusual** — 4-6s held (vs avg 2-3s)
4. **Small visual cue** — single tear / leaf falling / candle flicker
5. **Dappled light** — gauze curtain shadow / sunlight pattern

### ❌ 5 Lỗi thường gặp Tuần 4

1. **Duration request > 15s** → output cap 15s automatic
2. **Multi-age character sheet detailed** → filter #c455 block
3. **Storyboard text labels** → bleed gibberish vào video
4. **"Total silence" prompt** → Seedance ignore, phải edit CapCut
5. **Background modern drift** → vintage era prompt + double avoid "no modern skyscrapers"

---

## ⚡ Mini Challenge #3 — "Video Việt Nam"

> **Launch:** Day 28 · **Deadline:** Day 29 · **Chấm:** Day 30 wrap

### 🎯 Brief

Các bạn áp dụng tất cả skills Tuần 4 vào 1 video AI mang đậm chất Việt Nam tự chọn theme.

### 🎬 Themes gợi ý

| # | Theme | Hook gợi ý |
|---|---|---|
| 1 | **Gia đình VN** | 3 thế hệ ăn cơm chiều · Bà nội kể chuyện · Tết sum vầy |
| 2 | **Quê hương** | Cánh đồng lúa chín · Chợ quê sáng sớm · Sông quê đò ngang |
| 3 | **Pet & companion** | Mèo nhà · Chó cỏ · Trâu nông dân |
| 4 | **Ẩm thực VN** | Phở sáng Hà Nội · Bún bò Huế · Bánh mì SG |
| 5 | **Festival VN** | Trung Thu · Tết · Lễ hội đền |
| 6 | **City vintage** | Sài Gòn 1990s · Hà Nội phố cổ · Đà Lạt thông |
| 7 | **Career/passion** | Nghệ nhân làng nghề · Họa sĩ phố cổ · Người bán hàng rong |

→ **Tự do chọn** hoặc combine 2-3 themes.

### 📐 Specs bắt buộc

- **Duration:** 30-60s
- **Ratio:** 9:16 vertical
- **Cry-trigger:** Ít nhất 1 moment emotional (Memorable Moment OR Final ECU)
- **VN authenticity:** Setting/prop/character mang dấu ấn VN rõ
- **Cost target:** <150K VND
- **Stack:** Bất kỳ tools — Seedance / Kling / Veo / mix

### 📤 Submission

- **Upload video** lên Drive/Dropbox/YouTube → share link
- **Caption ngắn:** Theme + 1 insight learned + cost actual
- **Tag:** #Linh0AI #VideoVN30Days
- **Submit vào:** [Nhóm Zalo](https://zalo.me/g/umthmp096) (recommend) hoặc GitHub Issues

**Deadline submit:** Hết ngày Day 29 (24h sau launch)

### 🏆 Reward

- **Top 3 work** mention + spotlight trong Day 30 wrap
- **Best emotional moment** đặc biệt — feature trên trang Facebook Linh0AI
- **Best cost-efficiency** (cheapest production high quality) — case study Day 30

---

## ➡️ Day 29 preview — Capstone Quảng cáo 30s

Day 29 sẽ là **case study quảng cáo 30s thực tế** cho 1 sản phẩm thật (Linh tự chọn hoặc community vote):

- **Workflow A-Z:** Brief client → Storyboard → Production → Edit → Deliver
- **10 ảnh storyboard + 5 video clip** ghép thành quảng cáo 30s
- **Cost target:** <100K VND (commercial-grade)
- **Deliverable:** Video sản phẩm có thể đăng FB/IG/TikTok bán hàng thật

Đây là project capstone — tổng hợp tất cả skills 28 ngày vào 1 deliverable monetizable.

---

## ➡️ Day 30 preview — Tổng kết 30 ngày + Roadmap

Day 30 sẽ là **wrap-up emotional** của hành trình 30 ngày:

- **Stats khóa học:** Tổng ảnh tạo · Tổng video · Cost actual · Insights collected
- **Top 10 tips không có ở tutorial nào khác** — bí kíp pro Linh đã verify
- **Chấm Mini Challenge "Video Việt Nam"** — Top 3 reveal
- **Roadmap tiếp theo:** Khóa 31-60 nếu có (audio production · multi-platform distribution · monetization)
- **Thank you community** + invite cộng đồng dài hạn

---

## 🚀 Sau Day 30? — Khóa 31+ tiềm năng

Tuần 4 đã master production. Nếu cộng đồng vote tiếp, mình có thể làm khóa 31-60 với 3 modules:

| Module | Topic |
|---|---|
| **Audio Production** | BGM cinematic · SFX layering · Voice-over Việt · Silence drops |
| **Distribution & Multi-Platform** | Adapt 9:16 / 16:9 / 1:1 · Hook A/B testing · Platform-specific algorithms |
| **Monetization & Creator Economy** | Freelance gig · Agency build · Creator fund · Brand partnership |

→ **Comment Zalo / Facebook nếu muốn khóa 31+!** Mình quyết định dựa vào demand thực tế cộng đồng.

---

## 📊 30 ngày recap nhanh (cho audience mới)

| Tuần | Skills | Output |
|---|---|---|
| **Tuần 1** (Day 1-7) | Foundation — Setup, Prompt anatomy, Aspect, EN/VN | ~85 ảnh |
| **Tuần 2** (Day 8-14) | Master Skills — Seedream + Prompt nâng cao + Composition + Lighting + Color + Camera | ~91 ảnh |
| **Tuần 3** (Day 15-21) | Image Workflows — I2I + Inpaint + Upscale + Style Transfer + Case Studies | ~50 ảnh |
| **Tuần 4** (Day 22-27) | Video AI — Seedance basics → Camera moves → Multi-ref → Cinema trailer 30s → Cinema 70s narrative | 6+ videos |

**Tổng:** 250+ ảnh + 6+ videos · ~80-150K VND total · 30+ insights verified

---

## 📎 Files đính kèm Day 28

Mini Challenge brief có trong file kèm. Cheatsheet 1 trang in được sẽ embed như image:

- [Cheatsheet Tuần 4 — Video AI Production](../assets/images/day-28-cheatsheet-tuan-4.png) (Linh tạo riêng nếu muốn)
- [Mini Challenge "Video Việt Nam" brief PDF](../assets/files/day-28-mini-challenge-brief.pdf) (optional)

---

**[← Day 27: Cinema 70s "Cậu và Bơ"](./day-27.md)** · **[📚 Mục lục 30 ngày](../README.md)** · **[Day 29: Capstone Quảng cáo 30s →](./day-29.md)**

---

*Day 28 hoàn thành — Tổng kết Tuần 4 + Launch Mini Challenge "Video Việt Nam"*
*Hành trình 30 ngày sắp kết thúc — còn 2 ngày cuối để cùng đi tới đích!*
