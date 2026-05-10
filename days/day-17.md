# 🚀 Day 17 — Naming Convention & Version Control

> **Tuần 3 — Practical Production | Bài 3/7**
> *Đặt tên file ảnh AI và prompt sao cho 6 tháng sau vẫn tìm được trong 30 giây*

---

## 🎯 Mục tiêu Day 17

Sau bài này, các bạn sẽ:

- Có **quy tắc đặt tên file** chuẩn cho ảnh AI và prompt
- Biết cách **version control** (v1, v2, final, archive) mà không cần học Git
- Có **format pattern** áp dụng được cho mọi project (cá nhân + khách hàng)
- Tránh được **6 anti-patterns** thường gặp khi đặt tên file
- Có **cheatsheet 1 trang** dán lên màn hình

---

## 😤 Vấn đề thực tế: 110 ảnh test, 6 tháng sau khó tìm

Sau Tuần 2 mình đã tích lũy 95 ảnh test verified. Day 16 thêm 15 ảnh nữa. Tổng 110 ảnh trong folder.

Hôm qua mình thử mở lại folder, tìm "ảnh áo dài Tết phố cổ Hà Nội" của Day 9. Kết quả:

- Phải scroll qua hơn 60 file
- Một số file tên tùy hứng: `c1-traditional.png`, `seedream-trad-pro.png`, `pro-trad-1.jpg` — không nhớ cái nào là cái nào
- Mất 8 phút mới tìm ra ảnh đúng

Vấn đề **không phải số lượng** — 110 ảnh chưa nhiều. Vấn đề là **hệ thống tên không nhất quán**: nhìn tên file không biết ngay là ảnh gì, ở Day nào, version nào.

→ Day 17 mình cùng các bạn xây quy tắc đặt tên để 6 tháng sau mở folder vẫn tìm được trong 30 giây.

---

## 5 yếu tố trong tên file chuẩn

Mỗi file ảnh AI nên chứa đủ 5 thông tin trong tên:

| # | Yếu tố | Ví dụ | Lý do cần |
|---|--------|-------|-----------|
| 1 | **Prefix** | `day-09-` hoặc `tetcampaign-` | Biết file thuộc project nào |
| 2 | **Concept** | `aodai-traditional` | Biết ảnh nói về gì |
| 3 | **Variant** | `pro` / `basic` / `enhanced` | Biết mức độ prompt nào |
| 4 | **Sequence** | `01`, `02` (nếu cần) | Biết thứ tự trong batch |
| 5 | **Status** | `final` / `v2` / `draft` | Biết version nào dùng được |

→ Ghép thành: `day-09-aodai-traditional-pro-final.png`

Dài nhưng đọc 1 phát hiểu ngay. So với `pro-trad-1.jpg` thì rõ ràng cái nào dễ tìm và share với người khác hơn.

> Yếu tố 4 (sequence) và 5 (status) là **optional** — chỉ thêm khi có nhiều ảnh cùng concept hoặc cần track version. Day 16 batch 15 ảnh mình không dùng sequence vì variant đã đủ phân biệt.

---

## Pattern naming chuẩn — Format đã verify

Sau test thực tế Tuần 2 + Day 16, mình rút ra format:

```
[prefix]-[concept]-[variant]-[seq?]-[status?].png
```

### Ví dụ thực tế từ project mình đã làm

**Day 9 — Áo dài (12 ảnh test):**

```
day-09-aodai-traditional-basic.png        ← Test cấp Basic
day-09-aodai-traditional-advanced.png     ← Test cấp Advanced
day-09-aodai-traditional-pro.png          ← Test cấp Pro
day-09-aodai-modern-basic.png
day-09-aodai-modern-advanced.png
day-09-aodai-modern-pro-final.png         ← Bản chốt dùng cho hero
```

**Day 16 — Batch test (15 ảnh, 5 concept × 3 variant):**

```
day-16-c1-basic-personal-brand.png        ← Concept 1, variant Basic
day-16-c1-enhanced-personal-brand.png     ← Concept 1, variant Enhanced
day-16-c1-pro-personal-brand.png          ← Concept 1, variant Pro

day-16-c2-basic-affiliate-product.png
day-16-c2-enhanced-affiliate-product.png
day-16-c2-pro-affiliate-product.png

day-16-c4-pro-mientay-portrait.png        ← Concept 4 (Miền Tây)
day-16-c5-pro-bad-boy-magazine.png        ← Concept 5 (K-fashion)
```

