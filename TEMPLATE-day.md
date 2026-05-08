# 📖 TEMPLATE — File mẫu cho mỗi Day

> **Mục đích:** Template chuẩn để viết bài `day-XX.md` mỗi ngày.
> Copy file này → đổi tên → Find & Replace placeholder → điền nội dung.

---

## 🚀 Cách dùng template (đọc 1 lần, dùng cả 22 Day còn lại)

**Bước 1 — Copy:**
```bash
cp TEMPLATE-day.md days/day-09.md
```

**Bước 2 — Find & Replace** (Ctrl+H trong VSCode/Sublime/Notepad++):

| Tìm | Thay bằng | Ví dụ Day 9 |
|-----|-----------|-------------|
| `{{NUM}}` | Số Day | `09` |
| `{{NUM_PREV}}` | Số Day trước | `08` |
| `{{NUM_NEXT}}` | Số Day sau | `10` |
| `{{TIEU_DE}}` | Tên bài | `Prompt Engineering Nâng Cao` |
| `{{TAGLINE}}` | Phụ đề câu kết | `Từ "biết prompt" lên "prompt như senior"` |
| `{{LEVEL}}` | Cấp độ | `🔵 Intermediate` |
| `{{TIME_DOC}}` | Phút đọc | `12` |
| `{{TIME_TH}}` | Phút thực hành | `45` |
| `{{TUAN}}` | Tuần số | `2` |
| `{{TEN_TUAN}}` | Tên tuần | `Master Skills` |
| `{{TIEU_DE_NEXT}}` | Tên bài Day sau | `Composition & Framing` |

**Bước 3 — Điền nội dung** ở các section comment `<!-- HD: ... -->` (HD = Hướng Dẫn).

**Bước 4 — Xóa phần `📖 HƯỚNG DẪN` này** (từ đầu file đến dòng phân cách `═══`) trước khi commit lên GitHub.

**Bước 5 — Optional:** Xóa comments `<!-- HD: ... -->` nếu muốn, hoặc giữ để dễ update sau.

---

## 📋 Checklist trước khi đăng bài

- [ ] Đã Find & Replace tất cả `{{...}}` placeholder
- [ ] Đã có ít nhất 3 ảnh test (3-5 ảnh là sweet spot)
- [ ] Đã viết "🔥 Insight Linh" ít nhất 2 lần trong bài
- [ ] Đã có Cheatsheet hoặc Bảng tổng kết (nếu phù hợp)
- [ ] Đã viết 3 cấp độ Thử thách (🟢 Newbie / 🔵 Intermediate / 🟣 Pro)
- [ ] FAQ ít nhất 4 câu
- [ ] Navigation links đã update (Day trước/sau)
- [ ] Hashtags ở footer phù hợp với chủ đề
- [ ] Đã update `CHANGELOG.md` thêm dòng Day mới

---

═══════════════════════════════════════════════════════════════
═══ TEMPLATE BẮT ĐẦU TỪ ĐÂY — XÓA MỌI THỨ Ở TRÊN KHI DÙNG ═══
═══════════════════════════════════════════════════════════════

# 🎯 Day {{NUM}} — {{TIEU_DE}}: {{TAGLINE}}

> **Level:** {{LEVEL}}
> **Thời gian đọc:** ~{{TIME_DOC}} phút | **Thực hành:** ~{{TIME_TH}} phút
> **Ngày {{NUM}}/30** | Tuần {{TUAN}} — {{TEN_TUAN}}

---

## 🎬 Mở đầu — <!-- HD: 1 câu hook gây tò mò -->

<!-- HD: Hook 100-200 từ.
- Bắt đầu bằng câu hỏi/observation/insight gây tò mò
- Liên kết với Day trước (1 câu)
- Giới thiệu lý do bài hôm nay quan trọng (2-3 câu)
- Spoiler nhẹ về insight chính của bài (1 câu, gây hứng thú)
- Tone: friendly, conversational. Tránh academic.
-->

---

## 🎯 Mục tiêu hôm nay

<!-- HD: 3-5 bullets. Mỗi bullet bắt đầu bằng động từ (Hiểu/Học/Biết/Có/Master).
     Mỗi bullet phải actionable, đo được. Tránh "biết về X" mơ hồ. -->

- ✅ <!-- Mục tiêu 1 -->
- ✅ <!-- Mục tiêu 2 -->
- ✅ <!-- Mục tiêu 3 -->
- ✅ <!-- Mục tiêu 4 (optional) -->
- ✅ <!-- Mục tiêu 5 (optional) -->

---

## 📚 Phần 1 — <!-- HD: Tiêu đề phần đầu -->

