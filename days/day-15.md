# 📁 Day 15 — File & Folder Management

> **Tuần 3 — Practical Production | Bài 1/7**
> *Đặt nền cho 1 năm làm content AI không hỗn loạn*

---

## 🎯 Mục tiêu Day 15

Sau bài này, các bạn sẽ:

- Có **1 hệ thống folder duy nhất** cho toàn bộ ảnh AI từ nay về sau
- Biết tại sao **Project-based** thắng Date-based và Type-based với content creator
- Setup được hệ thống trong **30 phút** trên laptop/PC
- Tránh được **7 anti-patterns** mà 90% người làm AI mắc phải
- Tìm lại được ảnh đẹp tháng trước trong **dưới 10 giây**

---

## 😤 3 nỗi đau ai cũng từng gặp

Trước khi nói giải pháp, mình muốn các bạn tự hỏi 3 câu:

> **1. "Cái ảnh áo dài đẹp tháng trước mình để đâu rồi?"**
> *(Và sau 15 phút lục Downloads, vẫn không thấy)*

> **2. "Folder Downloads có 500 ảnh AI lẫn lộn — cái nào dùng được?"**
> *(Mở từng cái một, mở 50 cái thì bỏ cuộc)*

> **3. "Đẹp thật, nhưng prompt nào tạo ra ảnh này nhỉ?"**
> *(Và rồi không bao giờ tái tạo lại được vibe đó nữa)*

Nếu các bạn gật đầu ít nhất **2/3** câu → bài này dành cho các bạn.

Tin vui: đây không phải lỗi của các bạn. Đây là lỗi **không có hệ thống** — và hệ thống thì học được trong 30 phút.

---

## 🧠 Mindset đầu tiên: Ảnh AI = Digital Asset

Đây là chỗ 90% người làm content AI sai ngay từ đầu.

| Cách nghĩ SAI | Cách nghĩ ĐÚNG |
|---------------|-----------------|
| "Ảnh AI generate dễ, mất là tạo lại được" | "Mỗi ảnh đẹp = công sức + credit + may mắn — không tái tạo 100%" |
| "Để Downloads cũng được, lúc nào cần thì lục" | "Ảnh AI là **asset**, phải có chỗ ở chính thức" |
| "Prompt trong head, không cần lưu" | "Prompt = formula → mất prompt là mất công thức" |

**Sự thật phũ phàng:** một ảnh GPT Image 2 đẹp tốn **900 credit ≈ 9.000 VND**. 100 ảnh đẹp = **900.000 VND**.

Các bạn không vứt 900k vào Downloads rồi quên, đúng không? Vậy thì cũng đừng vứt ảnh AI vào đó.

---

## 🤔 Vì sao Project-based? So sánh 4 approach

Có 4 cách phổ biến để tổ chức ảnh AI. Mình đã thử cả 4 và đây là đánh giá thật:

### Bảng so sánh

| Approach | Ưu | Nhược | Phù hợp ai |
|----------|-----|--------|-------------|
| **Date-based** (`2026/05/09/`) | Sequential, đơn giản | Tìm theo client/job → khó | Hobbyist log thuần |
| **Type-based** (`portrait/`, `landscape/`) | Tìm nhanh theo loại ảnh | Scatter cùng 1 project | Photographer chuyên 1-2 type |
| **Project-based** (`TetCampaign/`) | Đóng gói được, dễ deliver | Cần định nghĩa "project" rõ | **Freelancer + Content Creator** |
| **Hybrid** (Project + Date) | Linh hoạt | Phức tạp setup | Pro studio team |

### Vì sao Project-based thắng?

**Lý do 1: Đóng gói được**
Khi xong job, các bạn **zip 1 folder duy nhất** gửi client. Date-based thì phải lục từng ngày, Type-based thì phải lục từng folder.

**Lý do 2: Deliver dễ**
Client hỏi "gửi mình tất cả ảnh chiến dịch Tết" → các bạn gửi 1 folder. Xong.

**Lý do 3: Tìm theo TIME đã có sẵn**
Mỗi file đều có timestamp. Cần tìm "ảnh tháng 5" → search hệ thống ra ngay. Không cần folder timeline.

**Lý do 4: Tìm theo TYPE đã có sẵn**
Tag, metadata, search filename — đủ rồi. Không cần folder type.