**Project khách hàng (giả định):**

```
vinamilk-tet2026-banner-pro-v2.png
highland-cafe-product-enhanced-final.png
shopee-flashsale-poster-basic-draft.png
```

### 6 quy tắc kỹ thuật bắt buộc

1. **Toàn lowercase** — không có chữ HOA. `day-09` chứ không `Day-09`
2. **Dấu gạch ngang `-`** ngăn cách — không khoảng trắng, không underscore (trừ status suffix `_final`)
3. **Không dấu tiếng Việt** — `mientay` thay vì `miền tây`
4. **Không ký tự đặc biệt** — không `()[]{}!@#$%^&*` (sẽ break URL, break terminal)
5. **English hoặc romaji Việt** — `aodai`, `mientay`, `phococaodien`
6. **Tên file < 60 ký tự** — quá dài bị cắt ở macOS/Linux

> **Vì sao quy tắc khắt khe?** Tên file này có thể up GitHub, dùng làm URL (Markdown image embed), paste vào tool (Photoshop, ffmpeg). Ký tự đặc biệt + dấu tiếng Việt sẽ break trong các context đó. Mình từng gặp lỗi này khi push ảnh Day 9 lên GitHub — file `áo-dài.png` bị encode thành `%C3%A1o-d%C3%A0i.png` trong URL, hỏng link.

---

## Version control mà không cần Git

Git là tool mạnh nhưng học mất 1-2 ngày. Cho creator AI quản lý ảnh, có cách đơn giản hơn — **suffix versioning**:

### Pattern 4 mức

| Suffix | Ý nghĩa | Khi nào dùng |
|--------|---------|--------------|
| (không suffix) | Bản gốc đầu tiên | Lần test đầu, prompt v1 |
| `_v2`, `_v3` | Bản sửa thứ 2, thứ 3 | Đã chỉnh prompt > 30%, generate lại |
| `_final` | Bản chốt cuối cùng | Đã quyết định dùng cho output |
| `_archive` | Bản backup giữ tham khảo | Không dùng nữa nhưng muốn lưu |

### Ví dụ workflow Day 16 thực tế

```
day-16-c1-pro-personal-brand.png             ← Generate lần 1, prompt 280 từ
day-16-c1-pro-personal-brand_v2.png          ← Sửa prompt: thêm stats numbers
day-16-c1-pro-personal-brand_v3_final.png    ← Bản chốt: dùng làm hero showcase
day-16-c1-pro-personal-brand_v1_archive.png  ← Backup bản gốc
```

Sau 1 tuần thấy không cần `v1` và `v2` (đã chốt v3 rồi) → move vào `02_drafts/old/`. Folder `03_finals/` chỉ giữ file có `_final` suffix.

### Quy tắc khi nào bump version

- **v2:** sửa prompt > 30%, output thay đổi đáng kể (đổi pose, đổi color, thêm element)
- **v3, v4...:** sửa lần 3, 4...
- **final:** đã quyết định dùng cho release/khách hàng
- **archive:** không dùng nữa nhưng cần giữ tham khảo (ví dụ: bản v1 quá đẹp dù không hợp brief)

> Đừng tạo `_v10` `_v15`. Quá nhiều version có nghĩa các bạn chưa quyết được brief. Lúc đó nên review lại yêu cầu trước khi generate tiếp.

### Anti-pattern thường thấy

```
ao-dai-1.png
ao-dai-2.png
ao-dai-3.png
ao-dai-4.png
ao-dai-final.png
ao-dai-final-2.png
ao-dai-final-real.png
ao-dai-FINAL-FINAL.png
```

→ Dấu hiệu các bạn đang lạc trong process. Sửa: pick 1 bản → đổi tên `_final` → archive hoặc delete các bản cũ → focus next task.

---

## Naming convention cho file prompt

### 2 cách quản lý prompt

Mỗi ảnh có thể đi cùng 1 file prompt `.txt` (cùng tên ảnh, khác extension), hoặc gộp tất cả prompt vào 1 file tổng.

**Cách 1 — 1 prompt = 1 file `.txt`:**

```
03_finals/
├── day-16-c1-pro-personal-brand.png
├── day-16-c1-pro-personal-brand.txt    ← Prompt sống cùng ảnh
├── day-16-c2-pro-affiliate-product.png
└── day-16-c2-pro-affiliate-product.txt
```

**Cách 2 — Gộp vào 1 file tổng:**