<!-- HD: Phần này thường là "lý thuyết nhẹ" / "tại sao quan trọng".
     Độ dài 200-400 từ. Có thể chia sub-sections (### Sub-title).
     Nên có 1 highlight box "🔥 Insight Linh:". -->

### <!-- HD: Sub-section 1 (optional, dùng khi phần 1 dài) -->

<!-- HD: Nội dung sub-section -->

> **🔥 Insight Linh:** <!-- HD: Bí kíp pro 1-3 câu, ít người dạy -->

### <!-- HD: Sub-section 2 (optional) -->

<!-- HD: Nội dung -->

---

## ⚙️ Phần 2 — <!-- HD: Tiêu đề phần 2 -->

<!-- HD: Phần này thường là "setup" / "cách làm".
     Độ dài 200-400 từ. Nên có:
     - Bảng setting/setup
     - Code block với prompt mẫu
     - Bullet list các bước -->

### Bước 1: <!-- HD: Bước 1 -->

<!-- HD: Mô tả + (nếu có) screenshot path: ![alt text](../assets/images/day-{{NUM}}-step1.png) -->

### Bước 2: <!-- HD: Bước 2 -->

<!-- HD: Mô tả -->

### Bước 3: <!-- HD: Bước 3 (optional) -->

<!-- HD: Mô tả -->

---

## 🧪 Phần 3 — Test thực tế

<!-- HD: Đây là phần "demo" — show prompt + ảnh + phân tích.
     Nếu test 3 model, có 3 sub-section.
     Nếu test 1 model với nhiều variation, dùng 1 sub-section + multiple images. -->

### 📝 Prompt sử dụng

<!-- HD: Hybrid VI+EN, sweet spot 60-150 từ tùy model -->

```
<!-- HD: Prompt thực tế ở đây -->

Negative: <!-- HD: negative prompt nếu có -->
```

### 🖼️ Kết quả

<!-- HD: Đặt path ảnh chuẩn: ../assets/images/day-{{NUM}}-{slug}.png
     slug = mô tả ngắn không dấu, ví dụ: "seedream-portrait", "lighting-rim", "comp-thirds" -->

**<!-- HD: Tên model/variation 1 -->:** *(<!-- giá credit -->)*
![Day {{NUM}} — <!-- alt text -->](../assets/images/day-{{NUM}}-<!-- slug -->.png)

**<!-- HD: Tên model/variation 2 -->:** *(<!-- giá credit -->)*
![Day {{NUM}} — <!-- alt text -->](../assets/images/day-{{NUM}}-<!-- slug -->.png)

**<!-- HD: Tên model/variation 3 -->:** *(<!-- giá credit -->)*
![Day {{NUM}} — <!-- alt text -->](../assets/images/day-{{NUM}}-<!-- slug -->.png)

### 🔍 Phân tích chi tiết

<!-- HD: Bảng so sánh hoặc bullet list các điểm.
     Khi đánh giá: cụ thể, có data, không vague.
     Tránh "ảnh A đẹp hơn" — nói rõ "ảnh A có lỗ chân lông rõ hơn 30%". -->

| Tiêu chí | <!-- Var 1 --> | <!-- Var 2 --> | <!-- Var 3 --> |
|----------|----------------|----------------|----------------|
| <!-- Tiêu chí 1 --> | ⏳ | ⏳ | ⏳ |
| <!-- Tiêu chí 2 --> | ⏳ | ⏳ | ⏳ |
| <!-- Tiêu chí 3 --> | ⏳ | ⏳ | ⏳ |

**🎯 Insight rút ra:** <!-- HD: 1-2 câu kết luận actionable từ test -->

---

## 📊 Phần 4 — Bảng tổng kết / Cheatsheet (optional)

<!-- HD: Phần này OPTIONAL. Chỉ làm nếu nội dung bài cần "1 trang quick ref".
     Bài về model review / skill có nhiều biến → nên có cheatsheet.
     Bài thuần lý thuyết / case study → có thể skip. -->

| <!-- Cột 1 --> | <!-- Cột 2 --> | <!-- Cột 3 --> |
|----------------|----------------|----------------|
| <!-- Row 1 --> | | |
| <!-- Row 2 --> | | |
| <!-- Row 3 --> | | |

---

## 🎁 Phần 5 — Cheatsheet "Khi nào dùng X?" (optional)

### ✅ DÙNG <!-- X --> khi:
- <!-- HD: Use case 1 với mô tả ngắn -->
- <!-- HD: Use case 2 -->
- <!-- HD: Use case 3 -->

### ❌ KHÔNG dùng <!-- X --> khi:
- <!-- HD: Khi nào tránh + alternative -->
- <!-- HD: Khi nào tránh + alternative -->

---

## 💎 Phần 6 — Insights Pro chỉ Linh0AI chia sẻ

<!-- HD: Đây là phần ĐINH của bài — bí kíp ít người dạy cho người Việt.
     3-5 insights. Mỗi insight 50-100 từ. Phải có data hoặc ví dụ cụ thể.
     KHÔNG insight kiểu "hãy luyện tập nhiều" — quá chung chung. -->

**1. <!-- Tên insight -->**
<!-- HD: Mô tả + ví dụ + data nếu có -->

**2. <!-- Tên insight -->**
<!-- HD: Mô tả -->

**3. <!-- Tên insight -->**
<!-- HD: Mô tả -->

**4. <!-- Tên insight (optional) -->**
<!-- HD: Mô tả -->

**5. <!-- Tên insight (optional) -->**
<!-- HD: Mô tả -->

---

## 🎯 Thử thách hôm nay

<!-- HD: 3 cấp độ — newbie / intermediate / pro.
     Mỗi cấp có time + credit dự kiến.
     Task phải actionable trong khung thời gian đó. -->

### 🟢 Cho Newbie (<!-- X --> phút, ~<!-- Y --> credit)
1. <!-- Task 1 -->
2. <!-- Task 2 -->
3. <!-- Task 3 (đăng vào Zalo group với hashtag #Day{{NUM}}Linh0AI) -->

### 🔵 Cho Intermediate (<!-- X --> phút, ~<!-- Y --> credit)
1. <!-- Task 1 -->
2. <!-- Task 2 -->
3. <!-- Task 3 -->

### 🟣 Cho Pro (<!-- X --> phút, ~<!-- Y --> credit)
1. <!-- Task 1 -->
2. <!-- Task 2 -->
3. <!-- Task 3 -->

> 🏆 **Mini Challenge "<!-- TÊN CHALLENGE -->"** vẫn đang chạy đến Day <!-- X -->! Top 3 sẽ được mention trong Day <!-- X -->.

---

## ❓ FAQ

<!-- HD: 4-7 câu Q&A. Mỗi câu trả lời 50-150 từ.
     Anticipate những câu hỏi thật người đọc sẽ hỏi.
     Đừng trả lời "có thể tham khảo Google" — phải có giá trị riêng. -->

**Q1: <!-- Câu hỏi 1 -->?**
<!-- HD: Trả lời -->

**Q2: <!-- Câu hỏi 2 -->?**
<!-- HD: Trả lời -->

**Q3: <!-- Câu hỏi 3 -->?**
<!-- HD: Trả lời -->

**Q4: <!-- Câu hỏi 4 -->?**
<!-- HD: Trả lời -->

**Q5: <!-- Câu hỏi 5 (optional) -->?**
<!-- HD: Trả lời -->

**Q6: <!-- Câu hỏi 6 (optional) -->?**
<!-- HD: Trả lời -->

---

## 🎬 Recap & Day {{NUM_NEXT}}

### Ghi nhớ chính
<!-- HD: 5 bullets ngắn gọn — TLDR của cả bài -->

- ✅ <!-- Point 1 -->
- ✅ <!-- Point 2 -->
- ✅ <!-- Point 3 -->
- ✅ <!-- Point 4 -->
- ✅ <!-- Point 5 -->

### 🔮 Day {{NUM_NEXT}} — Sneak peek
<!-- HD: 2-3 câu tease day sau. Tạo hook để người đọc háo hức. -->

Ngày mai mình sẽ <!-- HD: chủ đề Day next -->. Spoiler: <!-- HD: 1 câu insight gây tò mò -->!

---

## 📍 Navigation
[⬅️ Day {{NUM_PREV}}](./day-{{NUM_PREV}}.md) | [🏠 README](../README.md) | [➡️ Day {{NUM_NEXT}}: {{TIEU_DE_NEXT}}](./day-{{NUM_NEXT}}.md)

## 🏷️ Tags
<!-- HD: 6-10 hashtag. Bắt buộc có: #0aiVN #Day{{NUM}}Linh0AI.
     Còn lại là hashtag chuyên đề + tiếng Việt. -->

`#0aiVN #Day{{NUM}}Linh0AI <!-- + 4-8 hashtag khác -->`

---

> **💌 Có ý kiến hoặc trải nghiệm khác?**
> Comment vào [bài Facebook Day {{NUM}}](https://facebook.com/daclinh.tran) hoặc nhắn vào [Zalo group](https://zalo.me/g/umthmp096). Mình rất muốn nghe góc nhìn khác từ bạn!

---

*Nhật ký Day {{NUM}} by **Linh0AI** — chuỗi 30 ngày làm chủ AI tạo ảnh & video trên 0ai.vn 🇻🇳*
