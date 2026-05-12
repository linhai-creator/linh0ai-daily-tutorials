# Day 23 — Shot List Sản xuất

> Tuần 4 Day 2. Sau khi có brief + kịch bản 15s từ Day 22, bài này tách kịch bản thành shot list chi tiết — biến planning thành production blueprint. Bài này cũng quyết định approach: 1 clip Seedance 15s (như Day 22 demo) hay multi-shot 3-5 clips ghép trong CapCut.

---

## Mục tiêu bài học

Sau bài này, các bạn sẽ:

- Hiểu 2 approaches cho 1 ad 15s: single-clip vs multi-shot
- Biết khi nào chọn approach nào (decision tree concrete)
- Tách kịch bản 15s thành shot list 3-5 shots
- Áp dụng Risk Matrix Day 22 để chọn model phù hợp cho từng shot
- Có asset checklist + risk checklist sẵn sàng cho Day 24

## Output cuối bài

- 1 quyết định approach (single-clip hoặc multi-shot)
- Nếu multi-shot: 1 shot list 3-5 shots với 2 bảng Planning + Execution
- 1 bảng chọn model theo shot type
- 1 asset checklist 6 nhóm
- 1 risk checklist với mitigation rõ ràng

## Cost dự kiến

| Item | Cost |
|------|------|
| Planning thuần | 0 VND |
| **Tổng Day 23** | **0 VND** |

→ Day 23 không generate. Toàn bộ planning work để Day 24-26 (storyboard + Seedance + edit) hiệu quả, ít re-gen lãng phí credit.

---

## Phần 1 — Vì sao cần shot list?

Day 22 mình có brief + kịch bản 15s với 5 timecodes — Hook, Product, Benefit, Emotion, CTA. Đây là **high-level outline** cho audience experience, không phải production blueprint.

Nếu cầm kịch bản đó đi generate luôn, sẽ gặp 5 vấn đề:

1. **Không quyết định trước approach** — 1 clip 15s hay multi-shot? Quyết sai = lãng phí credit
2. **Tiêu credit lãng phí** — không identify risk trước, re-gen nhiều lần
3. **Asset scramble** — đến shot cuối mới phát hiện cần logo PNG mà chưa có
4. **Model mismatch** — dùng Seedance text-to-video cho branded product (HIGH risk theo Risk Matrix Day 22) → fail predictable
5. **Edit chỉnh sửa muộn** — quay lại sửa shot 2 sau khi shot 5 đã render xong = lãng phí credit + thời gian

Shot list giải quyết 5 vấn đề này bằng cách **plan trước mọi technical decision** trước khi tiêu credit đầu tiên.

---

## Phần 2 — 2 approaches cho ad 15s

Trước khi viết shot list, mình quyết approach. Day 22 đã verify cả 2 approaches work, mỗi cái có trade-off riêng.

### Approach A — Single clip Seedance 15s

1 clip duy nhất render full 5 phases internal (như 4 tests Day 22).

| Aspect | Detail |
|--------|--------|
| Số clips Seedance | 1 |
| Duration mỗi clip | 15s |
| Cost generate | 36,000 VND |
| Edit phase | Minimal — chỉ add logo/text overlay + audio |
| Risk | Cao nếu clip fail → re-gen full 36K |
| Flexibility | Thấp — không thể thay 1 phase lẻ |

**Khi nào dùng:**
- Sản phẩm generic LOW risk (cà phê, serum, bánh mì — Day 22 đã verify)
- Budget tight (1 lần generate là xong)
- Ad đơn giản, không cần camera variety phức tạp

### Approach B — Multi-shot 3-5 clips × 3-5s

Ghép nhiều clips ngắn trong CapCut. Mỗi clip = 1 shot riêng biệt.

| Aspect | Detail |
|--------|--------|
| Số clips Seedance | 3-5 |
| Duration mỗi clip | 3-5s |
| Cost generate | ~36-50K VND (tùy duration min Seedance) |
| Edit phase | Phức tạp hơn — ghép transitions + audio sync |
| Risk | Thấp — 1 clip fail chỉ re-gen 1 clip (~7-12K) |
| Flexibility | Cao — đổi 1 phase mà không ảnh hưởng phase khác |

**Khi nào dùng:**
- Branded products (HIGH risk) — cần image-to-video với reference từng shot
- Ad cần camera variety phức tạp (macro + medium + tracking + hero không fit 1 prompt)
- Khi có budget buffer để re-gen
- Khi cần A/B test từng shot

### Decision tree

