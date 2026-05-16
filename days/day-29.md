# Day 29 — Kling Motion 3.0: Thay nhân vật + sao chép chuyển động

[![Demo Day 29 — Kling Motion Character Replace](../assets/images/day-29-video-3-capcut-final-thumbnail.jpg)](https://github.com/linhai-creator/linh0ai-daily-tutorials/raw/main/assets/videos/day-29-video-3-capcut-final.mp4)

🎬 **[Tải video demo Day 29 — Kling Motion Character Replace (final 10s)](https://github.com/linhai-creator/linh0ai-daily-tutorials/raw/main/assets/videos/day-29-video-3-capcut-final.mp4)**

---

**[← Day 28: Tổng kết Tuần 4 + Mini Challenge "Video VN"](./day-28.md)** · **[📚 Mục lục](../README.md)** · **🎉 Day 29 — Bài cuối khóa 29 ngày**

> **Level:** 🟣 Advanced
> **Thời lượng đọc:** 15-20 phút
> **Thực hành:** 60-120 phút
> **Cost actual ước:** ~30-60K VND (1 ảnh + 1 video Kling Motion)

---

## 🎯 Mục tiêu bài học

Sau Day 29, các bạn sẽ biết cách:

- Dùng **Ảnh 1** làm bối cảnh, tư thế, ánh sáng và góc máy gốc
- Dùng **Ảnh 2** làm nhân vật cần thay vào ảnh mẫu
- Tạo **Ảnh 3**: nhân vật mới xuất hiện trong đúng bối cảnh và tư thế của ảnh mẫu
- Dùng **Video 1** làm video chuyển động gốc
- Dùng **Kling Motion 3.0** để tạo **Video 2**: nhân vật mới sao chép chuyển động từ video gốc
- Ghép/chỉnh lại bằng **CapCut** để tạo **Video 3** hoàn chỉnh

→ Workflow này cực kỳ valuable cho **UGC content · KOL AI · fashion · cosplay · viral re-creation**.

---

## 📖 Brief project

Mình demo workflow thay nhân vật A trong video gốc bằng nhân vật B — giữ nguyên identity nhân vật B (mặt, tóc, trang phục, phụ kiện) và sao chép motion (chuyển động, camera, tư thế) từ video gốc.

**Stack tools dùng:**

- 🎨 Image AI: **GPT Image 2** hoặc **NBN2** (trên 0ai.vn)
- 🎬 Video AI motion: **Kling Motion 3.0** (trên 0ai.vn)
- ✂️ Edit: **CapCut** (miễn phí)

---

## 📄 Prompt file

Tất cả prompts (1 cho image generation VN + 1 cho Kling Motion EN + 5 backup prompts fix lỗi) có trong file [day-29-prompts.txt](../prompts/day-29-prompts.txt).

---

## 🧠 Tư duy workflow

```text
Ảnh 1: Bối cảnh + tư thế gốc
+
Ảnh 2: Nhân vật cần thay
↓
[Step 1: GPT Image 2 / NBN2]
↓
Ảnh 3: Nhân vật mới khớp bối cảnh/tư thế ảnh mẫu

Ảnh 3
+
Video 1: Video chuyển động gốc
↓
[Step 2: Kling Motion 3.0]
↓
Video 2: Nhân vật mới sao chép chuyển động

Video 2
↓
[Step 3: CapCut edit]
↓
Video 3: Video hoàn thiện
```

---

## 📦 Tài nguyên bài học

| Tài nguyên | Vai trò |
|---|---|
| **Ảnh 1** | Ảnh mẫu gốc: bối cảnh, góc máy, ánh sáng, tư thế |
| **Ảnh 2** | Nhân vật cần thay vào ảnh mẫu |
| **Ảnh 3** | Ảnh kết quả sau khi thay nhân vật |
| **Video 1** | Video gốc có chuyển động cần sao chép |
| **Video 2** | Video tạo từ Kling Motion 3.0 |
| **Video 3** | Video hoàn thiện sau khi ghép/chỉnh trong CapCut |

---

## 🛠️ Bước 1 — Tạo ảnh nhân vật mới trên 0ai.vn

**Model khuyên dùng:**

- 🟪 **GPT Image 2** — ổn định, ít miss prompt
- 🟨 **Nano Banana 2** — đa dụng, hiểu tiếng Việt tốt

Mục tiêu của bước này là tạo một ảnh mới trong đó **nhân vật ở Ảnh 2 được thay vào bối cảnh Ảnh 1**, đồng thời **bắt chước tư thế của nhân vật trong Ảnh 1**.

### Ví dụ thực tế của mình

**Ảnh 1 — Bối cảnh + tư thế gốc (mình selfie trong quán container):**

![Ảnh 1 — Bối cảnh gốc](../assets/images/day-29-image-1-boi-canh-goc.png)

**Ảnh 2 — Nhân vật cần thay vào (giữ identity: mặt, mũ, áo, dây chuyền, tattoo):**

![Ảnh 2 — Nhân vật thay thế](../assets/images/day-29-image-2-nhan-vat-thay-the.jpg)

**Ảnh 3 — Kết quả ghép (nhân vật Ảnh 2 vào bối cảnh Ảnh 1, tư thế selfie):**

![Ảnh 3 — Kết quả ghép](../assets/images/day-29-image-3-ket-qua-ghep.png)

→ Identity Ảnh 2 giữ được rất tốt: **mặt · mũ trắng · áo trắng có hoạ tiết · dây chuyền pendant · tattoo tay**. Bối cảnh chuyển từ trong xe (Ảnh 2) sang container quán (Ảnh 1). Ánh sáng đồng bộ tự nhiên.

### Prompt tạo ảnh (Tiếng Việt)

```text
Dùng Ảnh 1 làm bối cảnh chính, giữ nguyên background, ánh sáng, góc máy, màu sắc và bố cục. Dùng nhân vật ở Ảnh 2 để thay vào vị trí nhân vật trong Ảnh 1.

Giữ đúng khuôn mặt, tóc, thần thái, đặc điểm nhận dạng và trang phục gốc của nhân vật Ảnh 2. Không thay đổi kiểu quần áo, màu sắc chính, phụ kiện hoặc phong cách trang phục của nhân vật Ảnh 2.

Cho nhân vật Ảnh 2 bắt chước đúng tư thế nhân vật trong Ảnh 1: dáng đứng/ngồi, hướng mặt, vị trí tay chân, trọng tâm cơ thể, hướng nhìn và tỷ lệ trong khung hình.

Hòa trộn nhân vật thật tự nhiên với bối cảnh Ảnh 1: ánh sáng, bóng đổ, màu da, độ nét và phối cảnh phải đồng bộ. Chỉ điều chỉnh ánh sáng và màu tổng thể trên trang phục để phù hợp môi trường, không đổi thiết kế trang phục.

Kết quả giống ảnh thật chụp cùng lúc, cùng địa điểm, không có cảm giác cắt ghép.

Negative: không đổi background, không thêm người lạ, không đổi mặt, không đổi trang phục nhân vật Ảnh 2, không đổi phụ kiện, không méo tay, không méo mặt, không sai tỷ lệ, không viền cắt ghép, không ánh sáng lệch, không chữ, không logo, không watermark.
```

---

## ✅ Bước 2 — Kiểm tra ảnh trước khi đưa vào Kling Motion 3.0

Ảnh đạt yêu cầu khi:

- ✅ Nhân vật mới giống nhân vật ở Ảnh 2
- ✅ Bối cảnh giữ đúng tinh thần của Ảnh 1
- ✅ Tư thế gần giống nhân vật trong Ảnh 1
- ✅ Ánh sáng, màu da, bóng đổ và độ nét hòa hợp
- ✅ Trang phục/phụ kiện của nhân vật Ảnh 2 được giữ nguyên
- ✅ Không có cảm giác cắt ghép
- ✅ Tay, mặt, mắt, cổ, vai không bị méo

Nếu ảnh chưa đạt, nên tạo lại trước khi đưa sang Kling Motion. **Ảnh đầu vào càng sạch thì video đầu ra càng ổn** — đây là rule #1 của workflow này.

---

## 🎬 Bước 3 — Tạo video bằng Kling Motion 3.0

Trong Kling Motion 3.0, dùng:

- **Ảnh đầu vào:** Ảnh 3 vừa tạo
- **Video tham chiếu:** Video 1 có chuyển động gốc

### Ví dụ thực tế

**Video 1 — Motion reference (mình quay thật, nói chuyện 10s):**

[![Video 1 — Motion gốc](../assets/images/day-29-video-1-motion-goc-thumbnail.jpg)](https://github.com/linhai-creator/linh0ai-daily-tutorials/raw/main/assets/videos/day-29-video-1-motion-goc.mp4)

🎬 [Tải Video 1 — Motion gốc (10s)](https://github.com/linhai-creator/linh0ai-daily-tutorials/raw/main/assets/videos/day-29-video-1-motion-goc.mp4)

**Video 2 — Kling Motion 3.0 output (nhân vật Ảnh 3 sao chép motion + lipsync từ Video 1):**

[![Video 2 — Kling output](../assets/images/day-29-video-2-kling-motion-output-thumbnail.jpg)](https://github.com/linhai-creator/linh0ai-daily-tutorials/raw/main/assets/videos/day-29-video-2-kling-motion-output.mp4)

🎬 [Tải Video 2 — Kling Motion output (10s)](https://github.com/linhai-creator/linh0ai-daily-tutorials/raw/main/assets/videos/day-29-video-2-kling-motion-output.mp4)

→ Identity nhân vật Ảnh 2 giữ được: **mặt · mũ · áo · pendant · tattoo**. Motion + biểu cảm miệng (lipsync) copy từ Video 1 rất tự nhiên.

### Prompt Kling Motion 3.0 (English — recommend)

```text
Use the uploaded image as the main character reference and visual identity.
Use the uploaded video as the motion reference.

Keep the new character from the image exactly the same: face, hairstyle, outfit, accessories, body proportion, lighting style, and overall identity.

Copy the motion, camera movement, body movement, head direction, pose transition, timing, rhythm, and general action from the reference video.

The new character should perform the same movement naturally in the same style, while preserving the background and visual consistency from the input image.

Make the motion smooth, realistic, and physically natural. Keep the character stable and consistent throughout the video.

Do not change the character identity. Do not change the outfit. Do not deform the face, hands, body, eyes, mouth, or accessories. Do not add extra people. Do not add text, logo, watermark, or random objects.
```

---

## 🔧 Bước 4 — Tối ưu prompt nếu video bị lỗi

### ❌ Nếu mặt bị méo hoặc không giống

Thêm dòng này vào cuối prompt:

```text
Prioritize facial consistency and identity preservation over exaggerated motion. Keep the face stable, natural, and recognizable during the entire video.
```

### ❌ Nếu chuyển động quá mạnh

```text
Reduce motion intensity. Keep the movement subtle, smooth, realistic, and natural.
```

### ❌ Nếu nhân vật bị đổi trang phục

```text
Do not change the outfit, color, accessories, hairstyle, or character identity from the input image.
```

### ❌ Nếu tay bị lỗi

```text
Keep hands anatomically correct, natural fingers, no extra fingers, no missing fingers, no twisted hands.
```

### ❌ Nếu camera bị lệch quá nhiều

```text
Maintain the same camera angle, framing, and composition as the input image. The character should move naturally but remain visually consistent with the original image composition.
```

---

## ✂️ Bước 5 — Hoàn thiện bằng CapCut

Sau khi có Video 2 từ Kling Motion 3.0:

1. Mở CapCut
2. Import Video 1, Video 2 và các file âm thanh nếu có
3. Cắt bỏ đoạn lỗi ở đầu/cuối video
4. Giữ đoạn chuyển động đẹp nhất
5. Chỉnh màu nhẹ để video đồng bộ hơn
6. Ghép thêm nhạc, hiệu ứng hoặc text nếu cần
7. Xuất video 1080p hoặc 2K

---

## 💎 5 Insights cho audience

| # | Insight | Detail |
|---|---|---|
| 1 | **Identity vs Motion trade-off** | Kling Motion 3.0 priority motion theo prompt. Khi motion mạnh → identity drift. Thêm "prioritize facial consistency" cứu được |
| 2 | **Ảnh đầu vào quyết định 70% chất lượng** | Ảnh 3 lỗi (mặt méo, ánh sáng lệch) → video output kém. Đầu tư time tạo Ảnh 3 chuẩn trước khi sang Kling |
| 3 | **Trang phục giữ nguyên cần explicit** | Default Kling tendency đổi trang phục khi motion phức tạp. Phải repeat "do not change outfit" trong prompt |
| 4 | **Motion reference video chọn thông minh** | Chọn video có motion vừa phải (không quá nhanh, không quá phức tạp tay). Video dance phức tạp → tay/mặt lỗi cao |
| 5 | **CapCut là final 20%** | Trim đầu/cuối + color grade + audio = critical. Đừng xuất bản video Kling raw |

---

## 💰 Cost actual ước tính

| Item | Quantity | Cost |
|---|---|---|
| Ảnh 3 generate (GPT Image 2 hoặc NBN2) | 1 + 1-2 regen | ~5-15K |
| Video Kling Motion 3.0 | 1 + 1-2 regen | ~25-50K |
| CapCut edit (free tool) | — | 0K |
| **TỔNG ƯỚC TÍNH** | | **~30-65K VND** |

→ Đây là pipeline **cost-efficient** cho UGC content creator — 1 video character-replace 5-10s chỉ ~50K VND.

---

## ⚡ Bài tập thực hành

| Level | Thử thách |
|---|---|
| 🟢 **Newbie** | Thay 1 nhân vật vào ảnh có sẵn, KHÔNG cần motion (chỉ làm Bước 1-2). Output: 1 ảnh nhân vật mới giống ảnh mẫu |
| 🔵 **Trung cấp** | Full workflow với 1 nhân vật + 1 motion video. Output: 1 clip 5-10s nhân vật mới sao chép motion |
| 🟣 **Pro** | Batch — thay **3 nhân vật khác nhau** vào cùng 1 motion video, ghép CapCut so sánh side-by-side. Output: 1 video 15-20s comparison |

---

## ⚠️ Lỗi thường gặp

| Lỗi | Nguyên nhân | Cách xử lý |
|---|---|---|
| Nhân vật không giống Ảnh 2 | Prompt chưa khóa identity đủ mạnh | Nhấn mạnh giữ mặt, tóc, trang phục, phụ kiện |
| Tư thế chưa giống Ảnh 1 | Model hiểu sai vai trò ảnh mẫu | Ghi rõ Ảnh 1 là pose/background reference |
| Video bị méo mặt | Motion quá mạnh | Thêm dòng ưu tiên facial consistency |
| Tay bị lỗi | Tay trong ảnh/video tham chiếu khó | Giảm chuyển động, chọn đoạn video tay ít phức tạp |
| Ánh sáng lệch | Ảnh 2 khác môi trường ảnh 1 quá nhiều | Tạo lại ảnh với yêu cầu đồng bộ ánh sáng mạnh hơn |
| Trang phục bị đổi | Kling default tendency đổi outfit | Repeat "do not change outfit" 2 lần trong prompt |
| Camera lệch quá | Motion video reference khác composition Ảnh 3 | Chọn motion video có framing similar |

---

## ✅ Checklist trước khi xuất bản

- [ ] Ảnh mới giữ đúng nhân vật ở Ảnh 2
- [ ] Bối cảnh vẫn giống Ảnh 1
- [ ] Tư thế nhân vật gần giống Ảnh 1
- [ ] Trang phục nhân vật Ảnh 2 không bị đổi
- [ ] Video Kling sao chép được chuyển động chính từ video gốc
- [ ] Mặt, tay, cơ thể không bị lỗi nặng
- [ ] Video cuối đã được cắt/chỉnh lại bằng CapCut
- [ ] Audio đã được mix balance (BGM + SFX nếu có)
- [ ] Export 1080p hoặc 2K, ratio phù hợp platform target

---

## 💡 Ứng dụng thực tế

Workflow này có thể dùng để:

- 🎬 Tạo video nhân vật mới từ video mẫu
- 📱 Làm content TikTok / Reels viral
- 🎭 Thay nhân vật vào bối cảnh có sẵn
- 👗 Làm video cosplay / fashion / lifestyle
- 💼 Tạo video quảng cáo cá nhân hoặc KOL AI
- 🔄 Tái sử dụng chuyển động từ video cũ để tạo nhân vật mới
- 📊 Re-create viral content với nhân vật riêng (vd: viral dance → nhân vật shop bạn)

---

## ⚖️ Lưu ý đạo đức và quyền sử dụng

Chỉ nên dùng workflow này với hình ảnh/video bạn có quyền sử dụng hoặc đã được sự đồng ý của nhân vật trong ảnh/video.

❌ **Không dùng để:**
- Mạo danh người khác
- Tạo nội dung lừa đảo
- Gây hiểu nhầm về danh tính
- Làm ảnh hưởng đến uy tín / hình ảnh người khác
- Tạo nội dung 18+ không có sự đồng ý

✅ **Use cases an toàn:**
- Tự thay mình vào video viral
- Thay nhân vật avatar tự tạo (không tồn tại thật)
- Thay mẫu shop của bạn (đã có sự đồng ý) vào content
- Cosplay nhân vật fictional (không phải celebrity thật)

---

## 🎉 Cảm ơn các bạn — kết thúc khóa 29 ngày

Day 29 là **bài cuối** của khóa **Linh0AI — 29 ngày làm chủ AI tạo ảnh & video trên 0ai.vn**.

### 📊 Stats khóa học 29 ngày

- **250+ ảnh** AI tạo (chân dung · phong cảnh · sản phẩm · áo dài VN)
- **9+ video** AI (commercial trailer · cinema narrative · character replace)
- **30+ insights verified** — bí kíp từ test thực tế
- **Cost actual:** ~240-460K VND tổng khóa
- **3 Mini Challenges:** Phong cảnh VN · Cảnh phim VN · Video VN

### 🏆 Mini Challenge #3 "Video Việt Nam" — vẫn còn deadline

Các bạn còn cơ hội submit Mini Challenge từ Day 28 — **deadline hết ngày Day 29**. Top 3 work sẽ được mention spotlight trên Facebook Linh0AI + nhóm Zalo cộng đồng.

→ Xem brief đầy đủ trong [Day 28](./day-28.md).

### 🚀 Sau khóa 29 ngày — Khóa 31+ tiềm năng

Nếu cộng đồng vote tiếp, mình sẽ làm khóa 31-60 với 3 modules nâng cao:

| Module | Topic chính |
|---|---|
| 🎵 **Audio Production** | BGM cinematic · SFX layering · Voice-over Việt · Silence drops cho cry-trigger |
| 📱 **Distribution & Multi-Platform** | Adapt 9:16 / 16:9 / 1:1 · Hook A/B testing · Platform-specific algorithms |
| 💰 **Monetization & Creator Economy** | Freelance gig AI content · Build agency · Brand partnership · Creator fund |

→ **Comment vào nhóm Zalo / Facebook Linh0AI nếu muốn khóa 31+** — mình quyết định dựa vào demand thực tế.

### 🎁 Lời cảm ơn

Cảm ơn các bạn đã đồng hành cùng mình suốt 29 ngày. Mỗi insight, mỗi bài học, mỗi đồng credit mình chi đều là **tiền túi thật** — không sponsor, không quảng cáo trá hình.

Hành trình AI của các bạn mới chỉ bắt đầu. Mình mong gặp lại các bạn ở khóa tiếp theo, hoặc đơn giản là thấy work của các bạn lên trend! 🚀

---

**[← Day 28: Tổng kết Tuần 4 + Mini Challenge "Video VN"](./day-28.md)** · **[📚 Mục lục 29 ngày](../README.md)** · **🎉 Day 29 — Bài cuối khóa**

---

*Day 29 hoàn thành — Kling Motion 3.0 Character Replace · 16/05/2026*
*Khóa Linh0AI 29 ngày — Hành trình hoàn thành 🎉*
