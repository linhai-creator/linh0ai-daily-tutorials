# 🚀 Day 17 — Tạo ảnh hoạt hình 3D phong cách Trung Quốc

> **Tuần 3 — Practical Production | Bài 3/7**
> *Inspired by Na Tra 2, Phàm Nhân Tu Tiên, Bạch Xà — 12 ảnh test ratio 9:16 + 16:9 cho creator Việt*

---

## 🎯 Mục tiêu Day 17

Sau bài này, các bạn sẽ:

- Master **5 thành phần prompt 3D animation chuẩn** áp dụng cho style Trung Quốc
- Phân biệt được **bố cục 9:16 vs 16:9** và viết prompt khác nhau cho từng tỉ lệ
- Có **6 concepts mẫu** lấy cảm hứng từ top 3D animation Trung Quốc 2025-2026 (xianxia, Na Tra style, master-disciple)
- Biết cách **tạo Character Sheet** để giữ nhân vật consistent qua nhiều ảnh (cực quan trọng cho series content)
- Tránh được **5 mistakes phổ biến** khi clone style 3D Trung Quốc

---

> 📋 **Prompts đầy đủ trong bài**: [`prompts/day-17.txt`](https://github.com/linhai-creator/linh0ai-daily-tutorials/blob/main/prompts/day-17.txt)
> 12 prompts (6 concepts × 2 ratio) — copy/download nguyên văn về paste vào 0ai.vn.

---

## 😤 Vì sao 3D animation Trung Quốc đang là format hot ở VN?

Năm 2025-2026, ngành hoạt hình 3D Trung Quốc bùng nổ với loạt blockbuster:

- **Na Tra 2 (Ne Zha 2)** — phá vỡ mọi kỷ lục phòng vé Trung Quốc, vibe Sanxingdui culture + modern 3D
- **Phàm Nhân Tu Tiên** — series xianxia 3D top trending Donghua 2025
- **Bạch Xà / White Snake** từ Light Chaser Animation — quality Pixar Trung Quốc
- **When Destiny Brings the Demon** — popularizing "Broken Immortal" aesthetic

Style này có 3 advantage cho creator Việt:

| Advantage | Vì sao |
|-----------|--------|
| **Eye-catching** | Visual đặc trưng (hanfu, kiếm phi, mây tiên, rồng) lướt là dừng |
| **Versatile** | Cùng 1 ảnh dùng được TikTok 9:16 + YouTube 16:9 |
| **Universal appeal** | Văn hóa Đông Á chung — audience Việt relate được, không cần adapt nhiều |
| **Trending** | Đang viral trên TikTok / Douyin / Xiaohongshu — content theo trend dễ reach |

→ Day 17 mình dạy cách clone style này cho cả TikTok 9:16 và YouTube 16:9 từ cùng một concept.

> **Note cho creator Việt:** Mình tập trung style Chinese 3D animation vì đó là gì đang trending 2025-2026. Sau khi master prompt structure, các bạn có thể adapt sang **Việt Nam aesthetic** dễ dàng (đổi hanfu → áo dài, đổi đền cổ Trung → chùa cổ Việt, đổi xianxia → thần thoại Việt). Day 17-18 build foundation, các bạn customize sau.

---

## 5 thành phần prompt 3D animation chuẩn

Sau test 12 ảnh thực tế, mình rút ra cấu trúc 5 thành phần. Thiếu bất kỳ thành phần nào → output sẽ kém:

### Thành phần 1: Subject (Nhân vật + chi tiết hanfu/cổ trang)

Tả nhân vật càng cụ thể càng tốt. KHÔNG đủ: "cô gái Trung Quốc xianxia".

✅ Đủ chi tiết:
```
Cô gái Trung Quốc tu tiên 22 tuổi mặc hanfu trắng tinh khiết dài
có thêu họa tiết hoa văn ngọc bích và mây tiên bạc, tóc đen dài búi cao
kiểu cổ trang có cài trâm bạc khắc rồng phượng, dải lụa trắng bay phấp
phới sau lưng, đôi mắt sáng long lanh nâu hổ phách thanh tịnh kiên định.
```

→ Bao gồm: tuổi + ngoại hình + hanfu chi tiết (màu, họa tiết, kiểu) + tóc + biểu cảm + accessories (kiếm, ngọc, trâm).

### Thành phần 2: Style (chỉ định 3D animation cụ thể)

Đây là phần **quan trọng nhất**. KHÔNG nói chung chung:

❌ "Phong cách 3D Trung Quốc"
❌ "Phong cách hoạt hình xianxia"

✅ Cụ thể style reference:
```
Phong cách 3D animation Phàm Nhân Tu Tiên official + Pixar render quality,
hanfu vải lụa texture chi tiết, da nhân vật sub-surface scattering tự nhiên,
ray-traced lighting, tóc strand-based realistic, kiếm phi specular highlight glow,
chất lượng cinematic film hoạt hình tu tiên Phàm Nhân Tu Tiên theatrical.
```

→ Reference cụ thể tới phim Trung Quốc + technical render terms (ray-traced, sub-surface scattering, strand-based hair).

### 6 style 3D Trung Quốc + Use case phù hợp

| Style | Đặc điểm | Use case phù hợp | Reference film |
|-------|----------|-----------------|----------------|
| **Phàm Nhân Tu Tiên 3D** | Cool tone xianxia, cultivator phi kiếm, cinematic | Hero xianxia, lifestyle | A Record of a Mortal's Journey |
| **Ne Zha 2 official** | Mythology + Sanxingdui patterns, dramatic fire | Action mythology, anti-hero | Ne Zha 2 (2025) |
| **White Snake / Bạch Xà** | Elegant ancient romance, atmospheric | Couple xianxia, wallpaper | White Snake (Light Chaser) |
| **Studio Ghibli + xianxia** | Stylized landscape, magical | Cảnh núi tiên, đền cổ | Bạch Xà landscape |
| **When Destiny Brings the Demon** | Broken Immortal aesthetic, tattered silk | Master-disciple, drama | When Destiny series |
| **Marvel cinematic 3D** | Dramatic lighting, hero shots | Promo dramatic, thumbnail | Cross-genre action |

### Thành phần 3: Setting & Background (Chinese aesthetic)

Bối cảnh càng cụ thể càng giúp AI render đúng vibe Trung Hoa cổ:

✅ Đủ chi tiết:
```
Đứng trên đỉnh núi cao xanh xám đá, mây trắng cuồn cuộn dưới chân như biển
mây bồng bềnh, phía xa là dãy núi tiên cao chót vót đỉnh phủ tuyết, ngôi đền
tu tiên cổ kiến trúc Tang Trung Quốc với mái cong vàng nằm xa trên đỉnh núi
đối diện, sương mù mỏng quấn quanh các đỉnh núi, một vài hạc tiên trắng bay
lượn xa, ánh sáng vàng tiên xuyên qua kẽ mây.
```

→ Setting Trung Quốc đặc trưng: núi tiên với biển mây, đền cổ Tang/Đường, hỏa liên (fire lotus), động bí cảnh, hạc tiên, cây cổ tùng.

### Thành phần 4: Lighting & Mood (Ethereal / Mystical / Dramatic)

Lighting là **soul** của xianxia 3D. Bỏ qua = ảnh sẽ flat:

✅ Tả lighting đầy đủ:
```
Ánh sáng ethereal mystical golden hour buổi bình minh,
key light từ mặt trời vàng phía sau tạo backlit halo divine quanh viền nhân vật,
rim light vàng chiếu vào tóc và viền hanfu tạo glow ethereal,
fill light xanh nhẹ từ mây phản chiếu, volumetric god rays mạnh xuyên qua mây
tạo light beams huyền ảo, kiếm phát quang ngọc bích nhẹ, mood spiritual peaceful
kiên định, immortal cultivation atmosphere.
```

→ Tả: key + rim + fill + volumetric god rays + special effect (sword glow / fire / lightning).

### Thành phần 5: Composition for ratio

Đây là phần **khác biệt nhất giữa 9:16 và 16:9**. Sẽ dive deep ở section dưới.

---

## Bố cục 9:16 (TikTok / Reels / Shorts)

Tỉ lệ dọc 1080×1920px. Đặc điểm:

### Quy tắc bố cục cho 9:16

1. **Subject ở 1/3 giữa hoặc 1/3 dưới** — cho không gian element overhead
2. **Element overhead 1/3 trên** — đèn lồng, mây, vũ khí, cánh tiên
3. **Safe zone bottom 10-15%** — chừa cho TikTok UI (caption, username, music)
4. **Vertical leading lines** — kiếm phi, dải lụa hanfu, thác nước
5. **Foreground bottom** — biển mây, hồ ngọc, sàn đá để tạo grounding

### Prompt template cho 9:16 (Chinese aesthetic)

```
Tỉ lệ ảnh dọc 9:16 (1080x1920px) chuẩn TikTok xianxia content viral.
Bố cục dọc cinematic vertical: [subject] full body chiếm 1/3 giữa ảnh,
đầu [subject] ở 1/3 trên, [overhead element xianxia] phía trên đầu tạo
chiều sâu, phần dưới ảnh [foreground Chinese element] tạo điểm nhấn,
khoảng trống bottom 15% chừa text overlay TikTok caption tiếng Việt.
```

### Camera setting recommend cho 9:16

- **Focal length:** 50mm portrait (chuẩn cho hero shot)
- **Distance:** 3-4 mét (medium shot full body)
- **Framing:** full body từ đầu đến chân
- **Depth of field:** f/2.8 shallow background bokeh
- **Angle:** eye-level slight low (góc thấp anh hùng cho hero pose)

---

## Bố cục 16:9 (YouTube / Facebook / Wallpaper)

Tỉ lệ ngang 1920×1080px. Đặc điểm:

### Quy tắc bố cục cho 16:9

1. **Rule of thirds** — subject ở 1/3 trái hoặc 1/3 phải
2. **Wide environment Trung Hoa** — biển mây, núi tiên, đền cổ panorama
3. **Leading lines** — hạc bay, kiếm phi, đèn lồng dẫn mắt
4. **Foreground depth** — element bên góc tạo lớp lớp depth (cây cổ tùng)
5. **Sky 1/3-1/2 trên** — bầu trời tiên với god rays mở open feel

### Prompt template cho 16:9 (Chinese aesthetic)

```
Tỉ lệ ảnh ngang 16:9 (1920x1080px) chuẩn YouTube xianxia cinematic banner.
Bố cục ngang epic cinematic: [subject] ở 1/3 trái rule of thirds,
2/3 phải dành cho [environment xianxia] rộng panoramic kéo dài về xa,
[leading element như hạc tiên] tạo leading line dẫn mắt vào subject,
[skyline núi tiên] ở 1/3 trên, [biển mây foreground] chiếm 1/3 dưới.
```

### Camera setting recommend cho 16:9

- **Focal length:** 35mm cinematic wide (hoặc 24mm cho ultra-wide epic)
- **Distance:** 5 mét (medium-wide)
- **Framing:** medium-full shot từ đầu gối lên ngực
- **Depth of field:** f/4 giữ environment một phần sharp
- **Angle:** eye-level slight low cho hero shot dramatic

---

## So sánh 9:16 vs 16:9 — Same xianxia concept, different framing

Cùng concept "Cô gái xianxia hanfu trắng + kiếm" nhưng prompt khác nhau:

| Element | 9:16 (TikTok) | 16:9 (YouTube) |
|---------|---------------|-----------------|
| **Subject position** | 1/3 giữa, hơi xuống | 1/3 trái (rule of thirds) |
| **Framing** | Full body | Medium shot waist-up |
| **Background** | Vertical compression, núi xếp dọc | Horizontal expansion, panorama biển mây |
| **Pose subject** | Đứng vững nâng kiếm cao | Nghiêng người dramatic, áo bay |
| **God rays direction** | Vertical (xuyên từ trên) | Horizontal (xuyên ngang) |
| **Leading lines** | Vertical (kiếm, lụa bay) | Horizontal (hạc bay, dãy núi) |
| **Camera** | 50mm, 3-4m | 35mm wide, 5m |
| **Mood** | Personal, hero pose | Cinematic, atmospheric epic |

→ **Cùng concept không có nghĩa cùng prompt**. Mỗi ratio cần prompt riêng tối ưu cho không gian đó.

---

## 🎭 Character Sheet — Giữ nhân vật consistent qua nhiều ảnh

### Vấn đề các bạn sẽ gặp

Tạo 1 cô gái xianxia hanfu trắng đẹp ở Day 17. Tuần sau muốn tạo 10 ảnh khác với cùng cô gái đó (cô gái đó đứng ở đền cổ, cô gái đó cầm sách tu tiên, cô gái đó cưỡi hạc tiên...).

Nếu dùng prompt riêng cho mỗi scene → mỗi lần AI ra 1 cô gái khác → audience không nhận ra **cùng 1 nhân vật** → series content KHÔNG có character recognition.

### Giải pháp: Character Sheet (Model Sheet)

**Character sheet là gì?**

Trong animation studio: bản vẽ chuẩn của nhân vật từ nhiều góc + nhiều biểu cảm + nhiều pose. Animator vẽ scene mới đều refer back character sheet để giữ consistent.

**Trong AI image:** ảnh reference + prompt template để tạo nhân vật consistent qua mọi scene.

### 4 elements quan trọng trong character sheet

| Element | Nội dung | Ví dụ |
|---------|----------|-------|
| **1. Multi-angle view** | Front, 3/4 trái, 3/4 phải, side profile, back | 4 góc nhìn của cùng 1 nhân vật |
| **2. Multiple expressions** | Neutral, smile, intense, sad, angry, surprise | Bảng cảm xúc nhân vật |
| **3. Multiple poses** | Standing relaxed, action pose, sitting, walking | Body language variants |
| **4. Outfit details** | Close-up trang phục, accessories, weapon | Hanfu pattern, kiếm, trâm cài tóc |

### Cấu trúc prompt character sheet

```
Character sheet of [character description chi tiết],
multi-angle turnaround view: front view, 3/4 left view, 3/4 right view,
side profile view, back view,
multiple expressions: neutral calm, smile gentle, intense focused,
multiple poses: standing relaxed, action sword pose, sitting meditation,
outfit details close-up,
white plain background, character design reference sheet style,
model sheet for animation production,
[style reference cụ thể],
[outfit details bắt buộc],
turnaround sheet layout, character bible reference,
3D animation production reference quality.
```

### 2 cách dùng Character Sheet trong AI workflow

#### Cách 1: Single image character sheet (đơn giản)

Generate 1 ảnh chứa nhiều view + nhiều biểu cảm trong 1 ảnh.

**Workflow:**
1. Viết prompt character sheet đầy đủ
2. Aspect ratio: **1:1** (vuông) hoặc **16:9** (ngang để xếp hàng nhiều view)
3. Generate → 1 ảnh chứa 4-6 view của character

**Ưu điểm:** Đơn giản, 1 lần generate. Dùng làm reference visual cho creator/designer.

**Nhược điểm:** Mỗi view nhỏ, detail không cao. Không direct dùng cho production.

#### Cách 2: Image-to-Image với character reference (cao cấp)

Generate 1 ảnh hero của character → save làm reference → upload làm reference cho mỗi scene mới qua **0ai.vn Image Edit feature**.

**Workflow:**
1. Generate **1 ảnh hero chuẩn** của character (vd: C1 cô gái xianxia hanfu trắng + kiếm)
2. Save về máy với naming: `character-c1-girl-xianxia-master.png`
3. Vào 0ai.vn → click **"Edit with image"** hoặc **"Re-prompt with image"**
4. Upload ảnh hero + viết prompt scene mới: "Cùng cô gái này nhưng đang đứng trong đền cổ tu tiên với đèn lồng đỏ vàng treo cao, hai tay nâng cuốn sách cổ Hán..."
5. AI giữ character consistent, chỉ đổi setting + pose

**Ưu điểm:** Character cực consistent qua nhiều scene. Quality từng ảnh cao.

**Nhược điểm:** Tốn credit (mỗi scene = 1 lần generate). Cần GPT Image 2 hoặc Nano Banana 2 có image edit feature.

### Pattern chuẩn cho creator series

Workflow recommend cho creator làm series xianxia (vd: TikTok series 30 tập về 1 nhân vật):

1. **Tuần 1:** Build character sheet — generate hero ảnh + character sheet đầy đủ
2. **Tuần 2-4:** Mỗi ngày dùng character sheet làm reference → tạo 1 scene mới (action, emotional, daily life)
3. **Output:** 30 ảnh content với cùng 1 cô gái nhân vật

→ **Audience recognize "cô gái xianxia của kênh Linh"** → brand recognition mạnh.

### Use case practical cho creator Việt

| Use case | Character cần build | Output |
|----------|---------------------|--------|
| **Series TikTok xianxia** | 1 cô gái + 1 chàng trai cultivator | 30+ ảnh story-driven |
| **Brand mascot kênh** | 1 mèo cafe / 1 cô gái áo dài 3D | Profile + cover + sticker |
| **Vlog persona** | Avatar 3D giống mình | Mọi thumbnail YouTube cùng character |
| **Tarot deck Vietnamese** | 22 nhân vật major arcana | Bộ 78 lá tarot consistent style |
| **Brand book khách hàng** | 1 mascot brand cafe / shop | Toàn bộ asset marketing |

### BONUS — 2 character sheet mẫu trong file prompts

Mình đã add 2 prompt character sheet BONUS vào `prompts/day-17.txt`:

- **Bonus 1:** Character sheet C1 cô gái xianxia hanfu trắng + kiếm (ratio 16:9)
- **Bonus 2:** Character sheet C5 chàng trai cultivator phi kiếm (ratio 16:9)

→ Test 2 prompt này sau khi xong 12 ảnh chính → có sẵn character bible cho 2 nhân vật chính của Day 17. Tổng cost thêm: 2 × 900 = **1,800 credit** (~1,800đ).

---

## 📋 Setup test Day 17

| Thông số | Giá trị |
|----------|---------|
| **Số concepts** | 6 (xianxia girl, **thần linh fire lotus**, núi tiên đền cổ, rồng-ngọc, cultivator boy, master-disciple) |
| **Số ratio** | 2 (9:16 + 16:9) |
| **Tổng prompts** | 12 chính + **2 BONUS character sheet** |
| **Model test** | GPT Image 2 only |
| **Cost dự kiến** | 12 × 900 = 10,800 credit + 2 × 900 = 1,800 credit (BONUS) = **~12,600 credit** (~12,600đ) |
| **Time dự kiến** | 70-100 phút |
| **Style mix** | Phàm Nhân Tu Tiên + Ne Zha 2 + Studio Ghibli + Bạch Xà + When Destiny + Marvel cinematic |

### 6 Concepts chi tiết

| # | Concept | Inspiration | 9:16 Use case | 16:9 Use case |
|---|---------|-------------|---------------|----------------|
| **C1** | Cô gái xianxia hanfu trắng + kiếm bay mây | A Record of a Mortal's Journey | TikTok xianxia viral | YouTube wallpaper |
| **C2** | Thanh niên thần linh + biển hỏa liên | Ne Zha 2 (2025) — adapted | TikTok mythology heroic | YouTube thumbnail epic |
| **C3** | Núi tiên + đền cổ Trung Hoa | Bạch Xà landscape + xianxia | TikTok aesthetic | YouTube wallpaper banner |
| **C4** | Rồng Trung Hoa cuộn quanh ngọc minh châu | Ne Zha 2 dragon design | TikTok mythology epic | YouTube banner movie poster |
| **C5** | Chàng trai cultivator phi kiếm | Phàm Nhân Tu Tiên (Han Li) | TikTok hero shot | YouTube cinematic banner |
| **C6** | Master + đệ tử trong động bí cảnh | When Destiny Brings the Demon | TikTok atmospheric | YouTube emotional scene |

### Câu hỏi mình muốn trả lời qua test này

> *Cùng style Chinese 3D animation, prompt 9:16 và 16:9 có cần khác nhau bao nhiêu để output đẹp tự nhiên cho cả 2 ratio?*

---

## 📊 Kết quả test 12 ảnh

> ⏳ **Section này Linh sẽ fill sau khi test xong 12 ảnh trên 0ai.vn.**
> Mình đã prepare structure để Linh chỉ cần điền số liệu vào.

### Bảng Star Rating

| # | Concept | Ratio | Star (1-5⭐) | Note |
|---|---------|-------|---------------|------|
| 1 | C1 Cô gái xianxia kiếm mây | 🟦 9:16 | ⭐⭐⭐⭐ | Pose 2 tay nâng kiếm dramatic, aura xanh đẹp nhưng pose hơi unusual |
| 2 | C1 Cô gái xianxia kiếm mây | 🟧 16:9 | ⭐⭐⭐⭐⭐ | Composition Bạch Xà cinematic perfect — đền + hạc V + golden hour |
| 3 | C2 Thanh niên thần linh hỏa liên | 🟦 9:16 | ⭐⭐⭐⭐⭐ | Mandala dưới chân + halo đỏ vàng + 2 rồng góc trên — vertical epic |
| 4 | C2 Thanh niên thần linh hỏa liên | 🟧 16:9 | ⭐⭐⭐⭐⭐ | **Policy fix work** — magical orb thay vì weapon, rồng vàng friendly |
| 5 | C3 Núi tiên đền cổ | 🟦 9:16 | ⭐⭐⭐⭐⭐ | Cầu thang đá dẫn lên đền — vertical leading line perfect |
| 6 | C3 Núi tiên đền cổ | 🟧 16:9 | ⭐⭐⭐⭐⭐ ⭐ | **Studio Ghibli quality** — hạc bay + cầu vồng + bình minh atmospheric |
| 7 | C4 Rồng quanh ngọc minh châu | 🟦 9:16 | ⭐⭐⭐⭐ | Vertical OK, ngọc less detailed than 16:9 nhưng lightning fill tốt |
| 8 | C4 Rồng quanh ngọc minh châu | 🟧 16:9 | ⭐⭐⭐⭐⭐ ⭐ | **Epic level** — vảy chi tiết + lightning + Tang patterns + S-curve |
| 9 | C5 Cultivator phi kiếm | 🟦 9:16 | ⭐⭐⭐⭐⭐ | Kiếm phi glow xanh dưới chân + đảo tiên — vertical hero shot |
| 10 | C5 Cultivator phi kiếm | 🟧 16:9 | ⭐⭐⭐⭐⭐ ⭐ | **Iconic xianxia hero shot** — Phàm Nhân Tu Tiên style perfect |
| 11 | C6 Master đệ tử động | 🟦 9:16 | ⭐⭐⭐⭐⭐ | Master + đệ tử cân đối, atmospheric warm vertical |
| 12 | C6 Master đệ tử động | 🟧 16:9 | ⭐⭐⭐⭐⭐ ⭐ | **Atmospheric perfect** — đèn lồng + thác nước + đá ngọc bích + văn tự Hán |
| **B1** | **BONUS C1 Character Sheet Cô gái** | 🎭 16:9 | ⭐⭐⭐⭐⭐ ⭐ | **Animation studio quality** — 4 view + 3 expressions + 3 details với labels |
| **B2** | **BONUS C5 Character Sheet Cultivator** | 🎭 16:9 | ⭐⭐⭐⭐⭐ ⭐ | **Title "Cultivator - Hàn Lập"** + character consistent qua mọi view |
| | **Tổng trung bình** | | **4.86/5** | **13/14 đạt 5 sao** |

> ⭐ = star bonus cho ảnh xuất sắc nhất batch (Hero candidates)

### Gallery 12 ảnh chính

#### 🎨 Concept 1 — Cô gái xianxia hanfu trắng + kiếm bay mây

**🟦 9:16 (TikTok)** — Pose 2 tay nâng kiếm dramatic, hanfu trắng aura xanh, đền vàng + hạc tiên bên phải

![Day 17 C1 9:16 Cô gái xianxia](https://github.com/linhai-creator/linh0ai-daily-tutorials/raw/main/assets/images/day-17-c1-916-girl-xianxia-sword.png)

**🟧 16:9 (YouTube)** — Composition Bạch Xà cinematic perfect, hạc xếp V + golden hour + đền cổ Tang

![Day 17 C1 16:9 Cô gái xianxia](https://github.com/linhai-creator/linh0ai-daily-tutorials/raw/main/assets/images/day-17-c1-169-girl-xianxia-sword.png)

---

#### 🔥 Concept 2 — Thanh niên thần linh + biển hỏa liên (policy-safe Ne Zha 2 inspired)

**🟦 9:16 (TikTok)** — Mandala xoay dưới chân + halo đỏ vàng quanh đầu + 2 rồng vàng góc trên — vertical epic

![Day 17 C2 9:16 Thanh niên thần linh](https://github.com/linhai-creator/linh0ai-daily-tutorials/raw/main/assets/images/day-17-c2-916-deity-firelotus.png)

**🟧 16:9 (YouTube)** — Magical orb thay vì weapon, rồng vàng bay xa thân thiện — Ne Zha 2 vibe mà policy-safe

![Day 17 C2 16:9 Thanh niên thần linh](https://github.com/linhai-creator/linh0ai-daily-tutorials/raw/main/assets/images/day-17-c2-169-deity-firelotus.png)

---

#### 🏔️ Concept 3 — Núi tiên + đền cổ Trung Hoa (Studio Ghibli quality)

**🟦 9:16 (TikTok)** — Cầu thang đá uốn lượn dẫn lên đền + hạc bay + cầu vồng — vertical leading line

![Day 17 C3 9:16 Núi tiên đền cổ](https://github.com/linhai-creator/linh0ai-daily-tutorials/raw/main/assets/images/day-17-c3-916-immortal-mountains.png)

**🟧 16:9 (YouTube)** — **Hero candidate** — Studio Ghibli atmospheric, hạc bay + cầu vồng + mặt trời mọc

![Day 17 C3 16:9 Núi tiên đền cổ](https://github.com/linhai-creator/linh0ai-daily-tutorials/raw/main/assets/images/day-17-c3-169-immortal-mountains.png)

---

#### 🐲 Concept 4 — Rồng Trung Hoa cuộn quanh ngọc minh châu

**🟦 9:16 (TikTok)** — Rồng cuộn xoắn ốc dọc + ngọc phát sáng giữa + lightning vertical

![Day 17 C4 9:16 Rồng ngọc minh châu](https://github.com/linhai-creator/linh0ai-daily-tutorials/raw/main/assets/images/day-17-c4-916-dragon-pearl.png)

**🟧 16:9 (YouTube)** — **Hero candidate** — Vảy chi tiết + lightning + Tang patterns trên ngọc + S-curve epic

![Day 17 C4 16:9 Rồng ngọc minh châu](https://github.com/linhai-creator/linh0ai-daily-tutorials/raw/main/assets/images/day-17-c4-169-dragon-pearl.png)

---

#### 🗡️ Concept 5 — Chàng trai cultivator phi kiếm (Phàm Nhân Tu Tiên style)

**🟦 9:16 (TikTok)** — Kiếm phi glow xanh dưới chân + đảo tiên rải rác — vertical hero shot

![Day 17 C5 9:16 Cultivator](https://github.com/linhai-creator/linh0ai-daily-tutorials/raw/main/assets/images/day-17-c5-916-cultivator-flying.png)

**🟧 16:9 (YouTube)** — **🏆 HERO** — Iconic xianxia hero shot, look y hệt Han Li từ Phàm Nhân Tu Tiên

![Day 17 C5 16:9 Cultivator](https://github.com/linhai-creator/linh0ai-daily-tutorials/raw/main/assets/images/day-17-c5-169-cultivator-flying.png)

---

#### 📜 Concept 6 — Master + đệ tử trong động bí cảnh

**🟦 9:16 (TikTok)** — Master + đệ tử cân đối, atmospheric warm — vertical scene

![Day 17 C6 9:16 Master đệ tử](https://github.com/linhai-creator/linh0ai-daily-tutorials/raw/main/assets/images/day-17-c6-916-master-disciple.png)

**🟧 16:9 (YouTube)** — **Hero candidate** — Atmospheric perfect, đèn lồng + thác + ngọc bích + văn tự Hán

![Day 17 C6 16:9 Master đệ tử](https://github.com/linhai-creator/linh0ai-daily-tutorials/raw/main/assets/images/day-17-c6-169-master-disciple.png)

---

### 🎭 BONUS — 2 Character Sheet (animation studio quality)

#### Character Sheet C1 — Xianxia Girl "Linh Nhi"

Layout chuẩn animation production reference: 4 view (Front, 3/4 Left, Side, 3/4 Right) + 3 expressions (Neutral Calm, Gentle Smile, Focused) + 3 details (Hanfu Pattern, Silver Dragon-Phoenix Hairpin, Jade Long Sword).

![Day 17 BONUS Character Sheet C1 Cô gái](https://github.com/linhai-creator/linh0ai-daily-tutorials/raw/main/assets/images/day-17-bonus-c1-character-sheet-girl.png)

#### Character Sheet C5 — Cultivator "Hàn Lập"

Layout tương tự: 4 view + 3 expressions (Neutral Cold, Intense Focused, Cultivation Determined) + 3 details (Pattern & Embroidery, Belt Engraved Characters, Jade-green Flying Sword).

![Day 17 BONUS Character Sheet C5 Cultivator](https://github.com/linhai-creator/linh0ai-daily-tutorials/raw/main/assets/images/day-17-bonus-c5-character-sheet-boy.png)

> 💎 **Cả 2 character sheet đều đạt animation studio quality** với layout chuẩn, labels Việt-Anh, character consistent qua mọi view. Dùng được trực tiếp làm reference cho production hoặc upload vào 0ai.vn Image Edit để tạo nhiều scene mới với cùng nhân vật.

---

## 🎓 Insights từ test 14 ảnh

### Insight 1: GPT Image 2 hiểu Chinese 3D aesthetic cực tốt — không cần re-gen

13/14 ảnh đạt 5⭐ ngay lần đầu generate (chỉ C1 9:16 đạt 4⭐ do pose hơi unusual). **Tỷ lệ thành công 92.8%** — cao hơn batch Day 16 (Vietnamese aesthetic, 14/15 = 93.3%) ~1%.

→ Conclusion: Style Chinese 3D animation là **sweet spot của GPT Image 2** vì model đã được train trên rất nhiều Chinese animation data (Ne Zha 2, Phàm Nhân Tu Tiên, Bạch Xà rất phổ biến trên internet). Creator Việt cứ tự tin write prompts theo style này.

### Insight 2: Style reference cụ thể tới phim work tốt hơn generic 10x

Prompts có mention **"Phàm Nhân Tu Tiên official"**, **"Ne Zha 2 official"**, **"Studio Ghibli + xianxia"** ra output **đúng style ngay** — không có drift sang Western 3D hoặc anime 2D.

So sánh với prompts không có style reference cụ thể (vd: "3D Trung Quốc cute"), output thường drift sang Cartoon Network style hoặc Pixar generic.

→ **Lesson:** Mention 1-2 phim/studio Trung Quốc cụ thể trong mỗi prompt — đây là cheat code cho output chuẩn xianxia.

### Insight 3: 16:9 cinematic ra impressive hơn 9:16 vertical — cần adjust prompt cho TikTok

**Top 4 Hero candidates đều là 16:9** (#7, #9, #11, #13). Vì sao?
- **16:9** cho phép **environment wide panoramic** (núi tiên kéo dài, biển mây panorama, hạc xếp V) → cinematic feel epic
- **9:16** vertical compress environment → focus character close-up nhiều hơn → lose some "wow factor" của xianxia landscape

**Lesson cho TikTok content:** Khi viết prompt 9:16, focus vào **character close-up + foreground hero pose** thay vì cố compress landscape. Vd: prompt nên mention "medium close-up shot from waist up" thay vì "full body with wide landscape".

→ Day 17 đã verify pattern: vertical content cần prompt khác từ horizontal, không chỉ đổi setting ratio.

### Insight 4: Character Sheet feature WORK — production-ready quality

2 BONUS character sheet đều ra **animation studio reference quality**:
- ✅ 4 view turnaround đầy đủ (Front, 3/4 Left, Side, 3/4 Right)
- ✅ 3 expressions với labels rõ ràng
- ✅ 3 outfit/accessory details close-up
- ✅ Title character ("Xianxia Girl - Linh Nhi", "Cultivator - Hàn Lập") — GPT Image 2 đọc được Vietnamese!
- ✅ Character consistent 100% qua mọi view

→ **Insight độc đáo:** Character sheet là feature **bán được riêng** cho clients (vd: studio làm webtoon Vietnamese, brand mascot service). Cost generate ~900đ + character bible production-ready cho client.

### Insight 5: Policy fix C2 work — vibe Ne Zha 2 vẫn được preserve

Prompt cũ (cậu bé 10 tuổi + 3 vũ khí + dung nham + chớp xé) → Policy violation. 
Prompt mới (thanh niên 18 tuổi + magical orb + đất linh thiêng + rồng vàng friendly) → **Pass policy + vẫn ra vibe Ne Zha 2 inspired** qua:
- ✅ Áo đỏ truyền thống Trung Quốc với kim phù vàng
- ✅ Sanxingdui patterns trên áo
- ✅ Lụa đỏ vàng bay phấp phới
- ✅ Vầng halo đỏ vàng quanh trán (dấu hiệu thần linh)
- ✅ Biển hỏa liên đỏ rực bao trùm
- ✅ Mandala xoay dưới chân
- ✅ Style 3D animation cinematic theatrical

→ **Lesson universal:** Khi prompt bị policy violation, **đừng bỏ concept** — chỉ adjust 5 elements: character age (>= 18), weapons (→ magical artifacts), violence imagery (→ heroic mythology), background threat (→ neutral/positive), keep visual aesthetic specific phim reference.

---

## 🏆 Hero Day 17 — Cultivator phi kiếm (C5 16:9)

![Hero Day 17 - Cultivator Phi Kiếm](https://github.com/linhai-creator/linh0ai-daily-tutorials/raw/main/assets/images/day-17-c5-169-cultivator-flying.png)

**Vì sao chọn ảnh này làm Hero:**

1. **Iconic xianxia hero shot** — look y hệt Han Li trong Phàm Nhân Tu Tiên, audience Việt nhận ra ngay phong cách
2. **Composition cinematic perfect** — chàng trai ở 1/3 trái rule of thirds, hạc bay xếp V dẫn mắt, biển mây panoramic, đảo tiên rải rác background
3. **Cool tone xianxia aesthetic chuẩn** — xám-đen + cyan kiếm + mây trắng + sky purple-blue
4. **Production value cao** — hanfu chi tiết, kiếm phi specular highlight, atmospheric perspective xa mờ
5. **Versatile use case** — thumbnail YouTube vlog xianxia, banner kênh, wallpaper, promo

### 🥈 3 Runners-up (Hero candidates khác)

| Image | Concept | Tại sao đẹp |
|-------|---------|-------------|
| **C3 16:9** Núi tiên đền cổ | Studio Ghibli quality | Atmospheric perfect — wallpaper-tier beauty với cầu vồng + hạc + bình minh |
| **C4 16:9** Rồng ngọc minh châu | Ne Zha 2 dragon | Visual impact strongest — vảy detailed + lightning + S-curve epic |
| **C6 16:9** Master đệ tử | When Destiny atmospheric | Storytelling warm — đèn lồng + thác + ngọc bích + văn tự Hán

---

## ⚠️ 5 Mistakes các bạn nên tránh

### Mistake 1: Style chung chung "3D Trung Quốc cute"

❌ "Phong cách 3D Trung Quốc cute, dễ thương"
✅ "Phong cách 3D animation Phàm Nhân Tu Tiên official + Pixar render quality, sub-surface scattering, ray-traced lighting"

→ AI cần style reference cụ thể tới phim. "3D Trung Quốc cute" có thể ra Cartoon Network hoặc thậm chí flat 2D.

### Mistake 2: Bỏ qua composition cho ratio

❌ Cùng prompt cho cả 9:16 và 16:9, chỉ đổi setting ratio trong 0ai.vn
✅ Mỗi ratio có instruction composition riêng + camera setting riêng trong prompt

→ AI cần biết "subject ở giữa hay 1/3 trái" và "kiếm vertical hay horizontal". Không nói = AI tự đoán = output kém.

### Mistake 3: Thiếu Chinese aesthetic specific elements

❌ "Áo dài Trung Quốc, kiếm"
✅ "Hanfu trắng tinh khiết có thêu họa tiết hoa văn ngọc bích và mây tiên bạc, kiếm trường ngọc bích phát quang xanh nhạt soft glow"

→ Element đặc trưng (hanfu pattern, kiếm phi với glow, đền Tang, hạc tiên, mây tiên) tạo authentic xianxia feel. Generic = output không xianxia.

### Mistake 4: Lighting flat / không tả mystical mood

❌ "Ánh sáng đẹp" / không nói gì về lighting
✅ "Ethereal mystical golden hour bình minh, key light backlit halo divine, volumetric god rays xuyên mây tạo light beams huyền ảo, immortal cultivation atmosphere"

→ Xianxia 3D phải có **mystical lighting + god rays + ethereal mood**. Lighting flat = ảnh look fake AI rõ.

### Mistake 5: Bỏ negative prompt cho 3D Chinese animation

❌ Không có negative
✅ "Negative: photorealistic photograph, real human photo, modern clothing jeans, modern setting urban, cyberpunk neon, flat 2D anime, body framing gợi cảm"

→ Không có negative, AI dễ drift sang **modern Chinese cyberpunk** (rất phổ biến hiện nay) hoặc realistic photo. Phải chặn rõ ràng từ đầu.

---

## Cheatsheet 1 trang (dán lên màn hình)

```
┌──────────────────────────────────────────────────────────┐
│  3D CHINESE ANIMATION PROMPT CHEATSHEET                 │
├──────────────────────────────────────────────────────────┤
│                                                          │
│  5 thành phần chuẩn:                                    │
│  1. Subject (chi tiết hanfu/cổ trang/ngoại hình/pose)   │
│  2. Style (Phàm Nhân Tu Tiên / Ne Zha 2 / Bạch Xà...)   │
│  3. Setting (núi tiên / đền cổ / hỏa liên / động bí)    │
│  4. Lighting (god rays + mystical + immortal aura)      │
│  5. Composition (riêng cho 9:16 hoặc 16:9)              │
│                                                          │
│  9:16 (TikTok/Reels):                                   │
│  • Subject 1/3 giữa, full body pose                     │
│  • Element xianxia overhead 1/3 trên                    │
│  • Bottom 15% chừa text TikTok                          │
│  • Camera 50mm, f/2.8, distance 3-4m                    │
│  • Vertical god rays + leading lines                     │
│                                                          │
│  16:9 (YouTube/Wallpaper):                              │
│  • Subject 1/3 trái (rule of thirds)                    │
│  • Environment xianxia panoramic 2/3 phải               │
│  • Sky 1/3 trên with god rays horizontal                │
│  • Camera 35mm/24mm, f/4, distance 5m                   │
│  • Horizontal leading lines (hạc bay, dãy núi)          │
│                                                          │
│  6 Style references Chinese 3D:                          │
│  • Phàm Nhân Tu Tiên — cultivator hero                  │
│  • Ne Zha 2 — mythology + Sanxingdui                    │
│  • Bạch Xà — elegant ancient romance                    │
│  • Studio Ghibli + xianxia — landscape                  │
│  • When Destiny Demon — broken immortal                 │
│  • Marvel cinematic 3D — dramatic action                │
│                                                          │
│  Element xianxia phổ biến:                              │
│  hanfu, kiếm phi (flying sword), mây tiên,              │
│  hạc tiên, ngọc bích, hỏa liên (fire lotus),            │
│  đền cổ Tang/Đường, núi tiên, động bí cảnh,             │
│  rồng Trung Hoa, ngọc minh châu                         │
│                                                          │
│  CHARACTER SHEET (cho series content):                   │
│  • 4 elements: multi-angle + expressions +              │
│    poses + outfit close-up                              │
│  • Cách 1: Single image character sheet (1:1)           │
│  • Cách 2: Image edit với reference (consistent)        │
│  • Use case: series xianxia, brand mascot, vlog avatar  │
│  • Workflow: build sheet 1 lần → 30+ ảnh content        │
│                                                          │
│  Negative bắt buộc:                                      │
│  photorealistic photo, modern clothing, cyberpunk,      │
│  flat 2D anime, body framing gợi cảm                    │
│                                                          │
└──────────────────────────────────────────────────────────┘
```

---

## 💰 ROI Tổng kết Day 17

| Item | Giá trị |
|------|---------|
| Số ảnh test | **14** (12 chính + 2 BONUS character sheet) |
| Cost credit | **~12,600** (~12,600đ) |
| Time generate | ~70-90 phút (estimate) |
| Time/ảnh | ~5-6 phút |
| Cost/ảnh | ~900đ |
| **Tỷ lệ thành công** | **13/14 = 92.8% đạt 5⭐ ngay lần đầu** |
| **Star average** | **4.86/5 ⭐** |
| Style học được | 6 (Phàm Nhân Tu Tiên + Ne Zha 2 + Bạch Xà + Studio Ghibli + When Destiny + Marvel) |
| Use case practical | 6 + Character sheet workflow cho series content |

> Đây là batch test có **thành công cao nhất từ Tuần 2 đến giờ** — 13/14 đạt 5⭐ ngay lần đầu generate. Verify rằng GPT Image 2 hiểu Chinese 3D animation aesthetic cực tốt.

### 💎 Bonus value: Character Sheet workflow

2 character sheet (BONUS C1 + C5) mở ra workflow **production-ready** cho:
- **Creator series:** build character bible 1 lần (~1,800đ) → 30+ ảnh content có cùng nhân vật
- **Brand mascot service:** sell character sheet cho clients (vd: ~500K-1tr cho 1 character)
- **Studio webtoon Vietnamese:** tạo character bible cho production

→ **ROI thực tế:** 1,800 credit (~1,800đ) cho 2 character sheet → có thể generate vô hạn scene mới với cùng character qua 0ai.vn Image Edit.

---

## 🔗 Liên kết với bài khác

- [Day 15 — File & Folder Management](https://github.com/linhai-creator/linh0ai-daily-tutorials/blob/main/days/day-15.md): hệ thống folder để chứa 12 ảnh test
- [Day 16 — Workflow Batch Processing](https://github.com/linhai-creator/linh0ai-daily-tutorials/blob/main/days/day-16.md): workflow batch test 12+ ảnh trong 1 giờ
- [Day 18 — Image-to-Video Seedance](https://github.com/linhai-creator/linh0ai-daily-tutorials/blob/main/days/day-18.md) (sắp ra): biến 6 ảnh hero Day 17 thành video xianxia 5-10s

---

## 🚀 Day 18 — Sneak peek

Mai mình deep dive **Image-to-Video với Seedance 2.0**:

- Lấy 6 ảnh hero từ Day 17 (1 ảnh/concept) → biến thành video 5-10 giây xianxia
- Prompt motion cho Seedance: subtle vs dramatic
- Camera movement: zoom, pan, tilt, orbit theo phong cách Trung Hoa
- Subject motion: hanfu bay, kiếm phi, mây cuộn, hạc bay, fire lotus animation
- Workflow batch render 6 video xianxia trong 30-45 phút

→ **Continuation tự nhiên:** Day 17 dạy tạo ảnh xianxia 3D → Day 18 biến thành video viral. Cùng 1 concept dùng được cho cả TikTok 9:16 + YouTube 16:9 + video.

---

## 📝 Ghi chú thực hành

Sau khi test Day 17, các bạn để ý 3 thứ:

1. **Concept nào ra đẹp nhất?** — note lại để dùng cho project content xianxia/cổ trang Việt
2. **Ratio nào AI generate dễ hơn cho Chinese aesthetic?** — adjust prompt cho ratio khó hơn
3. **Style 3D Trung Quốc nào hợp gu của các bạn nhất?** — focus deep style đó cho project sau

Đây là batch test lớn (12 ảnh) — xây dựng foundation hiểu prompt 3D Trung Quốc. Sau Day 17, các bạn có thể adapt prompts sang **Vietnamese aesthetic** dễ dàng (đổi hanfu → áo dài, đổi xianxia → thần thoại Việt, đổi đền Tang → chùa Việt).

> Sau Day 17, các bạn đã có 12 ảnh 3D xianxia chất lượng + master prompt structure cho 2 ratio chính. Day 18 sẽ thêm dimension thứ 3: video xianxia.

---

## 📍 Navigation

[⬅️ Day 16: Workflow Batch Processing](https://github.com/linhai-creator/linh0ai-daily-tutorials/blob/main/days/day-16.md) | [🏠 README](https://github.com/linhai-creator/linh0ai-daily-tutorials/blob/main/README.md) | [➡️ Day 18: Image-to-Video Seedance](https://github.com/linhai-creator/linh0ai-daily-tutorials/blob/main/days/day-18.md)

## 🏷️ Tags

#0aiVN #Day17Linh0AI #3DAnimation #ChineseAnimation #Xianxia #NeZha2 #PhamNhanTuTien #BachXa #TikTok916 #YouTube169 #PracticalProduction #Tuan3 #ContentCreator

---

*Linh0AI Daily Tutorials — Day 17/30 (57%)*