**Lý do 5: Tìm theo PROJECT thì BẮT BUỘC phải có folder**
Đây là chiều mà OS không tự lo cho các bạn. Nên các bạn phải tự build.

### Cảnh báo: Project-based KHÔNG dành cho ai?

- Người chỉ generate ảnh **cho vui, không có mục đích cụ thể** → Date-based đơn giản hơn
- Người làm **microstock** bán ảnh lẻ → Type-based + tag tốt hơn
- Người **chỉ test prompt** không lưu lâu dài → 1 folder duy nhất là đủ

Còn lại — content creator, freelancer, agency, người làm marketing — thì Project-based là chuẩn.

---

## 5 Nguyên tắc quản lý file ảnh AI

Đây là 5 nguyên tắc mình rút ra sau khi quản lý **95 ảnh test trong Tuần 2** của Linh0AI Daily Tutorials. Nếu các bạn chỉ nhớ được 5 thứ từ bài này, thì là 5 cái này:

### Nguyên tắc 1: 1 project = 1 folder gốc

**Định nghĩa Project:**
> Một mục đích cụ thể, một deadline, một nhóm deliverables liên quan.

**Ví dụ Project hợp lệ:**
- ✅ "Chiến dịch Tết 2026 cho Vinamilk"
- ✅ "Series áo dài cá nhân tháng 5"
- ✅ "Landing page cà phê Highlands"

**Ví dụ KHÔNG phải Project (sai cách hiểu):**
- ❌ "Tháng 5" *(đây là time period, không phải project)*
- ❌ "Portrait" *(đây là type, không phải project)*
- ❌ "Seedream" *(đây là model, không phải project)*

### Nguyên tắc 2: Numbered prefix để control order

OS sắp xếp folder theo **alphabet**. Tức là `references/` luôn ở dưới `drafts/` dù logic là references phải trước.

**Giải pháp:** đặt số ở đầu.

```
00_brief/          ← ở đầu
01_references/     ← thứ 2
02_drafts/         ← thứ 3
03_finals/         ← thứ 4
04_prompts/        ← thứ 5
05_deliverables/   ← cuối
```

Folder nào quan trọng nhất → số nhỏ nhất.

### Nguyên tắc 3: Inbox riêng biệt — không bao giờ làm việc trong Downloads

**Downloads = nơi mọi thứ đổ về**: hóa đơn, screenshot, file tải, ảnh AI...

Làm việc trong Downloads = mở 1 hộp lẫn lộn 100 thứ để tìm 1 thứ.

**Giải pháp:** có 1 folder `0_INBOX` riêng cho ảnh AI. Mỗi tối:
1. Move ảnh AI từ Downloads → `0_INBOX/`
2. Xử lý từng ảnh trong `0_INBOX/`: vào project nào, hay xóa
3. Đi ngủ với `0_INBOX/` empty

Mình gọi đây là **"Inbox Zero"** cho ảnh AI.

### Nguyên tắc 4: Final = chỉ có 1 version dùng được

**Anti-pattern kinh điển:**
```
final.png
final-v2.png
final-v2-edited.png
final-FINAL.png
final-FINAL-real.png
final-FINAL-real-this-time.png   ← các bạn cười nhưng ai cũng từng làm
```

**Giải pháp:** folder `03_finals/` chỉ chứa version **chốt cuối cùng**. Cũ thì move vào `02_drafts/old/` hoặc xóa.

Quy tắc: **mở `03_finals/` là dùng được ngay, không phân vân.**

### Nguyên tắc 5: Prompt log đi cùng ảnh — không tách rời

Các bạn KHÔNG bao giờ được lưu:
- Ảnh trong Google Drive
- Prompt trong Apple Notes
- Reference trong Pinterest

→ Sau 3 tháng các bạn không bao giờ ghép lại được.

**Giải pháp:** prompt sống cùng ảnh trong cùng project folder.

```
03_finals/
├── hero-shot.png
└── hero-shot.txt          ← prompt ngay cạnh ảnh

04_prompts/
└── all-prompts.md         ← log tổng
```

> Day 17 mình sẽ deep dive Naming Convention để file `hero-shot.png` và `hero-shot.txt` tự link với nhau qua tên. Day 20 sẽ build thư viện reusable prompts. Tuần 3 là 1 hệ thống — không phải 7 bài rời.

---

## 🏗️ Folder Structure chuẩn — Full tree