```
04_prompts/
└── all-prompts.md                       ← 1 file chứa tất cả prompts
```

### So sánh 2 cách

| Cách | Ưu điểm | Nhược điểm | Phù hợp khi |
|------|---------|------------|-------------|
| 1 prompt = 1 file `.txt` | Tự link với ảnh qua tên | Nhiều file rời, folder rối | Project >20 ảnh |
| Gộp `all-prompts.md` | 1 file Ctrl+F nhanh, gọn | Phải copy-paste khi cần | Project <20 ảnh |

→ Mình recommend **cách 1** cho project lớn (>20 ảnh) hoặc khi cần share prompt với người khác. **Cách 2** cho project nhỏ + cá nhân.

Day 16 mình dùng cách 2 (`prompts/day-16.txt` chứa cả 15 prompt) vì đây là test batch — học viên cần download 1 file là đủ. Nhưng nếu là project khách hàng 50+ ảnh, mình sẽ chọn cách 1 để dễ track từng ảnh.

---

## 6 Anti-patterns cần tránh

### 1. Tên có dấu tiếng Việt

❌ `day-09-áo-dài-truyền-thống.png`

→ Khi up GitHub, copy URL paste link, nhiều tool sẽ encode dấu thành `%C3%A1o-d%C3%A0i...` — không đọc được. Một số tool (terminal, ffmpeg) còn báo lỗi không recognize file.

✅ `day-09-aodai-truyenthong.png`

### 2. Khoảng trắng trong tên

❌ `day 09 ao dai pro.png`

→ Terminal phải escape `\ `, URL biến thành `%20`, code script regex hay nhầm.

✅ `day-09-aodai-pro.png`

### 3. Tên quá ngắn không có context

❌ `image1.png`, `output.png`, `final.png`

→ 1 tuần sau quên mất là cái gì. Folder 50 file thì phải mở từng cái xem.

✅ `day-09-aodai-traditional-pro.png`

### 4. Tên quá dài (gồm cả prompt)

❌ `vietnamese-woman-28yo-traditional-ao-dai-with-phoenix-embroidery-and-red-color-shot-on-sony-a7iv-85mm.png`

→ Tên file > 100 ký tự. macOS/Linux có thể bị cắt khi sync cloud. Ngoài ra không đọc được trong file explorer (bị cắt giữa).

✅ Tên gọn `day-09-aodai-traditional-pro.png` + lưu prompt vào file `.txt` riêng cùng tên

### 5. Tên giống nhau, chỉ khác số

❌ `image_1.png`, `image_2.png`, `image_3.png` ... `image_50.png`

→ Sau 50 file mất context hoàn toàn. Phải mở từng cái mới biết là gì.

✅ Mỗi tên có concept rõ ràng: `day-12-color-warm-1.png`, `day-12-color-warm-2.png`...

### 6. Random hash từ tool default

❌ `IMG_DSCF5421.png` (camera default)
❌ `5f3a8b9c.png` (AI tool default)
❌ `output_2026-05-10_14-23-45.png` (timestamp default)

→ Đây là tên default từ camera/AI tool. Phải rename ngay khi save về máy. Đừng lười.

✅ Rename theo convention ngay khi download.

> **Pro tip:** Một số tool (như Photoshop Batch, Bridge) có chức năng "Batch Rename" — chọn 50 ảnh, áp pattern là xong trong 30 giây. Nếu các bạn dùng nhiều, học function này tiết kiệm rất nhiều thời gian.

---

## Mini Challenge — 15 phút

Mở folder ảnh AI hiện tại của các bạn (folder gì cũng được — Tuần 2 ảnh test, hoặc folder Downloads).

**Task:**

1. Pick 5 ảnh bất kỳ
2. Đối chiếu tên hiện tại với 6 anti-patterns ở trên
3. Rename theo format: `[prefix]-[concept]-[variant].png`
4. Note xuống file Notes: tên cũ → tên mới (để track)

**Mục tiêu:** học bằng cách làm thật, không phải đọc xong skip.

Sau khi đổi 5 ảnh, các bạn sẽ thấy folder gọn hẳn. Cảm giác đó là motivation để tiếp tục đổi 50 ảnh tiếp theo.

---

## Cheatsheet 1 trang (dán lên màn hình)

