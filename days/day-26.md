# Day 26 — Cinema-Style 30s Trailer: 2 Videos × 15s + 7 Câu Hỏi Strategic Framework

> Tuần 4 Day 5. Sau khi master pipeline practice 3 ngành Day 25 (feature reel 15s product-focused), Day 26 tiến lên **cinema-style storytelling**: 30 giây tổng chia 2 videos × 15s với cliffhanger ending + memorable moment. Đây không phải feature reel "show sản phẩm đẹp" mà là **emotional narrative bán cảm xúc về sản phẩm**. Test case: pháp phục lam Phật tử — sản phẩm high-emotion (hiếu thảo, tâm linh, gia đình) mà feature reel 15s không cover hết được story arc.

---

## Mục tiêu bài học

Sau bài này, các bạn sẽ:

- Phân biệt được **Cinema-style 30s** vs **Feature reel 15s** — chọn đúng format theo sản phẩm
- Master **7 câu hỏi strategic framework** universal cho mọi commercial brief (commercial agency thinking)
- Áp dụng pipeline **6 prompts** cho cinema trailer (Character Sheet + Product Master + 2 Storyboards + 2 Videos)
- Master **multi-ref hybrid pattern** kết hợp Day 24 (multi-ref keyframes) + Day 25 (storyboard grid)
- Fix **duplicate person bug** khi Seedance Omni 2.0 confuse Character Sheet với multi-character instruction
- Avoid **visual prior bias** khi gen Storyboard sequel
- Workflow **CapCut Hybrid edit** — manual merge + AI music sync để preserve cinematic story arc

## Output cuối bài

- 1 Character Sheet turnaround (2 nhân vật × 3 views) — GPT Image 2
- 1 Product Master flat lay — GPT Image 2
- 2 Storyboards 4×2 (8 panels mỗi cái) — GPT Image 2 với multi-ref
- 2 Videos × 15s — Seedance Omni 2.0 image-to-video với multi-ref hybrid
- 1 Video final 30s đã edit CapCut với nhạc + CTA — production-ready ad
- 6 insights mới verified cho khóa học Tuần 4

---

## 📄 Prompt file

Tất cả prompt tiếng Việt + tiếng Trung dùng trong Day 26 được lưu trong:

**[`prompts/day-26-prompts.txt`](https://github.com/linhai-creator/linh0ai-daily-tutorials/blob/main/prompts/day-26-prompts.txt)** (595 lines, 6 prompts đầy đủ)

Cấu trúc file:

- **Phần A — Master References** (Prompt 1-2): Character Sheet + Product Master — tiếng Việt cho GPT Image 2
- **Phần B — Storyboards** (Prompt 3-4): 2 storyboards 4×2 với multi-ref — tiếng Việt cho GPT Image 2
- **Phần C — Video Prompts** (Prompt 5-6): 2 videos Seedance Omni 2.0 — tiếng Trung 11-section template (mỗi prompt < 5000 ký tự để vừa Seedance input)
- **GHI CHÚ**: Workflow tổng 10 bước + Cost breakdown + Compliance VN + Tips music/CTA

Copy nguyên văn từng prompt vào 0ai.vn theo thứ tự để reproduce kết quả.

---

## Phần 1 — Vì sao Cinema-Style 30s, không phải Feature Reel 15s?

Day 24-25 mình đã verified pipeline cho **feature reel 15s** — format "show sản phẩm đẹp" với cấu trúc Hook → Reveal → VFX → Use case → CTA. Format này work tốt cho **product-focused ads**: cà phê, sneaker, serum, trà thảo mộc. Audience hiểu nhanh "đây là cái gì, nó tốt vì sao".

Nhưng có **một loại sản phẩm mà feature reel 15s KHÔNG cover được story arc**:

| Loại sản phẩm | Format phù hợp | Lý do |
| --- | --- | --- |
| F&B generic, fashion basic, beauty basic | **Feature reel 15s** | Audience care về tính năng — show feature là đủ |
| Gift cho người thân, tâm linh, hiếu thảo, kỷ niệm | **Cinema-style 30s** | Audience care về cảm xúc — feature reel không bán được "lý do tặng" |
| B2B luxury, real estate, đám cưới | **Cinema-style 30s+** | Cần build trust + emotion + transformation |

**Đặc điểm sản phẩm Day 26 (pháp phục lam Phật tử) yêu cầu cinema-style:**

- Không bán "vải lam giá rẻ" — bán **bình an** của người đeo
- Không bán "may thủ công" — bán **hiếu thảo** của người tặng
- Audience không decide mua trong 15s — họ cần **resonate emotional** mới sẵn sàng commit

→ Feature reel 15s pháp phục: "Áo dài tay rộng, vải cotton mềm, may thủ công Huế, giá X" = audience scroll qua. **Cinema-style 30s pháp phục**: "Con gái thấy mẹ áo cũ sờn → quyết định may áo mới → mẹ peaceful rưng rưng dưới bồ đề" = audience dừng lại, cảm xúc lên tới đỉnh, sẵn sàng inquiry.

### Tại sao chia 2 videos × 15s thay vì 1 video 30s?

3 lý do platform-driven và 1 lý do storytelling-driven:

**1. Platform constraints Facebook/Instagram:**

Facebook Feed ads ưu tiên video ≤ 15s (skip rate giảm 40% so với 30s+). Nhưng 15s không đủ kể full story arc cảm xúc. Solution: 2 videos × 15s riêng biệt, có thể serve sequential trong cùng campaign hoặc cross-post (Video 1 lên Reels, Video 2 lên Stories).

**2. Seedance Omni 2.0 max duration 15s:**

Mỗi clip Seedance gen tối đa 15s. Nếu muốn 30s liên tục cinema phải ghép 2 clips. Cấu trúc 15s + 15s với cliffhanger ending tạo natural break point.

**3. A/B testing dễ:**

Có thể test Video 1 hook hiệu quả nhất, hoặc Video 2 CTA chuyển đổi nhất, mỗi cái independent. Nếu 1 video 30s liền thì khó isolate yếu tố nào work.

**4. Cliffhanger storytelling (storytelling-driven):**

Đây là technique từ Hollywood trailer convention — **2-act trailer structure**. Video 1 build tension đến climax → cut ngang → audience tò mò "rồi sao". Video 2 deliver payoff. Cấu trúc này hoạt động hiệu quả hơn 1 video 30s flow vì:

- Audience xem Video 1 tự nhiên muốn xem Video 2 (open loop psychology)
- 15s là sweet spot attention span — xem hết Video 1 không skip
- Khi ghép thành 30s cho landing page, vẫn có cảm giác "trailer" cao hơn 1 đoạn dài flow

→ **Day 26 chốt format: 2 videos × 15s, ghép thành 30s cinema trailer.**

---

## Phần 2 — 7 Câu Hỏi Strategic Framework

Trước khi viết brief / prompt / kịch bản, mỗi commercial production agency chuyên nghiệp đều trả lời 7 câu hỏi này. Day 26 explicit hóa framework để các bạn áp dụng cho **mọi brief tương lai**.

### Câu 1 — TRANSFORMATION: Customer trước và sau khi dùng sản phẩm khác nhau thế nào?

Đây là **xương sống** của cinema-style ads. Không có transformation = không có story.

Day 26 pháp phục lam:

- **Trước:** Mẹ Hương 52 tuổi mặc pháp phục lam cũ sờn → không nói ra nhưng audience cảm nhận được sự cô đơn, thiếu thốn, hoặc "mẹ đã già rồi, áo cũng cũ theo"
- **Sau:** Mẹ mặc pháp phục lam mới tinh khôi → peaceful, hạnh phúc, rưng rưng dưới bồ đề

→ Transformation **visible** trên screen, không cần text giải thích.

**Lỗi thường gặp:** Ads "before/after" của shop nhỏ thường chỉ show sản phẩm xuất hiện trong tay khách. Đó không phải transformation — đó là delivery. Transformation phải show **trạng thái cảm xúc của customer thay đổi**.

### Câu 2 — ENEMY: Kẻ thù của customer là gì?

Mọi câu chuyện cần kẻ thù (con người, hoàn cảnh, hoặc nội tâm). Audience care vì họ có cùng kẻ thù.

Day 26: Kẻ thù = **thời gian + sự lãng quên hiếu thảo**. Mẹ mặc áo cũ vì:
- Mẹ không muốn tốn tiền cho mình (sacrificing)
- Con gái mải làm việc/học hành, không để ý
- Áo cũ là dấu hiệu của thời gian trôi qua, mẹ đã già

Audience target (con gái/con trai 18-35 tuổi) **immediately resonate** vì hầu hết đều có guilt "mình chưa quan tâm bố mẹ đủ".

**Pattern generalize:**

| Sản phẩm | Kẻ thù |
| --- | --- |
| Pháp phục (Day 26) | Sự lãng quên hiếu thảo + thời gian trôi qua |
| Skincare anti-aging | Thời gian + so sánh với phụ nữ khác |
| Khóa học online | Sự ổn định việc làm + áp lực thu nhập |
| Tủ lạnh inverter | Tiền điện + thực phẩm hỏng |
| Đồ chơi trẻ em | Thời gian quý ở nhà + phát triển kỹ năng con |

### Câu 3 — EMOTIONAL STAKES: Tại sao audience phải care?

Stakes là **cost của không hành động**. Audience care nếu họ cảm thấy "nếu mình không làm gì, có thể sẽ tiếc".

Day 26: Stakes = **mẹ có thể không còn lâu nữa**. Câu này không bao giờ được nói thẳng trong video — nhưng dappled light qua bồ đề + mẹ tóc bạc + áo sờn = visual cues làm audience tự cảm nhận. Audience nhận ra "mình phải làm cái gì đó cho mẹ, ngay bây giờ".

**Quy tắc:** Stakes phải **implied bằng visual**, không spoken. Nếu phải nói "thời gian không đợi" = brief failure.

### Câu 4 — HOOK: 3 giây đầu thu hút bằng gì?

Hook là **3 giây đầu video** quyết định audience scroll qua hay dừng lại. Hook hiệu quả thường thuộc 1 trong 4 loại:

1. **Visual stunning** — composition đẹp lạ (Day 25 sneaker macro split-screen)
2. **Pattern interrupt** — frame unusual với thường ngày (Day 26 Panel 1 sân chùa empty sunbeam rays)
3. **Question-raising** — frame làm audience hỏi "đây là gì / sẽ ra sao" (Day 26 Panel 1 không có người = "ai sẽ xuất hiện?")
4. **Emotional shock** — frame chứa cảm xúc cao trào (Day 26 không dùng — vì memorable moment ở giữa, không ở đầu)

Day 26 chọn **mix Loại 1 + 2 + 3**: Wide sân chùa cổ Việt Nam với sunbeam rays xuyên qua bồ đề, không có người. Vừa stunning vừa raise question vừa pattern interrupt (Facebook feed thường full người + sản phẩm).

### Câu 5 — MEMORABLE MOMENT: Frame nào audience sẽ nhớ?

Đây là câu hỏi khó nhất + quan trọng nhất.

**Quy tắc industry:** Mỗi commercial cần 1 frame mà audience nhớ ngay cả khi đã tắt video. Apple ads luôn có 1 frame mới mọi người sẽ nhớ (silhouette dancer iPod, tear drop screen iPhone X). Nike "Just Do It" có frame Bo Jackson cross-training. Coca-Cola có frame Santa.

Day 26 Memorable Moment = **Panel 12 — Mẹ peaceful rưng rưng dưới bồ đề (3 giây static)**.

Để thiết kế Memorable Moment, áp dụng 5 conditions:

1. **Single subject focus** — không có distraction trong frame (chỉ mẹ, không có con An)
2. **Static camera** — không movement, audience focus 100% vào cảm xúc
3. **Duration unusual** — 3 giây dài hơn các panels khác (1-2s) → audience "có thời gian" cảm
4. **Small visual cue** — 1 giọt nước mắt ở khóe mắt (KHÔNG rơi xuống má — đó là crying, không phải moved)
5. **Dappled light** — natural environmental light pattern thêm cinematic depth

→ Frame mẹ Hương 52 tuổi, nhắm mắt nhẹ, mỉm cười peaceful, 1 giọt nước mắt rưng rưng, dappled light bồ đề chiếu trên mặt, đứng cạnh cây bồ đề lớn = **cry-trigger moment**.

Frame này là **xương sống** của cả 30s trailer. Nếu Panel 12 fail → cả trailer fail dù 15 panels khác đẹp.

### Câu 6 — TRUST: Bằng chứng đáng tin gì?

Audience emotional rồi nhưng vẫn cần lý do logic để purchase. Trust signal trong cinema commercial thường là:

- **Craftsmanship close-up** (bàn tay thợ may đang khâu)
- **Material origin** (vải cotton Huế truyền thống)
- **Time spent** (may 3 ngày thủ công)
- **Heritage proof** (xưởng may 30 năm)

Day 26: Panel 14 — Extreme close-up macro bàn tay người thợ may Việt Nam đang khâu kim chỉ tỉ mỉ trên áo lam. Audience thấy:
- Tay nhăn nheo tuổi trung niên (kinh nghiệm)
- Đường kim chỉ tỉ mỉ (chất lượng)
- Background xưởng may truyền thống (heritage)

→ 2 giây Panel 14 thay thế cho 100 chữ "made by hand in Hue".

### Câu 7 — ACTION: CTA cụ thể là gì?

CTA không chỉ là số điện thoại. CTA hiệu quả gồm 3 thành phần:

1. **What** — Sản phẩm/dịch vụ tên gì?
2. **Why** — Lý do mua (đặc biệt là gì)?
3. **How** — Cách hành động (SĐT/link/inbox)?

Day 26 CTA: `PHÁP PHỤC LAM HUẾ / May thủ công · Vải cotton mềm / Đặt may: 0XXX.XXX.XXX`

→ 3 dòng cover what + why + how trong 1 giây Panel 16.

> 💡 **Trong video demo bài giảng**, mình dùng SĐT placeholder `0XXX.XXX.XXX`. Khi các bạn áp dụng cho shop thật, thay bằng SĐT/Zalo/link landing page thực tế.

---

**Tóm tắt 7 câu hỏi cho mọi brief tương lai:**

| # | Câu hỏi | Day 26 pháp phục lam |
| --- | --- | --- |
| 1 | TRANSFORMATION trước/sau? | Mẹ áo cũ cô đơn → mẹ áo mới peaceful rưng rưng |
| 2 | ENEMY của customer? | Lãng quên hiếu thảo + thời gian trôi |
| 3 | EMOTIONAL STAKES? | Mẹ có thể không còn lâu nữa |
| 4 | HOOK 3s đầu? | Wide sân chùa sunbeam rays, không có người |
| 5 | MEMORABLE MOMENT? | Panel 12 mẹ rưng rưng peaceful 3s static |
| 6 | TRUST signal? | Panel 14 macro tay thợ may Huế khâu kim chỉ |
| 7 | ACTION CTA? | Tên shop + đặc trưng + SĐT |

→ 7 câu hỏi này áp dụng cho **mọi commercial brief** (ad sản phẩm, dịch vụ, brand). Trả lời được 7 câu = brief production-ready.

---

## Phần 3 — Workflow Tổng Pipeline 6 Prompts

Day 24 dùng 9 keyframes riêng + 3 video clips. Day 25 dùng 1 storyboard grid + 1 video. Day 26 kết hợp **best of both worlds**:

```
Day 24 pattern:               Day 25 pattern:               Day 26 pattern (NEW):
─────────────────             ─────────────────             ─────────────────
9 keyframes rời                1 storyboard 4x4              Character + Product
                                                            + 2 Storyboards 4x2
        │                              │                              │
        ▼                              ▼                              ▼
Multi-ref 3 @image refs       Single ref @image1            Multi-ref hybrid:
per scene                                                   Storyboard + Character
                                                            + Product
        │                              │                              │
        ▼                              ▼                              ▼
3 videos × 15s                 1 video × 15s                 2 videos × 15s
(commercial reel)              (commercial reel)             (cinema trailer)
```

### Pipeline 6 prompts Day 26 chi tiết:

**Phần A — Master References (gen 1 lần, dùng xuyên suốt):**

- **Prompt 1** — Character Sheet turnaround: Mẹ + Con cùng 1 ảnh, 2 hàng × 3 cột = 6 views
- **Prompt 2** — Product Master: Pháp phục lam flat lay product photography

**Phần B — Storyboards (gen 2 lần với multi-ref):**

- **Prompt 3** — Storyboard Video 1 "TRƯỚC": 4×2 = 8 panels, story arc Setup + Confrontation
- **Prompt 4** — Storyboard Video 2 "SAU": 4×2 = 8 panels, story arc Resolution + Trust + CTA

**Phần C — Videos (gen 2 lần với multi-ref hybrid):**

- **Prompt 5** — Video 1 Seedance: 15s "TRƯỚC" với cliffhanger ending
- **Prompt 6** — Video 2 Seedance: 15s "SAU" với memorable moment + CTA frame

### Reference chain:

```
Prompt 1 (Character Sheet) ──┐
                             ├──→ Prompt 3 (Storyboard 1) ──┐
Prompt 2 (Product Master) ──┤                               │
                             ├──→ Prompt 4 (Storyboard 2)   │
                             │                              │
                             ├──→ Prompt 5 (Video 1) ───────┘ (3 refs)
                             │
                             └──→ Prompt 6 (Video 2) ─────── (3 refs)
```

→ **Character + Product master làm foundation cho 4 prompts sau**. Skip 2 master này = identity drift xuyên video.

### Cost dự kiến:

| Prompt | Cost |
| --- | --- |
| Prompt 1 — Character Sheet | ~900 VND |
| Prompt 2 — Product Master | ~900 VND |
| Prompt 3 — Storyboard 1 | ~900 VND |
| Prompt 4 — Storyboard 2 | ~900 VND |
| Prompt 5 — Video 1 Seedance | ~36,000 VND |
| Prompt 6 — Video 2 Seedance | ~36,000 VND |
| **Tổng** | **~75,600 VND** |
| Buffer re-gen 20% | ~15,000 VND |
| **Total budget** | **~91,000 VND** |

→ Day 26 cost tương đương Day 25 (~110K) nhưng output là **cinema trailer 30s** thay vì 3 feature reels 15s.

---

## Phần 4 — Story Arc 3-Act + 16 Panels Breakdown

Cinema storytelling theory chuẩn từ Hollywood: **Three-act structure**.

- **Act 1 — Setup** (25% thời lượng): Giới thiệu nhân vật + bối cảnh + status quo
- **Act 2 — Confrontation** (50% thời lượng): Conflict xuất hiện, character phải decide
- **Act 3 — Resolution** (25% thời lượng): Decision dẫn đến transformation

Day 26 apply cho 30s trailer:

```
Video 1 "TRƯỚC" (15s):
├─ Act 1 Setup (0-6s, Panels 1-4): Mẹ trong sân chùa, áo lam cũ
└─ Act 2 Confrontation (6-15s, Panels 5-8): Con thấy → áy náy → quyết định → CLIFFHANGER

Video 2 "SAU" (15s):
└─ Act 3 Resolution (15-30s, Panels 9-16): Mẹ nhận → mặc → ⭐ peaceful → trust → CTA
```

### Breakdown 16 panels chi tiết:

**Video 1 "TRƯỚC" — Act 1 Setup (Panels 1-4):**

**Panel 1 (0-2s, Wide sân chùa cổ bình minh):** Establishing shot sân chùa cổ Việt Nam buổi sáng. Mái ngói rêu phong, cổng tam quan, cây bồ đề lớn. Sunbeam rays xuyên qua tán bồ đề. **Không có người**. → Pattern interrupt + question-raising hook.

**Panel 2 (2-4s, Mẹ chắp tay cầu nguyện):** Medium shot mẹ Hương 52 tuổi đứng chắp tay cầu nguyện, mặc pháp phục lam **CŨ sờn**. Background mái ngói + bồ đề soft focus. → Establishes character (mẹ) + place (sân chùa) + status quo (peaceful but worn).

**Panel 3 (4-5s, Macro áo sờn close-up):** Macro extreme close-up tay áo pháp phục lam **CŨ** trên cánh tay mẹ. Vải bạc màu, mép vải xơ rách. Ngón tay nhăn nheo tuổi 50+. → **Detail shot trigger empathy** — audience nhận ra áo cũ rồi, mẹ già rồi.

**Panel 4 (5-6s, Wide mẹ dưới bồ đề):** Wide cinematic mẹ đứng đơn độc dưới cây bồ đề lớn. Mẹ small trong frame, dappled light pattern trên sân. → **Cô đơn beat** — mẹ một mình dù trong sân chùa lớn.

**Video 1 "TRƯỚC" — Act 2 Confrontation (Panels 5-8):**

**Panel 5 (6-8s, Con từ xa nhìn mẹ):** Medium shot An 19 tuổi đứng góc sân chùa, bị cột gỗ tam quan che một phần thân. An nhìn về phía mẹ đang cầu nguyện, ánh mắt áy náy. → **Introduce character thứ 2** — con gái xuất hiện, conflict bắt đầu.

**Panel 6 (8-10s, Close-up mắt con áy náy):** Extreme close-up đôi mắt An, nước mắt rưng rưng khóe mắt (không khóc). Ánh phản chiếu mờ trong mắt có thể là hình ảnh mẹ. → **Emotional climax setup** — con cảm thấy đỉnh điểm áy náy.

**Panel 7 (10-13s, Tay con gấp áo mới):** Close-up macro tay An gấp pháp phục lam **MỚI tinh khôi**. Bên cạnh có lá bồ đề + chuỗi hạt gỗ. Ánh sáng natural cửa sổ. → **Decision beat** — con quyết định hành động, dấu hiệu visible đầu tiên của transformation.

**Panel 8 (13-15s, Con quyết tâm CLIFFHANGER):** Medium shot An đứng dậy cầm hộp pháp phục đã gói, ánh mắt quyết tâm hướng về phía cửa. Low angle camera. **Mẹ KHÔNG xuất hiện trong frame**. → **Cliffhanger** — audience tò mò "mẹ sẽ phản ứng sao?".

**Video 2 "SAU" — Act 3 Resolution (Panels 9-16):**

**Panel 9 (15-17s, Mẹ nhận hộp áo):** Medium shot mẹ ngồi bên bàn gỗ, vẫn mặc áo lam **CŨ** (continuity), nhận hộp từ tay An (chỉ thấy tay An ở mép frame). Mẹ ngạc nhiên xúc động. → **Payoff cliffhanger** — đáp lại curiosity từ Panel 8.

**Panel 10 (17-20s, Mẹ mặc pháp phục mới):** Medium shot mẹ đứng trong phòng ngủ Việt Nam (giường gỗ + cửa sổ), đã mặc pháp phục lam **MỚI** tinh khôi. Đang chỉnh cổ áo. → **Transformation visible** — áo mới đã trên người mẹ.

**Panel 11 (20-22s, Mẹ ngắm mình):** Medium close-up mẹ trước gương gỗ truyền thống. Tay vuốt nhẹ ngực áo lam mới, mắt rưng rưng nhẹ nhìn xuống. → **Emotional buildup** — chuyển từ trang trọng sang xúc động.

**Panel 12 (22-25s, ⭐ MEMORABLE MOMENT):** **Đỉnh cảm xúc.** Medium portrait mẹ Hương mặc pháp phục lam mới đứng cạnh bồ đề. Nhắm mắt nhẹ, mỉm cười peaceful, 2 hàng nước mắt rưng rưng đọng ở khóe mắt (không rơi xuống má). Dappled light xanh lá bồ đề trên mặt. **Camera static 3 giây**. → **Cry-trigger moment** — frame audience nhớ lâu nhất.

**Panel 13 (25-26s, Wide bồ đề mẹ peaceful):** Wide cinematic mẹ mặc áo mới đứng peaceful dưới bồ đề. Mẹ small trong frame, bối cảnh hùng vĩ. → **Resolution visual** — mẹ đã viên mãn trong bối cảnh trang nghiêm.

**Panel 14 (26-28s, Tay thợ may Huế):** Extreme close-up macro bàn tay thợ may trung niên đang khâu kim chỉ tỉ mỉ trên áo lam. Background xưởng may truyền thống. → **TRUST signal** — bằng chứng craftsmanship.

**Panel 15 (28-29s, Mẹ + Con peaceful cạnh nhau):** Medium shot mẹ + An đứng cạnh nhau trước cổng tam quan. Mẹ peaceful nhìn xa, An hơi cúi đầu hiền hậu, tay An đặt nhẹ trên tay mẹ. → **Family unity beat** — relationship transformed.

**Panel 16 (29-30s, CTA frame):** Medium wide mẹ + An peaceful trước cổng tam quan. CTA text overlay bottom 1/3 frame. → **Call to action** — thông tin shop để inquiry.

### Pacing analysis:

| Panel | Duration | Pace | Mục đích |
| --- | --- | --- | --- |
| 1 | 2s | Standard | Establish |
| 2 | 2s | Standard | Character |
| 3 | 1s | Quick | Detail trigger |
| 4 | 1s | Quick | Emotion beat |
| 5 | 2s | Standard | Character 2 |
| 6 | 2s | Standard | Emotional climax |
| 7 | 3s | Slow build | Decision |
| 8 | 2s | Standard | Cliffhanger |
| 9 | 2s | Standard | Payoff |
| 10 | 3s | Slow build | Transformation |
| 11 | 2s | Standard | Build to climax |
| **12** | **3s** | **EXTENDED** | **⭐ Memorable** |
| 13 | 1s | Quick | Resolution wide |
| 14 | 2s | Standard | Trust |
| 15 | 1s | Quick | Family unity |
| 16 | 1s | Quick | CTA |

→ **Pacing rule:** Memorable Moment Panel 12 là **panel duy nhất** giữ 3s extended duration. Tất cả các panels khác 1-2-3s standard pace.

→ **Tổng:** 8 panels × 2s trung bình + Panel 12 extended = 30s.

---

## Phần 5 — Multi-Ref Strategy Hybrid

Day 26 evolution của multi-ref pattern từ Day 24 + Day 25:

### Day 24 multi-ref pattern (verified):

```
Mỗi clip Seedance: 3 @image refs riêng biệt
- @image1 = Character Master
- @image2 = Product Master
- @image3 = Scene Keyframe
```

**Rule Day 24:** "Không upload grid 4×4 trong multi-ref single-clip" — vì grid 4×4 = 16 panels nhỏ, AI confuse khi kết hợp với refs khác.

### Day 25 single-ref grid pattern (verified):

```
Mỗi clip Seedance: 1 @image1 = Storyboard 4×4
Không kèm refs khác
```

**Rule Day 25:** Storyboard 4×4 chứa đủ visual info (character + product + scene), không cần multi-ref.

### Day 26 hybrid pattern (NEW — verify Day 24 rule boundary):

```
Mỗi clip Seedance: 3 @image refs
- @image1 = Storyboard 4×2 (8 panels — nhỏ hơn 4×4)
- @image2 = Character Sheet
- @image3 = Product Master
```

**Câu hỏi mà Day 26 test:** Day 24 rule "không grid trong multi-ref" có áp cho **grid 4×2** (8 panels) không?

**Hypothesis:** Grid 4×2 mỗi panel to gấp 2 grid 4×4, AI parse dễ hơn → có thể work với multi-ref.

**Kết quả Day 26 (verified):**

| Pattern | Result |
| --- | --- |
| Grid 4×4 trong multi-ref (Day 24 rule) | ❌ FAIL — AI confuse, identity drift |
| Grid 4×2 trong multi-ref (Day 26 test) | ✅ **PASS** — character lock + product lock + scene composition đều đúng |

→ **Insight verified:** Day 24 rule "không grid trong multi-ref" **chỉ áp cho grid ≥ 4×4**. Grid nhỏ hơn (4×2 = 8 panels) work với multi-ref vì mỗi panel đủ to để AI parse.

### Cách quyết định pattern cho brief tương lai:

| Brief đặc trưng | Pattern recommend |
| --- | --- |
| Single 15s feature reel, product-focused | **Day 25** — 1 storyboard 4×4 single ref |
| 15s commercial với character + product + scene khác nhau | **Day 24** — 3 refs riêng biệt (no grid) |
| 15s+ cinema trailer với character anchor + scene structured | **Day 26** — multi-ref hybrid (Character + Product + Storyboard 4×2) |
| 30s+ multi-scene narrative | **Day 26 pattern × N clips** ghép trong CapCut |

---

## Phần 6 — 4 Ảnh Master + Storyboards Kết quả Thực tế

### 🎨 Prompt 1 — Character Sheet (Mẹ Hương + Con An turnaround)

![Character Sheet](https://github.com/linhai-creator/linh0ai-daily-tutorials/raw/main/assets/images/day-26-character-sheet-combined-turnaround.png)

**Layout 2 hàng × 3 cột = 6 views:**

- Hàng trên: Mẹ Hương 52 tuổi (Front / 3/4 / Side)
- Hàng dưới: Con An 19 tuổi (Front / 3/4 / Side)

**Quality:** ✅ Excellent. Mẹ và Con là **2 nhân vật khác nhau rõ ràng** (mẹ phúc hậu, con trái xoan thanh tú). Skin texture authentic tuổi 50+ vs tuổi 19. Outfit cố định xuyên 3 views mỗi character.

**Insight Day 26 (NEW pattern):** Character Sheet **combined** 2 nhân vật trong 1 ảnh (vs Day 24 mỗi nhân vật 1 ảnh riêng). Lý do: tiết kiệm cost (1 prompt thay 2) + AI tự ensure 2 nhân vật khác biệt rõ.

### 🎨 Prompt 2 — Product Master (Pháp phục lam flat lay)

![Product Master](https://github.com/linhai-creator/linh0ai-daily-tutorials/raw/main/assets/images/day-26-product-master-phap-phuc-lam.png)

**Product specs lock:**

- Áo dài tay rộng cổ tròn, vải cotton mềm màu lam pastel
- Cài nút vải tròn bên hông
- Quần ống suông cùng tone
- KHÔNG hoa văn, KHÔNG logo

**Phụ kiện decoration:** Lá bồ đề + chuỗi hạt gỗ nâu.

**Quality:** ✅ Excellent. Texture vải cotton rõ ràng, color lam pastel authentic. **Trust trigger** cho Trust signal sau này.

### 🎨 Prompt 3 — Storyboard Video 1 "TRƯỚC" (4×2 = 8 panels)

![Storyboard Video 1](https://github.com/linhai-creator/linh0ai-daily-tutorials/raw/main/assets/images/day-26-storyboard-video-1-truoc-8-panels.png)

**Story arc Act 1 + Act 2:**

- Hàng trên (Panels 1-4): Setup — Sân chùa empty → Mẹ cầu nguyện → Áo sờn → Mẹ cô đơn bồ đề
- Hàng dưới (Panels 5-8): Confrontation — Con nhìn mẹ → Mắt rưng rưng → Tay gấp áo mới → Cliffhanger

**Quality:** ✅ Excellent. Identity mẹ + con khớp Character Sheet. Pháp phục lam cũ vs mới phân biệt rõ. Composition cinematic mỗi panel khác nhau (wide / medium / close-up / macro).

### 🎨 Prompt 4 — Storyboard Video 2 "SAU" (4×2 = 8 panels)

![Storyboard Video 2](https://github.com/linhai-creator/linh0ai-daily-tutorials/raw/main/assets/images/day-26-storyboard-video-2-sau-8-panels.png)

**Story arc Act 3:**

- Hàng trên (Panels 9-12): Resolution — Mẹ nhận hộp → Mặc áo → Ngắm mình → ⭐ Memorable rưng rưng
- Hàng dưới (Panels 13-16): Trust + CTA — Wide bồ đề → Tay thợ may → Mẹ+Con cạnh nhau → CTA frame

**Quality:** ✅ Excellent. Panel 12 (Memorable Moment) đạt cảm xúc đỉnh — mẹ peaceful + 1 giọt nước mắt khóe mắt + dappled light. Panel 14 (Trust signal) macro tay thợ may chi tiết kim chỉ. Panel 16 có khoảng trống bottom cho CTA text overlay.

**Cost 4 ảnh master + storyboards:** ~3,600 VND (4 × ~900).

---

## Phần 7 — 2 Videos Seedance + 1 Video Final 30s Kết quả Thực tế

### 🎬 Video 1 — "TRƯỚC" (15s Setup + Confrontation)

[![Video 1 thumbnail](https://github.com/linhai-creator/linh0ai-daily-tutorials/raw/main/assets/images/day-26-video-1-thumbnail.jpg)](https://github.com/linhai-creator/linh0ai-daily-tutorials/raw/main/assets/videos/day-26-video-1-truoc-15s.mp4)
> 👆 Click thumbnail để xem video MP4 (15s, ~8MB) — **Cinema cliffhanger ending**

**Highlight frames:**

| Time | Mô tả |
| --- | --- |
| 1s | Wide sân chùa cổ với sunbeam rays — Hook visual stunning |
| 3s | Mẹ chắp tay peaceful, áo lam sờn visible — Character + status quo |
| 4.5s | Macro áo sờn rách extreme detail — Empathy trigger |
| 11.5s | Extreme close-up mắt An rưng rưng — Emotional climax |
| 13s | Macro tay gấp áo lam MỚI + lá bồ đề — Decision beat |
| 14.5s | An cầm hộp quyết tâm — **Cliffhanger** (mẹ không xuất hiện) |

**Honest assessment:**

- ✅ Identity mẹ + con consistent xuyên 8 panels (Character Sheet ref work)
- ✅ Pháp phục lam cũ vs mới phân biệt rõ (Product Master ref work)
- ✅ Hard cut từ Panel 7 sang Panel 8 cinematic — cliffhanger giữ nguyên
- ✅ Tone color đồng nhất (lam pastel + nâu + xanh lá + trắng dịu)
- ⚠️ Seedance timing slight deviation từ prompt: Panel 4 (wide bồ đề) dilate từ 1s thành 1.5s, không ảnh hưởng story
- ⚠️ Panel 5 transition có cross-dissolve artifact 1 frame thấy "2 mẹ" — đây là transition artifact (không phải duplicate bug thật)

### 🎬 Video 2 — "SAU" (15s Resolution + Trust + CTA)

[![Video 2 thumbnail](https://github.com/linhai-creator/linh0ai-daily-tutorials/raw/main/assets/images/day-26-video-2-thumbnail.jpg)](https://github.com/linhai-creator/linh0ai-daily-tutorials/raw/main/assets/videos/day-26-video-2-sau-15s.mp4)
> 👆 Click thumbnail để xem video MP4 (15s, ~6MB) — **⭐ Memorable Moment + Trust signal**

**Highlight frames:**

| Time | Mô tả |
| --- | --- |
| 1s | Mẹ nhận hộp áo, xúc động bất ngờ — Payoff cliffhanger |
| 3.5s | Mẹ mặc áo MỚI trong phòng ngủ VN — Transformation visible |
| 6s | Mẹ ngắm mình trước gương gỗ — Emotional buildup |
| **8.5s** | **⭐ Mẹ peaceful rưng rưng dưới bồ đề** — Memorable Moment đỉnh |
| 11s | Macro tay thợ may Huế khâu kim chỉ — Trust signal |
| 13s | Mẹ + Con cạnh nhau trước cổng tam quan — Family unity |
| 14.5s | CTA frame mẹ + An peaceful — Action invite |

**Honest assessment:**

- ✅ **Memorable Moment Panel 12 đạt cảm xúc đỉnh** — frame audience sẽ nhớ
- ✅ Continuity với Video 1 hoàn hảo (mẹ + con same identity, pháp phục same design)
- ✅ Panel 14 Trust signal macro tay thợ may đẹp cinematic
- ✅ Panel 16 có khoảng trống cho CTA text overlay
- ⚠️ Panel 9 minor deviation: An visible nửa người thay vì chỉ tay (prompt yêu cầu "chỉ tay") — không hurt story
- ⚠️ Panel 13 ban đầu có duplicate person bug (2 mẹ trong frame) → Fix với explicit "CHỈ 1 NGƯỜI" instruction → bug resolved

### 🎬 Video Final — 30s đã ghép CapCut (Cinema Trailer Production-Ready)

[![Final 30s thumbnail](https://github.com/linhai-creator/linh0ai-daily-tutorials/raw/main/assets/images/day-26-phap-phuc-lam-30s-thumbnail.jpg)](https://github.com/linhai-creator/linh0ai-daily-tutorials/raw/main/assets/videos/day-26-phap-phuc-lam-30s.mp4)
> 👆 Click thumbnail để xem video MP4 final (~30s, ~10MB) — **Cinema-style 30s trailer hoàn chỉnh với nhạc + CTA**

Đây là **output cuối cùng** của Day 26 — 2 videos × 15s đã ghép lại trong CapCut Desktop với **Hybrid workflow** (manual merge + AI music sync). Toàn bộ story arc 3-act + cliffhanger + Memorable Moment + Trust signal + CTA gói trong 30 giây.

**Cấu trúc 30s timeline:**

| Time | Phase | Mô tả |
| --- | --- | --- |
| 0-15s | Video 1 "TRƯỚC" | Setup + Confrontation + Cliffhanger ending |
| 15s | **Hard cut** | Transition Video 1 → Video 2 (KHÔNG fade — preserve cliffhanger) |
| 15-22s | Video 2 đầu | Resolution (mẹ nhận → mặc → ngắm) |
| **22-25s** | **⭐ Memorable Moment** | **Mẹ peaceful rưng rưng dưới bồ đề (3s static)** |
| 25-28s | Trust + Family | Wide bồ đề → Tay thợ may → Mẹ+Con cổng tam quan |
| 27.5-29.2s | CTA text overlay | Fade in/out CTA "PHÁP PHỤC LAM HUẾ" |
| 29.2-30s | Ending peaceful | Mẹ + An yên bình trước cổng |

**Specs technical:**

- **Resolution:** 1280×720 (720p)
- **Duration:** 29.27s (CapCut auto-trim 0.73s ở cuối, acceptable)
- **Codec:** H.264 video + AAC stereo audio 44.1kHz
- **Bitrate:** 2.68 Mbps
- **Frame rate:** 30fps (CapCut convert từ source 24fps)
- **Watermark:** KHÔNG có (export clean cho commercial use)

**Honest assessment:**

- ✅ Cliffhanger 14.5s → Panel 9 payoff hard cut work cinematic — audience không cảm giác "ghép 2 video"
- ✅ Memorable Moment Panel 12 giữ nguyên 3s static — KHÔNG bị Hybrid workflow shorten (insight kỹ thuật quan trọng)
- ✅ CTA text bottom 1/3 frame — đọc rõ trên busy background nhờ shadow
- ✅ Nhạc instrumental peaceful đồng bộ với tone video — không drop bass, không lyrics
- ✅ Tone color consistent xuyên 30s (lam pastel + nâu gỗ + xanh lá bồ đề + trắng dịu)
- ⚠️ CTA SĐT là placeholder `0XXX.XXX.XXX` — đây là video demo bài giảng. Khi áp dụng cho shop thật, thay bằng số thực tế.

> 💡 **Lưu ý cho học viên:** Đây là video demo minh họa pipeline. Khi các bạn sản xuất ad cho shop thật, output này sẽ là kết quả các bạn submit cho khách hàng. Quality + duration + structure đã production-ready cho campaign Facebook/Instagram.

**Cost 2 videos Seedance:** ~72,000 VND (2 × 36K).

---

## Phần 8 — ⭐ 6 Insights Mới Verified Day 26

### Insight 1: Cinema-style 30s Outperform Feature Reel 15s cho Sản phẩm High-Emotion

Day 25 verified feature reel 15s work cho product-focused commercial (sneaker, serum, trà). Day 26 verify **cinema-style 30s** (2 videos × 15s) work tốt hơn cho **sản phẩm high-emotion**:

| Loại sản phẩm | Format optimal |
| --- | --- |
| F&B generic | Feature reel 15s (Day 25 pattern) |
| Fashion branded | Feature reel 15s (Day 25 image-to-video) |
| Beauty generic | Feature reel 15s (Day 25 pattern) |
| **Gift / hiếu thảo / tâm linh** | **Cinema-style 30s (Day 26 pattern)** |
| **B2B luxury / wedding** | **Cinema-style 30s+ (Day 26 pattern)** |

**Tiêu chí quyết định:**

- Customer decide trong 15s (impulse buy) → feature reel
- Customer decide trong 1-7 ngày (considered purchase) → cinema-style

### Insight 2: 7 Câu Hỏi Strategic Framework Universal

7 câu hỏi (TRANSFORMATION / ENEMY / STAKES / HOOK / MEMORABLE / TRUST / ACTION) áp dụng được cho **mọi commercial brief**. Khi nhận brief mới từ khách, trả lời 7 câu trước khi viết prompt = chất lượng output tăng đáng kể.

→ **Khuyến nghị:** Save 7 câu thành **checklist template** trong notes/Notion. Mỗi brief mới copy template, trả lời 7 câu, sau đó mới viết prompt.

### Insight 3: Multi-Ref Hybrid với Grid 4×2 Work cho Seedance Omni 2.0 🎯

**Đây là insight kỹ thuật quan trọng nhất Day 26.**

Day 24 documented rule "Không upload grid 4×4 trong multi-ref single-clip". Day 26 verify rule này **chỉ áp cho grid ≥ 4×4**, không áp cho grid 4×2.

| Pattern | Result |
| --- | --- |
| 3 refs + grid 4×4 (Day 24 test) | ❌ FAIL — AI confuse, identity drift |
| 3 refs + grid 4×2 (Day 26 test) | ✅ **PASS** — character + product + composition đều lock |

**Lý do technical:**

- Grid 4×4 = 16 panels nhỏ → mỗi panel ~25% kích thước reference ảnh → AI khó parse
- Grid 4×2 = 8 panels → mỗi panel ~50% kích thước → AI parse rõ từng panel

**Implication cho khóa học:** Khi cần multi-ref + storyboard reference, **dùng grid 4×2 thay vì 4×4**. Story arc 15s = 8 panels là sweet spot (vs 16 panels Day 25 dư thừa cho 15s).

### Insight 4: Duplicate Person Bug Fix Pattern (Discovery Unique Day 26)

**Đây là insight Day 26 lần đầu phát hiện trong khóa học.**

**Bug:** Khi Character Sheet chứa nhiều views (Front/3/4/Side) của cùng 1 nhân vật, Seedance Omni 2.0 có thể **merge 2 views vào cùng 1 frame** → output có 2 nhân vật giống nhau trong 1 wide shot (đặc biệt frames có nhiều không gian background).

**Cụ thể Day 26:** Panel 13 ban đầu (Wide bồ đề mẹ) gen ra **2 mẹ** trong frame — 1 mẹ ở giữa + 1 mẹ phía xa background.

**Diagnosis:**

- AI nhận Character Sheet làm reference
- Character Sheet có 3 views mẹ (Front/3/4/Side)
- AI hiểu nhầm = "frame phải có nhiều mẹ" thay vì = "identity reference"

**Fix pattern (3 layers):**

1. **Explicit single-subject instruction per panel** — Trong prompt Panel 13: `Wide cinematic画面中CHỈ 1 NGƯỜI DUY NHẤT — 母亲...绝对不要出现第二个母亲`
2. **Educate AI về Character Sheet purpose** — Add note: `如果@image2 Character Sheet中有母亲多个views，AI请理解那是身份reference，不是要在视频frame中显示多个母亲`
3. **DUPLICATE PERSON BUG PREVENTION section** trong 严格避免 — Liệt kê chi tiết person count expected cho từng panel

**Verified:** Fix work — Panel 13 sau khi áp 3 layers → chỉ 1 mẹ duy nhất, identity vẫn lock từ Character Sheet.

**Rule generalize:** Khi multi-ref bao gồm Character Sheet với nhiều views, **LUÔN add explicit single-subject instruction** cho mỗi panel có wide shot.

### Insight 5: Visual Prior Bias khi Gen Storyboard Sequel (Discovery Unique Day 26)

**Bug:** Khi gen Storyboard Video 2 với 3 references (Character + Product + **Storyboard Video 1**), AI output ra content gần giống Storyboard Video 1 (Setup + Confrontation) thay vì Video 2 content mới (Resolution + Trust + CTA).

**Diagnosis:** AI ưu tiên **visual signal** (Storyboard Video 1 reference) hơn **text prompt signal** (text mô tả Video 2 content). Visual prior bias rất mạnh khi reference image có structure rõ (8 panels grid).

**Fix:** **KHÔNG upload Storyboard Video 1 làm reference khi gen Storyboard Video 2.**

Continuity giữa 2 videos đảm bảo qua:

- Character Sheet (lock identity mẹ + con)
- Product Master (lock design pháp phục)
- Text prompt explicit: `tone color match Storyboard Video 1: lam pastel + nâu + xanh lá + trắng dịu`

→ KHÔNG cần upload Storyboard cũ làm reference.

**Rule generalize:** Khi gen sequel/Part 2 của 1 series, **chỉ upload upstream master references** (Character + Product), KHÔNG upload Part 1 output làm reference.

### Insight 6: Memorable Moment 3s Static Camera = Cry-Trigger Design

5 conditions để frame Memorable Moment đạt cry-trigger:

1. Single subject focus (không distraction)
2. Static camera (không movement, 3s)
3. Duration unusual (dài hơn các panels khác 1.5-2x)
4. Small visual cue (1 giọt nước mắt khóe mắt, không rơi)
5. Dappled light (natural environmental light pattern)

→ Pattern này áp dụng cho **mọi sản phẩm high-emotion**. Wedding ads, gift ads, hiếu thảo ads đều có thể design 1 frame Memorable Moment theo công thức này.

---

## Phần 9 — CapCut Hybrid Workflow (Edit 2 Videos thành 30s Final)

Sau khi có 2 videos Seedance, dùng CapCut Desktop ghép + thêm nhạc + CTA. Day 26 verify **Hybrid workflow** (manual merge + AI music sync) là optimal cho cinema trailer.

### Tại sao KHÔNG dùng CapCut "Auto Cut" classic?

CapCut "Auto Cut" / "Công cụ cắt clip bằng AI" được thiết kế để **cắt 1 video dài thành nhiều clip ngắn**. Nếu apply cho 2 videos 15s đã cinema-design, AI có thể:

- Cắt mất Panel 12 Memorable Moment (3s static = "low motion" AI nghĩ là "boring")
- Add fade transition giữa Panel 8 → Panel 9 → mất cliffhanger feel
- Cắt nhỏ frames → mất pacing rhythm cinema

→ **Avoid Auto Cut cho cinema-designed videos.**

### Hybrid Workflow 8 bước:

**Bước 1 — Import 2 videos:** Mở CapCut Desktop → Dự án mới → Nhập 2 file → kéo Video 1 + Video 2 lên timeline track Video chính.

**Bước 2 — Chuyển tiếp:** Để **KHÔNG có transition** giữa Video 1 và Video 2. Hard cut là cinematic standard cho cliffhanger.

**Bước 3 — Thêm nhạc:** Tab Âm thanh → Nhạc → search keywords ưu tiên: `zen`, `meditation`, `temple`, `emotional piano`, `bamboo flute`. Preview 5-10 bài, chọn 1 bài có tempo chậm 60-80 BPM, không lời, build-up ở giữa.

Tránh nhạc upbeat pop / EDM / TikTok viral sounds → phá tone peaceful.

**Bước 4 — Adjust nhạc:** Click clip nhạc → âm lượng 30-40% → fade in 0.5s + fade out 1s.

**Bước 5 — Cắt nhạc khớp 30s:** Kéo cạnh phải clip nhạc về vị trí 30:00.

**Bước 6 — Thêm CTA text Panel 16:** Tab Văn bản → kéo text box đến giây 27.5 → 29.2 (~1.7s duration cho audience đọc).

CTA text settings (verified work cho 1080p):

- **Cỡ chữ:** 11-14 (font Inter-Medium / Be Vietnam Pro)
- **Màu:** Trắng `#FFFFFF` + shadow đen mỏng
- **Position:** Bottom 1/3 frame (không che mặt nhân vật)
- **Animation:** Fade in 0.3s, fade out 0.3s

**Bước 7 — Preview verify 5 điểm:**

1. Tổng duration ~ 30s
2. Panel 12 (giây 22-25) vẫn dài 3s — KHÔNG bị Auto Cut shorten
3. Cliffhanger giây 14-15 hard cut
4. Nhạc tone peaceful, không drop bass
5. CTA text chỉ hiện 1-2s cuối, không che mặt

**Bước 8 — Xuất:** 1080p, 24fps (match source — KHÔNG để 30/60fps), H.264 codec, MP4, bitrate Khuyến nghị.

→ Output: **`day-26-phap-phuc-lam-30s.mp4`** ~ 25-40MB, production-ready ad.

---

## Phần 10 — Compliance VN cho Religious Products

Pháp phục Phật tử thuộc category **religious-sensitive products** ở Việt Nam. Quảng cáo phải tuân thủ:

- **Luật Quảng cáo 2012** điều 8 (cấm xúc phạm tôn giáo)
- **Luật Tín ngưỡng, Tôn giáo 2016** (không xúc phạm hoạt động tín ngưỡng)
- Cultural sensitivity (không thương mại hóa tâm linh)

### 6 quy tắc compliance Day 26:

**1. KHÔNG show bàn thờ rõ nét trong background.** Bàn thờ là không gian thiêng — không nên xuất hiện rõ trong frame thương mại. Nếu xuất hiện, phải mờ background hoặc out of focus.

**2. KHÔNG show tượng Phật close-up.** Tượng Phật là đối tượng tôn kính — close-up tượng cho mục đích thương mại có thể bị hiểu nhầm là disrespect.

**3. KHÔNG show hương đốt rõ ràng.** Hương = nghi lễ — show rõ có thể gây cảm giác "quảng cáo dịch vụ tôn giáo".

**4. KHÔNG show sư sãi / nhà tu hành.** Nhân vật tôn giáo không được sử dụng cho thương mại trừ khi có permission explicit.

**5. KHÔNG glamour pose / makeup đậm trên người mặc pháp phục.** Pháp phục là trang phục trang nghiêm — fashion glamour pose hoặc makeup đậm vi phạm tinh thần.

**6. Trang nghiêm peaceful tones, KHÔNG over-spiritual.** Tone color recommend: lam pastel + nâu gỗ + xanh lá bồ đề + trắng dịu. Avoid: golden hour cam đậm, dramatic high contrast, neon effects.

### Pattern này áp dụng được cho:

- Pháp phục Phật tử (Day 26)
- Áo dài tâm linh
- Trang phục biểu diễn hầu đồng (cẩn thận hơn — có thể restrict)
- Phụ kiện tâm linh (chuỗi hạt, vòng tay phong thủy)
- Bài giảng / khóa thiền online (cẩn thận hơn — không claim healing)

### Pattern này KHÔNG áp dụng cho:

- Bùa chú / phong thủy claim cụ thể (vi phạm Luật Quảng cáo điều cấm "lừa dối / mê tín")
- Dịch vụ tâm linh có thu phí (cúng giải hạn, xem tử vi cá nhân)
- Sản phẩm claim healing / chữa bệnh tâm linh

→ Học viên nhận job ad shop áo dài / pháp phục / phụ kiện tâm linh safe với pattern Day 26.

---

## Phần 11 — Lỗi thường gặp khi production cinema-style ads

**Skip 7 câu hỏi strategic framework.** Đây là lỗi lớn nhất — viết prompt trực tiếp mà không trả lời 7 câu = output có thể đẹp nhưng không hit emotional target. Audience xem mà không feel.

**Force cinema-style 30s cho mọi sản phẩm.** Sản phẩm impulse buy (F&B, fashion basic) không cần cinema — feature reel 15s đủ. Force 30s = waste budget + audience scroll sớm.

**Skip Memorable Moment design.** Trailer 30s không có Memorable Moment = audience xem xong quên ngay. Phải có 1 frame audience sẽ nhớ ít nhất 24 giờ sau khi xem.

**Cliffhanger ending mà không có payoff sớm.** Cliffhanger Video 1 phải được payoff trong Panel 9 Video 2 (giây 15-17). Nếu payoff trễ (sau giây 20) audience đã mất kiên nhẫn.

**Upload Storyboard Part 1 làm reference cho Part 2.** Visual prior bias — AI sẽ copy content thay vì follow text prompt. Continuity đảm bảo qua Character + Product master, không cần Storyboard cũ.

**Multi-ref với grid 4×4.** Day 24 rule áp cho grid ≥ 4×4. Day 26 grid 4×2 work, nhưng nếu cần 16 panels structure thì dùng Day 25 single-ref pattern (không kèm Character/Product master).

**Memorable Moment camera movement.** Camera phải static 3s. Pan/zoom làm audience focus vào motion, không focus vào emotion.

**Memorable Moment nước mắt RƠI xuống má.** Đó là crying (sad). Day 26 design = nước mắt RƯNG RƯNG đọng khóe mắt (moved, peaceful). Rơi xuống má → trigger sadness, không trigger inspiration.

**CapCut Auto Cut classic cho cinema-designed videos.** AI sẽ cắt nhỏ Panel 12 → mất Memorable Moment. Dùng Hybrid workflow (manual merge + AI music sync).

**CTA text quá to.** Cỡ chữ 36-42 mà nhiều tutorial mạng recommend là cho TikTok 9:16 vertical. Cho 1080p 16:9 horizontal, cỡ 11-14 là sweet spot.

**CTA text che mặt nhân vật.** Bottom 1/3 frame là vị trí safe. Top hoặc center thường che mặt.

**Skip compliance check cho religious products.** Vi phạm Luật Quảng cáo 2012 + Luật Tín ngưỡng 2016 = ad bị Facebook/Google reject + có thể bị xử phạt hành chính.

---

## Bài tập thực hành

Chọn 1 brief của riêng bạn thuộc category **high-emotion** (gift, hiếu thảo, kỷ niệm, B2B luxury, wedding) và áp dụng pipeline Day 26:

**Bước 1 — Trả lời 7 câu hỏi strategic framework:**

| # | Câu hỏi | Brief của bạn |
| --- | --- | --- |
| 1 | TRANSFORMATION trước/sau? | _______ |
| 2 | ENEMY của customer? | _______ |
| 3 | EMOTIONAL STAKES? | _______ |
| 4 | HOOK 3s đầu? | _______ |
| 5 | MEMORABLE MOMENT? | _______ |
| 6 | TRUST signal? | _______ |
| 7 | ACTION CTA? | _______ |

**Bước 2 — Character + Product master (Prompts 1-2):**

- Character Sheet turnaround 6 views (nếu có nhân vật)
- Product Master flat lay
- Cost ~1,800 VND

**Bước 3 — Storyboard 4×2 × 2 (Prompts 3-4):**

- Storyboard 1 "TRƯỚC" với cliffhanger ending
- Storyboard 2 "SAU" với Memorable Moment + CTA frame
- Upload references: Character Sheet + Product Master (KHÔNG upload Storyboard 1 cho Prompt 4)
- Cost ~1,800 VND

**Bước 4 — Videos Seedance × 2 (Prompts 5-6):**

- Multi-ref hybrid: Storyboard + Character + Product
- Tiếng Trung 11-section template Day 22 + anti-pop-in Day 24
- Cost ~72,000 VND

**Bước 5 — CapCut Hybrid edit:**

- Manual merge 2 videos (no transition)
- Add nhạc instrumental peaceful
- CTA text Panel 16 (cỡ 11-14, bottom 1/3)
- Export 1080p 24fps MP4

**Bước 6 — Review honest:**

- Memorable Moment có cry-trigger không?
- Cliffhanger có hook audience xem Video 2 không?
- 7 câu hỏi strategic được trả lời visible trên screen?
- Compliance VN cho category sản phẩm bạn chọn?

---

## Tiêu chí đạt bài

- [ ] Trả lời 7 câu hỏi strategic framework cho brief
- [ ] 1 Character Sheet turnaround (nếu có nhân vật)
- [ ] 1 Product Master flat lay
- [ ] 2 Storyboards 4×2 với story arc 3-act
- [ ] 2 Videos × 15s từ Seedance multi-ref hybrid
- [ ] 1 Video final 30s đã edit CapCut với nhạc + CTA
- [ ] Memorable Moment đạt cry-trigger (5 conditions)
- [ ] Cliffhanger ending Video 1 + payoff Video 2
- [ ] Compliance check cho category sản phẩm
- [ ] CTA text Panel 16 đúng cỡ + position

---

## Cost summary Day 26

| Item | Cost |
| --- | --- |
| Character Sheet (Prompt 1) | ~900 VND |
| Product Master (Prompt 2) | ~900 VND |
| Storyboard Video 1 (Prompt 3) | ~900 VND |
| Storyboard Video 2 (Prompt 4) | ~900 VND |
| Video 1 Seedance (Prompt 5) | ~36,000 VND |
| Video 2 Seedance (Prompt 6) | ~36,000 VND |
| **Tổng cost cơ bản** | **~75,600 VND** |
| Buffer re-gen 20% | ~15,000 VND |
| **Total budget** | **~91,000 VND** |

→ Day 26 cost tương đương Day 25 (~110K) nhưng output là **cinema trailer 30s** production-ready cho sản phẩm high-emotion, không phải 3 feature reels generic.

---

## Sang Day 27

Day 27 sẽ là **A/B Testing + Multi-Platform Optimization**:

- Adapt cinema trailer 30s sang 3 versions cho 3 platforms:
  - **Facebook Feed 16:9** (1080p × 1920p, full 30s)
  - **TikTok/Reels 9:16** (vertical crop, có thể giữ 30s hoặc trim 15s)
  - **YouTube Shorts 9:16** (vertical, full 30s)
- Aspect ratio adaptation strategy (không phải mọi panel work cho 9:16)
- Hook A/B testing — 2 phiên bản 3s đầu khác nhau
- Performance metrics framework (CTR, completion rate, conversion)

Sau Day 27, các bạn có **multi-platform package** ready deploy cho cùng 1 brief.

---

## 📍 Navigation

[⬅️ Day 25: Pipeline Practice 3 Ngành + Risk Matrix Verification](https://github.com/linhai-creator/linh0ai-daily-tutorials/blob/main/days/day-25.md) | [🏠 README](https://github.com/linhai-creator/linh0ai-daily-tutorials/blob/main/README.md) | [➡️ Day 27: A/B Testing + Multi-Platform Optimization](https://github.com/linhai-creator/linh0ai-daily-tutorials/blob/main/days/day-27.md)

---

## 🏷️ Tags

#0aiVN #Day26Linh0AI #CinemaStyle30s #2VideosX15s #7CauHoiStrategic #MemorableMoment #CliffhangerEnding #MultiRefHybrid #DuplicatePersonBugFix #VisualPriorBias #CapCutHybridWorkflow #ReligiousCompliance #PhapPhucLam #Tuan4

---

*Linh0AI Daily Tutorials — Day 26/30 (87%) Tuần 4 Day 5: Cinema-style 30s trailer (2 videos × 15s) + 7 câu hỏi strategic framework + Multi-ref hybrid pattern verified + Duplicate person bug fix pattern discovered + 6 insights mới + 91K VND cost actual*