Đây là cây thư mục mình đề xuất. Các bạn copy y nguyên cũng được:

```
📁 AI-Content/                          ← ROOT duy nhất, đặt ở Documents/
│
├── 📁 0_INBOX/                         ← Landing zone cho ảnh mới
│   └── (ảnh từ 0ai.vn download về đây trước)
│
├── 📁 1_PROJECTS/                      ← Projects ACTIVE (đang làm)
│   │
│   ├── 📁 2026-05_TetCampaign-Vinamilk/
│   │   ├── 📄 README.md                ← brief, deadline, status
│   │   ├── 📁 00_brief/                ← yêu cầu khách hàng
│   │   ├── 📁 01_references/           ← moodboard, ảnh tham khảo
│   │   ├── 📁 02_drafts/               ← ảnh AI draft, v1, v2...
│   │   ├── 📁 03_finals/               ← chốt - dùng được ngay
│   │   ├── 📁 04_prompts/              ← log prompts đầy đủ
│   │   └── 📁 05_deliverables/         ← đóng gói cho client
│   │
│   ├── 📁 2026-05_AoDaiPortrait-Personal/
│   │   └── (cấu trúc giống trên)
│   │
│   └── 📁 2026-04_HoiAn-LandscapeSeries/
│       └── (cấu trúc giống trên)
│
├── 📁 2_ARCHIVE/                       ← Projects DONE > 3 tháng
│   ├── 📁 2025-Q4/
│   └── 📁 2025-Q3/
│
├── 📁 3_TEMPLATES/                     ← Reusable assets
│   ├── 📁 prompt-templates/            ← template prompts hay dùng
│   ├── 📁 reference-packs/             ← bộ ảnh tham khảo tái sử dụng
│   └── 📄 _readme-template.md          ← template README cho project mới
│
└── 📁 4_TRASH/                         ← Chuẩn bị xóa, giữ 30 ngày
    └── (ảnh không xài nữa, để 30 ngày rồi xóa hẳn)
```

### Giải thích từng folder

**`0_INBOX/`** — Landing zone
Tất cả ảnh AI mới generate xuống đây trước. Mỗi tối dọn về project tương ứng. **Folder này phải empty trước khi đi ngủ.**

**`1_PROJECTS/`** — Active workspace
Tất cả project đang làm. Mỗi project là 1 folder con với cấu trúc 6 subfolder chuẩn.

**`2_ARCHIVE/`** — Cold storage
Projects xong > 3 tháng → move vào đây để giảm noise. Tổ chức theo Quarter (Q1/Q2/Q3/Q4) hoặc Year.

**`3_TEMPLATES/`** — Reusable
Prompt templates, reference packs, README template — những thứ tái sử dụng cho project mới.

**`4_TRASH/`** — Soft delete
Folder này tồn tại để các bạn **đừng xóa thẳng**. Ảnh xấu/lỗi → move vào `4_TRASH/`. Sau 30 ngày, nếu không tiếc thì xóa hẳn. Vài lần các bạn sẽ "Ơ may quá còn" — đó là lúc folder này cứu đời.

### Tên Project folder — Convention

Format: `YYYY-MM_TenProject-Client`

```
2026-05_TetCampaign-Vinamilk     ✅
2026-05_AoDaiPortrait-Personal    ✅
2026-04_HoiAn-LandscapeSeries     ✅
```

**Tại sao có YYYY-MM ở đầu?**
- Sort tự động theo thời gian
- Biết ngay project khi nào
- Khi archive thì rõ ràng

**Tại sao có dấu `_` và `-` lẫn lộn?**
- `_` ngăn block lớn (date | name | client)
- `-` ngăn từ trong cùng block
- Đọc dễ hơn `TetCampaignVinamilk2026May`

**Tại sao KHÔNG có dấu cách?**
Sẽ giải thích ở phần Anti-patterns 👇

---

## 🔄 Lifecycle 1 ảnh AI — 5 stages

Đây là hành trình 1 ảnh AI đi qua hệ thống của các bạn:

```
   ┌─────────┐    ┌──────────┐    ┌──────────┐    ┌───────────┐    ┌─────────┐
   │ GENERATE │ →  │ 0_INBOX  │ →  │02_drafts │ →  │03_finals  │ →  │2_ARCHIVE│
   │ (0ai.vn) │    │ (1 đêm)  │    │ (1 tuần) │    │  (delivered)   │ (>3 tháng)│
   └─────────┘    └──────────┘    └──────────┘    └───────────┘    └─────────┘
                       ↓               ↓                ↓
                   4_TRASH         4_TRASH          4_TRASH
                   (xấu)           (không pick)    (lỗi sau)
```

### Stage 1: GENERATE
Tạo ảnh trên 0ai.vn → tải về máy → mặc định vào `Downloads/`.

### Stage 2: INBOX (mỗi tối ≤ 5 phút)
Move tất cả ảnh AI từ Downloads về `0_INBOX/`. Đây là **buffer**: ảnh chưa được phân loại, chưa thuộc project nào.

### Stage 3: DRAFTS (trong tuần)
Mở `0_INBOX/` lên → quyết định:
- Ảnh thuộc project nào? → move vào `1_PROJECTS/{project}/02_drafts/`
- Ảnh không dùng? → move vào `4_TRASH/`
- Ảnh hay nhưng chưa rõ project? → tạo project mới hoặc move vào `3_TEMPLATES/reference-packs/`

### Stage 4: FINALS (chốt deliverable)
Trong `02_drafts/` chọn version chốt → move sang `03_finals/`. Lưu prompt cuối cùng vào `04_prompts/`.

### Stage 5: ARCHIVE (sau 3 tháng)
Project xong > 3 tháng → move toàn bộ folder project vào `2_ARCHIVE/{Quarter}/`. Folder `1_PROJECTS/` chỉ giữ những gì đang sống.

> Đây là điểm 70% người làm AI bỏ qua. Họ chỉ nghĩ stage 1-2 (generate + lưu). Stage 3-4-5 mới là chỗ tách người chuyên với người chơi.

---

## 🛠️ Setup Local từ A-Z

### Bước 1: Chọn ổ đĩa và root location

**Recommended:**
- **Windows:** `C:\Users\{Tên}\Documents\AI-Content\`
- **macOS:** `~/Documents/AI-Content/`

**Tại sao Documents/?**
- Được Time Machine (Mac) / File History (Windows) backup mặc định
- Dễ tìm, dễ sync sau này (khi các bạn upgrade lên Cloud)
- Không nằm trong Downloads (vốn dễ bị clean nhầm)

**Cảnh báo:** **KHÔNG** đặt trong:
- Desktop *(rối mắt, dễ kéo nhầm)*
- Downloads *(dễ bị các tool dọn rác xóa nhầm)*
- OneDrive/iCloud auto-sync folder *(file ảnh AI nặng → tốn tiền cloud + chậm)*

### Bước 2: Tạo cây folder

Mở Terminal/Command Prompt:

**macOS / Linux:**
```bash
cd ~/Documents
mkdir -p AI-Content/{0_INBOX,1_PROJECTS,2_ARCHIVE,3_TEMPLATES/prompt-templates,3_TEMPLATES/reference-packs,4_TRASH}
```

**Windows (PowerShell):**
```powershell
cd $HOME\Documents
New-Item -ItemType Directory -Path "AI-Content\0_INBOX","AI-Content\1_PROJECTS","AI-Content\2_ARCHIVE","AI-Content\3_TEMPLATES\prompt-templates","AI-Content\3_TEMPLATES\reference-packs","AI-Content\4_TRASH"
```

Hoặc các bạn click chuột tạo từng folder cũng được — mất 2 phút.

### Bước 3: Pin vào sidebar

**macOS:** Mở Finder → kéo `AI-Content/` vào sidebar bên trái → giờ truy cập 1 click.

**Windows:** Mở File Explorer → click phải `AI-Content/` → "Pin to Quick Access" → hiện ở sidebar bên trái.

### Bước 4: Tạo project đầu tiên

Tạo `1_PROJECTS/2026-05_FirstProject-Personal/` với 6 subfolder chuẩn:

```bash
cd AI-Content/1_PROJECTS
mkdir -p 2026-05_FirstProject-Personal/{00_brief,01_references,02_drafts,03_finals,04_prompts,05_deliverables}
```

### Bước 5: Tạo README.md template

Trong `3_TEMPLATES/_readme-template.md`:

```markdown
# {Project Name}

**Client:** {Tên khách / Personal}
**Started:** YYYY-MM-DD
**Deadline:** YYYY-MM-DD
**Status:** 🟡 In Progress | 🟢 Done | 🔴 On Hold

