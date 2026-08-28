# 🏰 Lâu Đài Nguyệt Huyết

Game hành động platformer kiểu Castlevania, chạy hoàn toàn trong trình duyệt. **Một file HTML duy nhất** — không build, không dependency, không server.

▶️ **[Chơi ngay](https://USERNAME.github.io/lau-dai-nguyet-huyet/)** *(thay `USERNAME` bằng tên GitHub của bạn sau khi bật Pages)*

---

## Chơi thế nào

| Bàn phím | Cảm ứng | Hành động |
|---|---|---|
| `←` `→` hoặc `A` `D` | ◀ ▶ | Di chuyển |
| `X` / `K` / `Space` | NHẢY | Nhảy |
| `Z` / `J` | KIẾM | Vung kiếm |
| `↓` | ▼ | Ngồi (chém thấp) |
| `↑` `↓` | ▲ ▼ | Lên xuống cầu thang |
| `↑` + `Z` | ▲ + KIẾM | Ném phụ khí (tốn 1 tim) |
| `Esc` / `P` | ☰ Menu | Tạm dừng |
| `R` | — | Chơi lại màn |
| `F` | ⛶ | Toàn màn hình |

> 📱 **Trên điện thoại nên xoay ngang** — khung game lớn hơn khoảng 1,8 lần, nút bấm dạt về hai góc dưới.

---

## Có gì trong game

**Hai nhân vật**, chọn ở màn tiêu đề:

| | HP | Tốc độ | Nhảy | Vung kiếm |
|---|---|---|---|---|
| **Kiên** — bền bỉ | 16 | 1.45 | 6.6 | chuẩn |
| **Nguyệt** — nhanh nhẹn | 13 | 1.78 | 7.1 | nhanh hơn 3 frame |

**Năm loại kiếm**, mỗi cây một tính cách chứ không phải nâng cấp tuyến tính:

| Kiếm | Tầm | Sát thương | Frame | DPS |
|---|---|---|---|---|
| Đoản kiếm | 30 | 2 | 18 | 6.7 |
| Trường kiếm | 42 | 3 | 18 | 10.0 |
| Đại kiếm | 54 | 4 | 18 | 13.3 |
| Katana | 46 | 3 | 11 | 16.4 |
| Huyết kiếm | 40 | 3 | 14 | 12.9 |

- **Katana** — chiêu rút chém ngang (iai), tầm ngắn hơn Đại kiếm nhưng vung nhanh gần gấp đôi
- **Huyết kiếm** — hút 1 HP mỗi nhát trúng, nhưng tự rút 1 HP mỗi 4,5 giây. Đứng yên là yếu dần, xông lên là mạnh lên. Không bao giờ tự giết bạn (sàn chặn ở 2 HP)

**Ba phụ khí**: dao (nhanh, thẳng), rìu (bay vòng cung, xuyên nhiều địch), nước thánh (cháy lan trên sàn).

**Hai màn**, mỗi màn một boss:

- **Màn 1 — Tiền đình** (3440px): zombie, dơi, khung xương, đầu Medusa
  → **Tử Thần**: dịch chuyển tức thời, ném lưỡi hái truy đuổi, lao xuống sàn tạo cửa sổ phản công
- **Màn 2 — Hầm mộ** (3712px): thêm hunchback, đèn chùm rơi, bãi gai, bục di chuyển
  → **Bá Tước Huyết Nguyệt**: giai đoạn 1 đứng sàn bắn cầu lửa, dưới nửa máu mọc cánh, lao ngang và rải dơi

**Điểm cao** lưu qua các lần chơi (top 5, kèm nhân vật và màn đạt được).

---

## Ghi chú kỹ thuật

Viết tay bằng Canvas 2D thuần, không dùng engine hay thư viện.

- **Pixel art sinh bằng code** — không có file ảnh nào. Nhân vật, quái, boss đều vẽ bằng `fillRect` với bảng màu cố định và nguồn sáng nhất quán
- **Viền tối tự động** — mỗi sprite render vào canvas phụ, lấy silhouette tô màu tối rồi dập 4 hướng lệch 1px trước khi vẽ sprite thật. Hiệu ứng bán trong suốt (hào quang, vệt lao) vẽ riêng để không bị viền
- **Supersampling 2×** — canvas nội bộ 1024×576, `setTransform(2,2)` nên code vẽ vẫn dùng toạ độ 512×288. Chữ HUD sắc nét kể cả khi thu nhỏ trên điện thoại
- **Cảm ứng hit-test theo toạ độ** thay vì gắn event lên từng nút, để trượt ngón giữa các nút vẫn đổi hướng được (chạm cảm ứng có implicit pointer capture nên cách gắn event thông thường không xử lý được)
- **Điều khiển có bộ đệm nhảy 9 frame và coyote time 7 frame**, lái nhẹ trên không
- Nhạc chip và toàn bộ âm thanh sinh bằng WebAudio, không có file audio
- Lưu điểm qua `window.storage`, tự xử lý khi không có bộ lưu

---

## Chạy tại máy

Chỉ cần mở `index.html` bằng trình duyệt. Không cần server.

Nếu muốn chạy qua HTTP:

```bash
python3 -m http.server 8000
# rồi mở http://localhost:8000
```

---

## Giấy phép

MIT — xem file [LICENSE](LICENSE). Dùng, sửa, chia sẻ thoải mái.

---

<details>
<summary><b>English summary</b></summary>

A Castlevania-style action platformer that runs entirely in the browser from a **single HTML file** — no build step, no dependencies, no server.

**Features:** two playable characters with distinct stats, five swords designed as sidegrades rather than a linear upgrade path (including a life-stealing blade that also drains you), three sub-weapons, two stages with a unique multi-phase boss each, moving platforms, spike pits, falling chandeliers, stairs, and persistent high scores.

**Technical notes:** hand-written Canvas 2D with no engine. All pixel art is generated procedurally with `fillRect` — there are no image assets. Sprites get an automatic dark outline via an offscreen silhouette pass. The canvas renders at 2× internally for crisp text when scaled down on phones. Touch controls use coordinate hit-testing rather than per-button events so sliding a thumb between buttons works. Jump buffering and coyote time are implemented. Music and SFX are synthesised with WebAudio.

**Controls:** arrows/WASD to move, `X` jump, `Z` attack, `↑`+`Z` sub-weapon, `↑`/`↓` on stairs, `F` fullscreen. On mobile, rotate to landscape.

</details>