```
┌──────────────────────────────────────────────────────────┐
│  NAMING CONVENTION CHEATSHEET                           │
├──────────────────────────────────────────────────────────┤
│                                                          │
│  Format chuẩn:                                           │
│  [prefix]-[concept]-[variant]-[seq?]-[status?].png      │
│                                                          │
│  6 Quy tắc kỹ thuật:                                    │
│  ✓ Toàn lowercase                                       │
│  ✓ Dấu gạch ngang `-` (không khoảng trắng)              │
│  ✓ Không dấu tiếng Việt                                 │
│  ✓ Không ký tự đặc biệt ()[]!@#                         │
│  ✓ English hoặc romaji Việt                             │
│  ✓ < 60 ký tự                                           │
│                                                          │
│  Version suffix:                                         │
│  (none) → _v2, _v3 → _final → _archive                  │
│                                                          │
│  Examples:                                               │
│  day-09-aodai-traditional-pro.png                       │
│  day-16-c1-pro-personal-brand_v2_final.png              │
│  vinamilk-tet2026-banner-enhanced.png                   │
│                                                          │
│  6 Anti-patterns tránh:                                 │
│  ✗ Dấu tiếng Việt                                       │
│  ✗ Khoảng trắng                                          │
│  ✗ Tên quá ngắn (image1.png)                            │
│  ✗ Tên quá dài (>100 ký tự)                             │
│  ✗ Tên giống nhau khác số                               │
│  ✗ Hash random từ tool default                          │
│                                                          │
└──────────────────────────────────────────────────────────┘
```

---

## 🎓 5 Bài học từ thực tế Tuần 2 + Day 16

### Bài học 1: Đặt tên ngay khi save, đừng để sau

Ban đầu mình hay download cả batch 12 ảnh từ 0ai.vn về với tên default `IMG_5421.png` rồi định "lát rename sau". Lát = 1 tuần sau. Lúc đó quên mất ảnh nào là ảnh nào.

→ Cách fix: **rename ngay tại bước save**. Tốn 10 giây nhưng tiết kiệm 1 tuần đau đầu.

### Bài học 2: Concept name phải nhất quán xuyên project

Day 9 mình test áo dài. Có lúc gọi `traditional`, có lúc gọi `truyenthong`, có lúc gọi `trad`. Đến Day 14 review lại thấy 3 cái cùng nói về 1 thứ.

→ Cách fix: **lock concept name từ đầu project**. Nếu chọn `traditional` thì dùng `traditional` đến cuối, không đổi giữa chừng.

### Bài học 3: Variant naming phải có quy tắc

Day 9 mình dùng `basic`/`advanced`/`pro` (3 mức). Day 16 đổi thành `basic`/`enhanced`/`pro`. Sau Day 14 review thấy `advanced` và `enhanced` có nghĩa khác nhau, nên giữ riêng.

→ Cách fix: **viết ra 1 file `naming-convention.md`** trong root project. Mỗi project mới refer back để đảm bảo nhất quán.

### Bài học 4: Prefix theo project, không theo ngày

Khi làm cho khách hàng, prefix `day-XX-` không phù hợp. Phải đổi thành `vinamilk-tet2026-` hoặc `highland-cafe-product-`.

→ Cách fix: **prefix phản ánh context project**, không phải context cá nhân học.

### Bài học 5: `_final` chỉ dùng 1 lần per concept

Đừng có `_final`, `_final2`, `_final-real`, `_FINAL-FINAL`. Khi đặt `_final` là quyết định cuối. Nếu sau đó muốn sửa nữa → bump lên `_v4` → review lại → đặt `_final` lần nữa.

→ Cách fix: **`_final` = stop sign**. Không qua được nó.

---

## ⚠️ 5 Mistakes các bạn nên tránh

### Mistake 1: Đổi tên file đã upload GitHub/share Drive

Đã upload ảnh lên GitHub repo + share link Zalo group. Sau đó đổi tên local → push lên GitHub → URL cũ broken, người follow click không thấy ảnh.

→ Tránh: **đặt tên cẩn thận từ đầu**. Sau khi đã share, tên file là contract — không đổi được.

### Mistake 2: Đặt convention quá phức tạp ngay từ đầu

Convention 8 yếu tố, 5 cấp version, 12 quy tắc — đẹp về lý thuyết nhưng không ai theo nổi (kể cả mình).

→ Tránh: **bắt đầu với convention đơn giản** (3-5 yếu tố). Sau 1 tháng nếu thiếu mới bổ sung.

### Mistake 3: Dùng số quá dài cho sequence

`day-16-c01-basic-personal-brand-001.png` — đếm 100 ảnh thì cần 3 chữ số, nhưng đếm 15 ảnh chỉ cần `c1` `c2`... Đừng over-engineer.