```
Bắt đầu với kịch bản 15s
        ↓
Sản phẩm có brand/logo cần lock?
   ├─ CÓ → Approach B (multi-shot với image-to-video)
   └─ KHÔNG → Tiếp tục
        ↓
Camera variety có quá phức tạp cho 1 clip?
   ├─ CÓ → Approach B
   └─ KHÔNG → Approach A (single clip)
```

→ **Đa số creator solo nên start với Approach A.** Khi đã có experience, level up Approach B khi cần.

---

## Phần 3 — Anatomy shot list: 12 trường thông tin

Nếu chọn Approach B (multi-shot), shot list cần 12 trường thông tin chia 2 bảng để dễ đọc trên mobile/GitHub.

### Bảng 1 — PLANNING (creative side)

| Trường | Mục đích |
|--------|----------|
| Shot # | ID để reference (Shot 1, Shot 2...) |
| Time | Vị trí trong kịch bản 15s (vd 0-3s) |
| Phase công thức | Hook / Product / Benefit / Emotion / CTA |
| Sản phẩm/Nhân vật | Subject chính trong shot |
| Bối cảnh | Setting (cafe / studio / street...) |
| Action chính | 1 hành động duy nhất (quy tắc Day 18) |
| Camera | Loại shot (macro / medium / hero / wide...) |
| Sound | Audio cụ thể (ambient / SFX / voice) |

### Bảng 2 — EXECUTION (technical side)

| Trường | Mục đích |
|--------|----------|
| Shot # | Match Bảng 1 |
| Model | Seedance text-to-video / image-to-video / GPT Image 2 keyframe / CapCut edit |
| Duration | Thời lượng generate (3s, 4s, 5s) |
| Asset cần chuẩn bị | Logo PNG / reference photo / font file... |
| Risk lỗi | Identified risk từ Risk Matrix Day 22 |

→ Bảng 1 = "Cảnh gì?" Bảng 2 = "Làm thế nào?". Mỗi shot fill cả 2 bảng.

Nếu chọn Approach A (single clip), không cần shot list traditional — toàn bộ 5 phases đã trong 1 prompt Seedance (Day 22 template 11 section).

---

## Phần 4 — Shot list mẫu Approach B: Cà phê sữa đá 15s

Áp dụng kịch bản Ví dụ 1 Day 22 (cà phê sữa đá quán nhỏ Sài Gòn). Kịch bản 5 timecodes 15s → tách thành 5 shots multi-clip.

### Bảng 1 — PLANNING (cà phê 15s, multi-shot)

| Shot | Time | Phase | Sản phẩm/Nhân vật | Bối cảnh | Action chính | Camera | Sound |
|------|------|-------|-------------------|----------|--------------|--------|-------|
| 1 | 0-3s | Hook | Ly cà phê đá | Quầy cafe gỗ, sáng warm | Giọt nước condensation nhỏ giọt | Macro extreme close-up | Ice clink |
| 2 | 3-6s | Product | Ly cà phê + tay barista | Quầy bar cafe | Rót cà phê đậm vào ly đá | Medium 3/4 angle | Coffee pouring |
| 3 | 6-10s | Benefit | Ly cà phê + sữa hòa | Cận ly trên quầy gỗ | Khói + sữa hòa vào (stable state) | Macro top-down | Cafe ambience |
| 4 | 10-13s | Emotion | Khách hớp + biểu cảm partial | Bàn cafe, background bokeh | Khách hớp ngụm, miệng mỉm | Medium portrait crop tight | Nhạc nhẹ + sip |
| 5 | 13-15s | CTA | Ly cà phê hero + logo overlay | Quầy cafe central | Ly đặt centered, logo add edit | Hero shot centered | Ending music + CTA voice |

### Bảng 2 — EXECUTION (cà phê 15s, multi-shot)

| Shot | Model | Duration | Asset cần chuẩn bị | Risk lỗi |
|------|-------|----------|--------------------|----------|
| 1 | Seedance text-to-video | 3s | Không cần | Liquid state morph (Day 22 coffee insight) |
| 2 | Seedance text-to-video | 3s | Không cần | Hand warp → crop chỉ tay + chai |
| 3 | Seedance text-to-video | 4s | Không cần | Liquid state change → lock "stable mixed state" |
| 4 | Seedance text-to-video | 3s | Không cần | Face full warp → crop partial (miệng + cằm) |
| 5 | GPT Image 2 keyframe + Seedance image-to-video | 2s | Logo quán PNG + CTA copy | Logo render bịa → image lock, video add motion |

**Tổng duration generate:** 3 + 3 + 4 + 3 + 2 = 15s exact (nếu Seedance support min 2-3s). Nếu min Seedance là 5s, tăng mỗi shot lên 5s = total 25s raw, trim trong CapCut về 15s final.