## Brief
{Yêu cầu ngắn gọn}

## Deliverables
- [ ] 5 ảnh hero (16:9, 4K)
- [ ] 10 ảnh social (1:1, 2K)
- [ ] Source files

## Models used
- GPT Image 2: {credit dùng}
- Seedream 4.5: {credit dùng}

## Notes
{ghi chú quan trọng, learnings}
```

Mỗi project mới các bạn copy file này vào, đổi tên thành `README.md`, fill thông tin.

### Bước 6: Đổi default download location (optional)

Nếu các bạn download ảnh từ 0ai.vn thường xuyên, có thể set Chrome/Edge download thẳng vào `0_INBOX/`:

**Chrome:** Settings → Downloads → Location → chọn `Documents/AI-Content/0_INBOX`

→ Bỏ qua bước "move từ Downloads", ảnh xuống thẳng INBOX.

⚠️ **Lưu ý:** chỉ làm khi các bạn 95% là tải ảnh AI. Nếu hay tải file khác lẫn vào → đừng đổi, dễ rối.

---

## ⚠️ 7 Anti-patterns thường gặp

Đây là 7 lỗi mình thấy 90% người làm AI mắc. Tránh được hết = các bạn đã hơn đa số.

### ❌ Anti-pattern #1: Làm việc trực tiếp trong Downloads
**Vấn đề:** Downloads là nơi mọi thứ đổ về. Tìm 1 ảnh AI giữa 200 file lẫn lộn = stress.
**Fix:** Có `0_INBOX/` riêng. Mỗi tối move sang.

### ❌ Anti-pattern #2: Tên file vô nghĩa
```
Untitled-1.png
Untitled-2.png
ảnh đẹp.png
ảnh đẹp 2.png
ChatGPT Image May 9 2026.png
```
**Vấn đề:** 6 tháng sau các bạn không nhớ "Untitled-1" là cái gì.
**Fix:** Naming convention chuẩn — sẽ deep dive Day 17.

### ❌ Anti-pattern #3: "Final-FINAL-v2-real-this-time.png"
**Vấn đề:** Folder finals có 5 version "final" → version nào là final thật?
**Fix:** `03_finals/` chỉ có 1 version duy nhất. Cũ → `02_drafts/old/`.

### ❌ Anti-pattern #4: Folder/file có dấu tiếng Việt
```
ảnh áo dài/        ← LỖI
hội an đẹp.png     ← LỖI
2026-05_TếtCampaign/  ← LỖI
```
**Vấn đề:**
- Sync với cloud bị lỗi encoding (file biến mất hoặc tên bị phá)
- Terminal/Command Prompt báo lỗi
- Khi share zip cho client Windows → tên file thành ký tự lạ

**Fix:** **Luôn dùng tiếng Việt KHÔNG dấu** cho tên file/folder. Trong README.md thì viết tiếng Việt có dấu thoải mái.

```
ao-dai-tet-hanoi/           ✅
hoi-an-symmetry-001.png     ✅
2026-05_TetCampaign/        ✅
```

### ❌ Anti-pattern #5: Prompt và ảnh tách rời
**Lỗi điển hình:**
- Ảnh trong Google Drive
- Prompt trong Apple Notes
- Reference trong Pinterest
- Brief trong Gmail

**Vấn đề:** 3 tháng sau ghép lại = không thể.
**Fix:** Mọi thứ liên quan 1 project → trong cùng folder project. README.md link đến brief gốc nếu cần.

### ❌ Anti-pattern #6: Không bao giờ xóa
**Vấn đề:** 2 năm sau ổ cứng đầy 800GB ảnh AI mà 90% là ảnh xấu/test/draft không dùng.
**Fix:** Có `4_TRASH/` để soft-delete. Mỗi quý dọn 1 lần. Đừng tiếc — ảnh xấu càng nhiều, ảnh đẹp càng khó tìm.

### ❌ Anti-pattern #7: Backup = không có
**Vấn đề:** Laptop rớt nước → mất sạch.
**Fix tối thiểu:** Bài này focus Local-only nên mình chỉ nói nguyên tắc:
- Time Machine (Mac) / File History (Windows) auto backup vào ổ ngoài
- Hoặc: copy thủ công folder `1_PROJECTS/` sang USB 1 tuần/lần

> **Khi nào upgrade lên Cloud?** Khi các bạn có > 50GB ảnh asset, hoặc làm việc trên 2+ máy, hoặc client trả $$. Lúc đó setup Google Drive / Dropbox sync `1_PROJECTS/` là đủ. Mình sẽ nói thêm khi nào cần thiết.

---

## 📊 Case Study: Linh0AI quản lý 95 ảnh Tuần 2 ra sao

Mình kể luôn 1 case thật từ chính khóa này — vì lý thuyết suông không đủ thuyết phục.

### Cách mình tổ chức Tuần 2

Repo GitHub `linh0ai-daily-tutorials` của mình có cấu trúc:

```
linh0ai-daily-tutorials/
├── days/
│   ├── day-08.md ... day-14.md      ← tutorials
├── prompts/
│   └── day-08.txt ... day-14.txt    ← prompt logs
└── assets/images/
    ├── day-08-{type}-{subject}.png
    ├── day-09-{type}-{subject}.png
    └── ...                           ← 95 ảnh test