→ Tránh: **dùng số đủ với scope project**. 15 ảnh: 1-9 đủ. 100 ảnh: 01-99 đủ. 1000 ảnh: 001-999.

### Mistake 4: Mix English và tiếng Việt trong cùng 1 tên

`day-09-aodai-cách-tân-modern.png` — nửa Việt nửa Anh. Inconsistent.

→ Tránh: **chọn 1 ngôn ngữ cho concept name**. Hoặc all English (`aodai-modern`) hoặc all romaji Việt (`aodai-cachtan`). Không mix.

### Mistake 5: Quên rename khi convert format

TinyPNG convert PNG → JPG nhưng giữ nguyên tên `.png`. Hoặc Photoshop save `.png` thành `.jpg.png`. Sau đó link broken.

→ Tránh: **kiểm tra extension** sau mỗi lần convert. Tên file phải match đúng format thực tế.

> Đây là lỗi mình đã gặp ở Day 9 — TinyPNG nén ảnh PNG > 5MB tự động convert thành JPG nhưng tên vẫn `.png`. Reference trong Markdown thành broken. Mất 30 phút tìm chỗ sai.

---

## 🔗 Liên kết với bài khác

- [Day 15 — File & Folder Management](https://github.com/linhai-creator/linh0ai-daily-tutorials/blob/main/days/day-15.md): hệ thống folder để chứa file đã đặt tên đúng convention
- [Day 16 — Workflow Batch Processing](https://github.com/linhai-creator/linh0ai-daily-tutorials/blob/main/days/day-16.md): cách scale 15+ ảnh/giờ, mỗi ảnh có tên chuẩn ngay khi save
- [Day 18 — Editing & Retouching](https://github.com/linhai-creator/linh0ai-daily-tutorials/blob/main/days/day-18.md) (sắp ra): workflow chỉnh ảnh sau generate — bump version đúng cách
- [Day 20 — Templates & Reusable Prompts](https://github.com/linhai-creator/linh0ai-daily-tutorials/blob/main/days/day-20.md) (sắp ra): thư viện prompt dùng lại theo naming convention

---

## 🚀 Day 18 — Sneak peek

Mai mình deep dive **Editing & Retouching ảnh AI**:

- 5 use case phổ biến (rotate, crop, color tweak, background remove, upscale)
- Tool free vs Photoshop — khi nào dùng cái nào
- Workflow batch edit 10+ ảnh trong 5 phút
- Khi nào nên edit, khi nào generate lại trong 0ai.vn

Một insight mình rút ra sau Tuần 2: **70% ảnh AI không cần edit Photoshop** — chỉ cần crop + color tweak nhẹ. Day 18 dạy cách làm điều đó trong 30 giây/ảnh.

---

## 📝 Ghi chú thực hành

Sau khi setup naming convention, các bạn để ý 3 thứ trong tuần đầu:

1. **Mỗi file mới có theo convention không?** — nếu không, force rename ngay khi save về máy
2. **Có file nào còn `image1`, `output.png`, `IMG_xxx.png` không?** — rename hết, đừng để lẫn
3. **`03_finals/` chỉ chứa file `_final` không?** — clean up nếu lẫn version cũ

Đây là tuần đầu — chấp nhận quên vài lần. Tuần thứ 2 quen tay là tự động.

> Sau Day 17, các bạn đã có đủ 3 nền tảng Tuần 3: **hệ thống folder** (Day 15) + **workflow scale** (Day 16) + **naming convention** (Day 17). Day 18-21 sẽ thêm các kỹ năng polish và templates để đóng gói thành 1 production system hoàn chỉnh.

---

## 📍 Navigation

[⬅️ Day 16: Workflow Batch Processing](https://github.com/linhai-creator/linh0ai-daily-tutorials/blob/main/days/day-16.md) | [🏠 README](https://github.com/linhai-creator/linh0ai-daily-tutorials/blob/main/README.md) | [➡️ Day 18: Editing & Retouching](https://github.com/linhai-creator/linh0ai-daily-tutorials/blob/main/days/day-18.md)

## 🏷️ Tags

#0aiVN #Day17Linh0AI #NamingConvention #VersionControl #FileManagement #ProductionWorkflow #PracticalProduction #Tuan3 #ContentCreator #AIWorkflow

---

*Linh0AI Daily Tutorials — Day 17/30 (57%)*