### Tổng cost ước tính cho Approach B (Day 25-26)

| Item | Calc | Cost |
|------|------|------|
| Day 25 Seedance generate (15s total assuming min 3s) | 15 × 2,400 | ~36,000 VND |
| Day 25 Seedance generate (25s total assuming min 5s) | 25 × 2,400 | ~60,000 VND |
| Day 24 keyframes + storyboard | ~5 × 900 | ~4,500 VND |
| Day 26 buffer re-gen 20-30% | | ~10-15K VND |
| **Tổng Approach B ước tính** | | **~50-80K VND** |

**So sánh Approach A:**
- Approach A (1 clip 15s): ~36K + Day 24 keyframe ~900 = **~37K total**
- Approach B (multi-shot): **~50-80K total** (tùy Seedance min duration)

→ Approach A rẻ hơn nhưng Approach B linh hoạt hơn. Trade-off rõ ràng.

---

## Phần 5 — Bảng chọn model theo shot type

Decision tree này mình rút ra từ Day 22 Risk Matrix (4 tests, 144K VND data thực):

| Shot type | Best model | Lý do |
|-----------|-----------|-------|
| Product static hero (logo, brand cần lock) | **GPT Image 2 keyframe** | Precision lock, không cần motion |
| Product action không brand (rót, nhỏ giọt) | **Seedance text-to-video** | Motion natural, generic LOW risk |
| Product motion + brand cần consistent | **GPT Image 2 keyframe → Seedance image-to-video** | Image lock branding, video thêm motion |
| Người + sản phẩm (LOW risk product) | **Seedance text-to-video** | Risk face warp manageable nếu crop partial |
| Người + sản phẩm (HIGH risk branded) | **Seedance image-to-video** với reference | Image-to-video override training bias |
| Text overlay (CTA, brand name) | **CapCut edit phase** | KHÔNG dùng AI generate text — 100% fail (Day 22 sneaker "BIOTOR") |

### 3 quy tắc chính từ Risk Matrix Day 22

1. **Branded products** → KHÔNG dùng Seedance text-to-video (HIGH risk fail)
2. **Text/logo trên product** → KHÔNG generate bằng AI — luôn add edit phase trong CapCut
3. **Static product hero** → keyframe (precision); **Motion shot** → video model

---

## Phần 6 — Asset checklist trước Day 24

Sau khi có shot list, chuẩn bị 6 nhóm assets trước khi sang Day 24-26:

| Nhóm | Mục tiêu | Format |
|------|----------|--------|
| Logo quán/brand | Add edit phase (Shot CTA) | PNG transparent, ≥500px |
| Sản phẩm reference photo | Cho image-to-video nếu HIGH risk | JPG/PNG real shot |
| Brand colors | Color grading consistent | Hex codes (vd #8B4513) |
| Audio assets | Voice/BGM cho edit | MP3/WAV |
| Font file | Text overlay | TTF/OTF |
| CTA copy | Voice script + text on screen | Plain text |

**Risk nếu skip checklist:** Đến giữa Day 24 (storyboard) hoặc Day 25 (Seedance) mới phát hiện thiếu logo PNG → phải pause production, scramble find/create asset → lãng phí thời gian, mất flow.

---

## Phần 7 — Risk checklist: identify trước, mitigate sớm

Mỗi shot trong list cần identify ít nhất 1 risk + mitigation strategy. Đây là application thực tế Risk Matrix Day 22:

| Shot | Risk identify | Mitigation strategy |
|------|---------------|---------------------|
| 1 — Macro cà phê | Liquid state morph (Day 22 coffee insight) | Prompt thêm "稳定融合状态" / "已经混合好的" |
| 2 — Barista rót | Hand/body warp | Crop chỉ tay + chai cà phê, không show face barista |
| 3 — Macro khói + sữa | Sản phẩm transform giữa frame | Lock single state, 1 action duy nhất (quy tắc Day 18) |
| 4 — Khách hớp ngụm | Face full → warp risk cao | Crop partial face (chỉ miệng + cằm), hoặc back shot |
| 5 — Product hero + logo | Logo render bịa (Day 22 BIOTOR pattern) | GPT Image 2 keyframe trước, CapCut edit thêm logo PNG sau |

### 5 quy tắc chung mitigation

1. **Generic products (LOW risk):** prompt text-to-video OK, không cần mitigation đặc biệt
2. **Liquid products:** lock state cụ thể trong prompt — không để model interpret mixing process
3. **Human + product:** crop tight, hạn chế full face/body để giảm warp risk
4. **Branded products:** KHÔNG dùng text-to-video — luôn image-to-video với reference ảnh thật
5. **Text/logo trên video:** add edit phase trong CapCut, KHÔNG generate AI

---

## Phần 8 — 6 lỗi thường gặp

**Skip quyết định approach.** Lao vào shot list multi-shot ngay mà không cân nhắc Approach A (1 clip 15s). Cà phê/serum/bánh mì test Day 22 đều work với 1 clip — không cần Approach B phức tạp.

**Mỗi shot quá nhiều action.** "Shot 3: barista pha cà phê, rót sữa, trang trí, đưa cho khách" — 4 actions trong 1 shot vi phạm quy tắc Day 18 "1 shot = 1 action chính". AI render sẽ lỗi. Tách thành 4 shots riêng.

**Không identify risk trước.** Risk Matrix Day 22 rút ra với cost 144K VND. Skip risk identification ở Day 23 = lãng phí experience đó.

**Chọn sai model.** Dùng Seedance text-to-video cho sneaker → predict fail từ Day 22 (logo brand thật + brand swap + Frankenstein). Phải dùng image-to-video với reference ảnh giày thật.

**Quên asset checklist.** Đến Day 24 phát hiện thiếu logo PNG → pause production. Asset checklist Day 23 prevent issue này hoàn toàn.

**Shot list trên giấy.** Viết tay, không sync với brief Day 22 → quên elements quan trọng trong brief (CTA cụ thể, brand colors). Shot list nên là file markdown/spreadsheet copy được vào project folder.

---

## Bài tập thực hành

Chọn 1 brief từ 4 ví dụ Day 22 (cà phê / serum / bánh mì / sneaker) hoặc brief của bạn.

**Bước 1:** Quyết approach
- Approach A nếu generic LOW risk + đơn giản
- Approach B nếu branded HIGH risk hoặc cần variety phức tạp

**Bước 2:** Nếu chọn Approach B, tách shot list hoàn chỉnh:
- Bảng 1 PLANNING — 3-5 shots với 8 columns
- Bảng 2 EXECUTION — matching shots với 5 columns

**Bước 3:** Asset checklist 6 nhóm

**Bước 4:** Risk checklist với mitigation mỗi shot

Shot list này là input cho Day 24 (storyboard + keyframe). Shot list tốt = Day 24 nhẹ nhàng.

---

## Tiêu chí đạt bài

- [ ] Có quyết định approach (A hoặc B) với lý do cụ thể
- [ ] Nếu Approach B: Bảng 1 PLANNING có 3-5 shots, đủ 8 columns
- [ ] Nếu Approach B: Bảng 2 EXECUTION có 3-5 shots, đủ 5 columns
- [ ] Mỗi shot có 1 action chính (không nhồi nhiều action)
- [ ] Mỗi shot có model assignment cụ thể từ Bảng chọn model
- [ ] Asset checklist liệt kê ≥3 nhóm cần thiết
- [ ] Risk checklist có mitigation rõ ràng cho ≥3 shots
- [ ] Tổng duration shots = 15s

---

## Cost summary Day 23

| Item | Cost |
|------|------|
| Planning thuần | 0 VND |
| **Tổng Day 23** | **0 VND** |

---

## Sang Day 24

Day 24 mình sẽ generate **storyboard + keyframes** từ shot list này.

- **Nếu Approach A:** 1 storyboard 5-panel overview + 1 keyframe hero shot
- **Nếu Approach B:** 1 storyboard overview + 3-5 keyframes (1 per shot)

Brief Day 22 + Shot list Day 23 = đủ input cho Day 24. Học viên hoàn thành Day 23 trước rồi sang.

---

## 📍 Navigation

[⬅️ Day 22: Brief & Kịch bản 15s](https://github.com/linhai-creator/linh0ai-daily-tutorials/blob/main/days/day-22.md) | [🏠 README](https://github.com/linhai-creator/linh0ai-daily-tutorials/blob/main/README.md) | [➡️ Day 24: Storyboard & Keyframe](https://github.com/linhai-creator/linh0ai-daily-tutorials/blob/main/days/day-24.md)

---

## 🏷️ Tags

#0aiVN #Day23Linh0AI #ShotList #PreProduction #CommercialPipeline #RiskMatrix #AssetChecklist #SingleClipVsMultiShot #Tuan4

---

*Linh0AI Daily Tutorials — Day 23/30 (77%) Tuần 4 Day 2: Shot list 3-5 shots cà phê 15s + 2 approaches decision tree + Asset/Risk checklist + 0 VND cost (pure planning)*