```

Đây là **Type-based + Date-based hybrid** chứ không phải Project-based — vì repo này là 1 series tutorial 30 ngày, mỗi ngày là 1 "project nhỏ".

### Lỗi thực mình đã gặp (các bạn nên tránh)

**Lỗi 1: Inconsistency tên file**
- Day 1-9 mình dùng `day-08-`, `day-09-` (số có 0 đứng trước)
- Day 10+ mình dùng `day-10-`, `day-11-` (số tự nhiên)

**Hậu quả:** sort theo alphabet, `day-10-` đứng **TRƯỚC** `day-09-` vì "1" < "9" trong string sort. Lỗi này giờ project đã sống chung không sửa được nữa.

→ Bài học mình rút ra: quyết định format ngay từ ngày 1. Nếu các bạn nghĩ project sẽ kéo dài 100 ngày → dùng 3 chữ số (`001`, `010`, `099`, `100`). Nếu chỉ 30 → 2 chữ số có 0 đầu (`01`, `09`, `30`).

**Lỗi 2: TinyPNG auto-convert**
Day 9 mình upload ảnh > 5MB lên TinyPNG để nén. TinyPNG **tự động đổi PNG → JPG** với ảnh nặng. Kết quả: file trên local là `.png`, file trên repo là `.jpg` → markdown link gãy.

→ Sau lần đó mình rút ra: tool nén ảnh có thể đổi extension. Sau mỗi lần nén, kiểm tra extension lại. Hoặc dùng tool nén PNG vẫn giữ PNG (squoosh.app).

→ Đây là lý do Day 17 sẽ deep dive **Naming Convention + Version Control** — để đặt tên file mà 6 tháng sau vẫn tìm được, và tránh các bẫy của tool nén/convert.

---

## 🎯 Mini Challenge — 30 phút setup hệ thống

Các bạn dành **30 phút TỐI NAY** làm 4 việc sau. Không trì hoãn — vì mỗi tuần trì hoãn = thêm 100 ảnh AI lẫn lộn trong Downloads.

### ✅ Task 1 (5 phút): Tạo cây folder
- Tạo `~/Documents/AI-Content/` với 5 folder chính: `0_INBOX`, `1_PROJECTS`, `2_ARCHIVE`, `3_TEMPLATES`, `4_TRASH`
- Pin vào Finder/Explorer sidebar

### ✅ Task 2 (10 phút): Migrate 1 project hiện tại
- Chọn 1 project các bạn đang làm (hoặc đã làm gần đây nhất)
- Tạo folder `1_PROJECTS/2026-05_{TenProject}-{Client}/` với 6 subfolder chuẩn
- Move ảnh, prompts, references vào đúng subfolder

### ✅ Task 3 (10 phút): Viết README.md cho project đó
- Copy template README.md ở phần "Bước 5" trong bài
- Điền: brief, deadline, deliverables, models used
- Save trong root folder của project

### ✅ Task 4 (5 phút): Setup quy tắc INBOX Zero
- Đặt **alarm 21:00 mỗi tối** trên điện thoại: "Dọn 0_INBOX"
- Quy tắc: trước khi đi ngủ, `0_INBOX/` phải empty
- Làm 7 ngày liên tiếp = thành habit

---

## 📋 Cheatsheet Day 15

### Folder Structure
```
AI-Content/
├── 0_INBOX/         ← landing zone
├── 1_PROJECTS/      ← active work
├── 2_ARCHIVE/       ← done >3 months
├── 3_TEMPLATES/     ← reusable
└── 4_TRASH/         ← soft delete
```

### Naming Convention (folder)
- Project: `YYYY-MM_TenProject-Client`
- Subfolder: `00_`, `01_`, `02_`... (numbered prefix)
- KHÔNG dấu tiếng Việt, KHÔNG dấu cách

### 5 Nguyên tắc quan trọng
1. 1 project = 1 folder gốc
2. Numbered prefix control order
3. Inbox riêng — không làm việc trong Downloads
4. Final = chỉ 1 version
5. Prompt log đi cùng ảnh

### 7 Anti-patterns nhớ tránh
1. Làm việc trong Downloads
2. Tên file `Untitled-1`, `ảnh đẹp`
3. `final-FINAL-v2-real`
4. Dấu tiếng Việt trong tên file
5. Prompt và ảnh tách rời
6. Không bao giờ xóa
7. Backup = không có

### Lifecycle 1 ảnh
```
GENERATE → 0_INBOX → 02_drafts → 03_finals → 2_ARCHIVE
                ↓        ↓           ↓
             4_TRASH  4_TRASH    4_TRASH
```

---

## 🎓 5 Lessons từ Day 15

**Lesson 1:** Ảnh AI là **digital asset** — không phải junk file. Đối xử như tài sản 9.000đ/ảnh.

**Lesson 2:** **Project-based** thắng cho content creator vì OS đã lo time + type, chỉ project là phải tự build.

**Lesson 3:** Numbered prefix (`00_`, `01_`) là cách rẻ nhất để control order — không cần tool gì.

**Lesson 4:** **Inbox Zero** cho ảnh AI = thói quen 5 phút/ngày, cứu các bạn 5 giờ/tháng.

**Lesson 5:** Quyết định naming convention **ngay từ ngày 1** — vì sửa retroactive hầu như không khả thi (mình đã trải nghiệm với `day-08` vs `day-10`).

---

## ⚠️ 5 Mistakes Linh đã thấy nhiều người mắc

1. **Setup hệ thống nhưng không dùng** → 1 tuần sau quay lại làm việc trong Downloads
2. **Folder structure quá phức tạp** → 10 cấp folder, mở 5 lần mới đến file
3. **Đặt root ở Desktop** → màn hình rối, ảnh hưởng tâm trạng làm việc
4. **Không viết README.md** → 6 tháng sau quay lại không nhớ project làm gì
5. **Đợi "rảnh" mới setup** → không bao giờ rảnh, không bao giờ setup

---

## 🚀 Day 16 Sneak Peek

**Workflow Batch Processing — Scale 10+ ảnh/ngày**

Day 15 các bạn có hệ thống. Day 16 mình sẽ dạy workflow để vận hành hệ thống đó hiệu quả:

- Batch generate 10 ảnh trong 30 phút thay vì 3 giờ
- Template prompt theo batch (không phải gõ lại từ đầu)
- Quy trình review nhanh: **3 giây/ảnh** quyết định keep/trash
- Phím tắt + automation cơ bản (tool free)

Mục tiêu cuối Tuần 3: **làm content AI hàng ngày trong 1 giờ thay vì 4 giờ.**

Day 15 = nền móng. Day 16-21 = vận hành. Đừng skip Day 15 đi thẳng Day 16 — không có nền thì workflow cũng không bền.

---

## 📝 Ghi chú thực hành

Sau khi setup xong, các bạn để ý 3 thứ trong tuần đầu:

1. **`0_INBOX/` có empty được mỗi tối không?** — nếu không, các bạn đang generate quá nhiều hoặc quá lười
2. **Có vào `1_PROJECTS/` đúng chỗ không?** — nếu hay quên, dán cheatsheet folder structure lên màn hình
3. **README.md có viết không?** — nếu skip, project sẽ chết dần

Đây là tuần đầu — chấp nhận là sẽ vụng. Tuần thứ 2 quen tay là tự động.

---

*Day 15 — Tuần 3 Practical Production bắt đầu*
*Linh0AI Daily Tutorials | 14/30 → 15/30*

#Linh0AI #AIArtVN #FileManagement #PracticalProduction
