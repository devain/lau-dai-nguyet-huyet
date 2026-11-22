# 🏰 Lâu Đài Nguyệt Huyết

Game hành động platformer kiểu Castlevania, chạy hoàn toàn trong trình duyệt. **Một file HTML duy nhất** — không build, không dependency, không server, không có file ảnh hay âm thanh nào.

▶️ **[Chơi ngay](https://devain.github.io/lau-dai-nguyet-huyet/)**

Bảy màn, bảy boss, hai nhân vật với cách chơi riêng, 20 vũ khí rơi ra theo độ hiếm để farm, hệ thống cấp độ – trang bị – tạo hình, và lưu tiến độ riêng cho từng nhân vật.

---

## Điều khiển

| Bàn phím | Cảm ứng | Hành động |
|---|---|---|
| `←` `→` hoặc `A` `D` | ◀ ▶ | Di chuyển |
| `X` / `K` / `Space` | NHẢY | Nhảy |
| `Z` / `J` | KIẾM | Vung kiếm |
| `↓` + `Z` | ▼ + KIẾM | **Kiên**: Xung kích · **Nguyệt**: ngồi chém thấp |
| `↑` `↓` | ▲ ▼ | Lên xuống cầu thang |
| `↑` + `Z` | ▲ + KIẾM | Ném phụ khí (tốn 1 tim) |
| `C` / `Q` | nút đổi kiếm | Đổi vũ khí đang cầm |
| `V` | Menu → Lưu game | Lưu tiến độ |
| `G` | nút ⚙ | Trang bị & tạo hình |
| `T` | nút ⚔ BÃI TẬP | Vào bãi tập (từ màn chính) |
| `1` – `7` | — | Nhảy thẳng tới màn bất kỳ (phím thử nghiệm, bỏ qua tiến độ mở màn) |
| `R` | Menu → Chơi lại màn | Chơi lại màn hiện tại |
| `L` | Menu → Độ sáng | Đổi độ sáng (Sáng / Vừa / Tối) |
| `B` | Menu → Cỡ nút bấm | Đổi cỡ nút cảm ứng |
| `F` | ⛶ | Toàn màn hình |
| `Esc` / `P` | ☰ | Tạm dừng, mở menu |

> 📱 **Trên điện thoại nên xoay ngang** — khung game lớn hơn khoảng 1,8 lần, nút bấm dạt về hai góc dưới. Trượt ngón tay giữa các nút vẫn đổi hướng được.

---

## Hai nhân vật

| | Máu | Tốc chạy | Lực nhảy | Điểm mạnh |
|---|---|---|---|---|
| **Kiên** — thợ săn làng Đoài | 16 | 1.45 | 6.6 | **Xung kích**, bền bỉ |
| **Nguyệt** — người trở về, tóc bạc | 13 | 1.78 | 7.1 | Nhanh, nhảy cao, vung kiếm lẹ |

- **Xung kích của Kiên** (`↓` + `Z`): lao ngắn về phía trước, **bất tử trong lúc lao**, xuyên qua địch và gây 3 sát thương mỗi con, làm đổ nến trên đường. Dùng được một lần khi đang trên không, hồi chiêu khoảng 0,7 giây. Nhờ chiêu này Kiên vượt được hố rộng 6 ô (nhảy thường chỉ 3 ô).
- **Nguyệt** không có chiêu lao nhưng chạy nhanh hơn, nhảy cao hơn (qua được hố 4 ô bằng nhảy thường) và vung kiếm nhanh hơn. Đổi lại máu thấp hơn.

Cả hai có **chân dung bán thân** ở màn chọn nhân vật và trong các đoạn truyện. Chân dung và sprite đổi theo bộ tạo hình đang mặc. Vũ khí đang mang được vẽ trên người: giáo, búa, liềm vác sau lưng; song đao bắt chéo bên hông; roi xích cuộn ở hông; thần khí có bao kiếm phát sáng theo màu riêng.

**Cốt truyện kể từ hai góc nhìn.** Kiên đi tìm đứa em gái mất tích mười ba năm trước trong một đêm trăng máu. Nguyệt tỉnh dậy bên bìa rừng với mái tóc bạc trắng và không nhớ mình là ai. Mỗi nhân vật có đoạn mở đầu, lời dẫn từng màn và phần kết riêng.

---

## Bảy màn

| Màn | Bối cảnh | Boss | Máu boss |
|---|---|---|---|
| 1 | **Tiền đình** — sân lâu đài ngoài trời, hành lang mái vòm, nghĩa địa | Tử Thần | 28 |
| 2 | **Hầm mộ** — ván gỗ treo xích trên hố gai, đèn chùm rơi | Bá Tước | 34 |
| 3 | **Tháp đồng hồ** — bánh răng khổng lồ, sàn gỗ, hành lang gai | Quỷ Vương | 44 |
| 4 | **Mái tháp** — ngoài trời, mưa, **gió thổi từng cơn** đẩy lệch cú nhảy, tượng đá thức giấc | Bóng Nguyệt Huyết | 52 |
| 5 | **Điện Nguyệt Huyết** — đại điện kính màu, **sàn đá sụp** sau khi đứng lên | Chúa Tể Nguyệt Huyết | 64 |
| 6 | **Vực Nguyệt** — lâu đài đang chìm, **bể nước** làm chậm bước và hạ lực nhảy, người cá | Mẹ Vực | 74 |
| 7 | **Tâm Nguyệt** — hư không trong lòng trăng, **bục nhấp nháy hai pha**, vực hư không | Nguyệt Huyết | 88 |

Mỗi boss có lối đánh riêng và thay đổi khi xuống dưới nửa máu. Vài ví dụ:

- **Quỷ Vương** giậm đất tạo sóng chấn chạy dọc sàn (phải nhảy) và gọi cột lửa từ trần (phải chạy).
- **Bóng Nguyệt Huyết** triệu bóng nhân bản **mang đúng hình dạng nhân vật bạn đang chơi**.
- **Chúa Tể** dựng tường cầu máu có một khe để lách qua.
- **Mẹ Vực** lặn xuống là bất khả xâm phạm rồi trồi lên chỗ khác.
- **Nguyệt Huyết** là vầng trăng khổng lồ có mặt người, với vành cầu máu, tia laser và mưa thiên thạch.

Trước mỗi trận có thẻ giới thiệu boss, kèm chân dung và lời thách thức.

---

## Vũ khí

### Mười vũ khí thường — tám kiểu đánh

| Vũ khí | Độ hiếm | Tầm | Sát thương | Sát thương/giây | Đặc điểm |
|---|---|---|---|---|---|
| Đoản kiếm | Thường | 30 | 2 | 6.7 | Chém ngang, gọn |
| Trường kiếm | Thường | 42 | 3 | 10.0 | Chém ngang, tầm vừa |
| Song đao | Thường | 26 | 2 | 13.3 | Liên hoàn 3 đòn, đòn thứ 3 gấp đôi |
| Đại kiếm | Hiếm | 54 | 4 | 13.3 | Chém ngang, tầm xa |
| Giáo | Hiếm | 66 | 3 | 11.3 | Đâm thẳng rất xa, xuyên cả hàng |
| Roi xích | Hiếm | 72 | 2 | 6.0 | Với xa nhất, đầu roi +2 sát thương |
| Katana | Sử thi | 46 | 3 | 16.4 | Rút kiếm cực nhanh |
| Búa chiến | Sử thi | 36 | 6 | 12.9 | Chậm, nện đất tạo sóng chấn |
| Liềm hái | Sử thi | 46 | 4 | 12.0 | Vòng cung lớn, trúng cả phía trên |
| Huyết kiếm | Huyền thoại | 40 | 3 | 12.9 | Trúng thì hút 1 máu, nhưng cầm thì tự rút máu dần |

### Mười thần khí

Tên mượn từ truyền thuyết, hình dáng và hiệu ứng thiết kế riêng. Thần khí có viền cầu vồng khi rơi ra.

| Thần khí | Sát thương/giây | Hiệu ứng |
|---|---|---|
| Excalibur | 18.8 | Mỗi nhát phóng kiếm quang xuyên thấu |
| Ragnarök | 16.7 | Sét giáng xuống kẻ trúng đòn, lan sang kẻ đứng gần |
| Apocalypse | 18.0 | Kẻ gục ngã nổ tung, thiêu kẻ xung quanh |
| Soul Breaker | 16.0 | Mỗi mạng hạ được +1 sát thương, tối đa +6 |
| Muramasa | 20.0 | Cực nhanh, 25% chí mạng ×2,5 |
| Durandal | 21.2 | Chém trả đạn địch bay ngược lại |
| Gram | 16.7 | Diệt long: gấp đôi sát thương lên boss |
| Kusanagi | 13.3 | Lưỡi gió với rất xa, thổi bay địch |
| Lævateinn | 16.0 | Thiêu đốt kẻ trúng đòn trong 3 giây |
| Thuận Thiên | 22.5 | Gươm của Lê Lợi — Kim Quy hộ thể: 25% chặn trọn một đòn |

### Rơi đồ và kho vũ khí

- **Quái rơi vũ khí theo độ hiếm**, càng về sau tỉ lệ đồ hiếm càng cao. Thần khí chỉ bắt đầu rơi từ khoảng màn 3. Boss màn 4–7 có 3% → 8% → 12% → 25% ra thần khí.
- **Bảo hiểm xui**: mỗi lần hạ quái mà không ra đồ, tỉ lệ cộng thêm 1,5%; hạ 18 con liên tiếp trắng tay thì con tiếp theo chắc chắn rơi.
- Đồ rơi **lơ lửng và tự bay về phía nhân vật** khi lại gần, không bao giờ rơi xuống hố mất.
- **Kho vũ khí lưu vĩnh viễn**, dùng chung cho cả hai nhân vật. Nhặt trùng món đã có thì món đó **lên bậc** (tối đa +5, mỗi 2 bậc +1 sát thương); đủ bậc rồi thì đổi thành 10 tim.
- **Chỉ tự cầm món mới khi nó tốt hơn món đang cầm** (xét độ hiếm trước, rồi tới sát thương). Món kém hơn được cất vào túi, bấm `C` để đổi.
- **Vũ khí mang theo** chọn trong Kho vũ khí. Đã chọn thì game luôn tôn trọng, kể cả khi vào thẳng màn sau.

### Phụ khí

Dao (bay nhanh, thẳng), rìu (bay vòng cung, xuyên nhiều địch), nước thánh (cháy lan trên sàn). Mỗi lần ném tốn 1 tim; tim nhặt từ nến và quái.

---

## Tiến trình

**Cấp độ** (tối đa 20): hạ quái, đập nến, phá boss để lấy kinh nghiệm. Lên cấp mở khoá trang bị và tạo hình. Cấp và kho vũ khí dùng chung cho cả hai nhân vật.

**Trang bị** — ba ô, mở dần theo cấp:

| Ô | Cấp 1 | Mở thêm |
|---|---|---|
| Giáp | Áo vải | Giáp da (cấp 3, giảm 1 sát thương) · Giáp xích (cấp 7, giảm 2) · Giáp bạc (cấp 12, giảm 2 và +2 máu) |
| Giày | Giày thường | Ủng nhẹ (cấp 4, +8% tốc chạy) · Ủng lò xo (cấp 9, +0,5 nhảy) · Ủng gió (cấp 15, +8% tốc và +0,35 nhảy) |
| Bùa | Không đeo | Bùa tim (cấp 5, tim gấp đôi) · Bùa hồi (cấp 10, hồi 1 máu mỗi 12 giây) · Bùa nguyệt (cấp 16, +1 sát thương kiếm) |

**Tạo hình** — mỗi nhân vật bốn bộ, mở ở cấp 1 / 5 / 11 / 18:
- Kiên: Mặc định · Thợ săn đêm · Hiệp sĩ bạc · Huyết chiến
- Nguyệt: Mặc định · Nguyệt bạch · Ám nguyệt · Hoả nguyệt

**Bãi tập** — mở tạm cả 20 vũ khí để thử. Có hàng bia gỗ để thử tầm và xuyên, bia trên cao, người rơm 3 máu tự hồi sinh để thử hiệu ứng khi hạ gục, và bia bắn cầu lửa để thử Durandal hay Thuận Thiên. **Trên đầu mỗi bia hiện sát thương/giây** trong 3 giây gần nhất. Không chết được, đồng hồ đứng yên, và **không ảnh hưởng gì tới tiến độ thật**.

---

## Lưu game

- **Mỗi nhân vật có ô lưu riêng.** Chơi Kiên không đè lên tiến độ của Nguyệt và ngược lại; hết mạng chỉ xoá ô của nhân vật đó.
- **Tự lưu** ở mỗi điểm hồi sinh và khi sang màn. Lưu tay bằng phím `V` hoặc Menu → Lưu game.
- Màn chính hiện nhãn **▣ LƯU · MÀN N** trên nhân vật có bản lưu, chọn **▸ TIẾP TỤC** để vào lại đúng chỗ.
- Cài đặt (độ sáng, cỡ nút, bật/tắt số sát thương), các màn đã mở và **top 5 điểm cao** cũng được lưu.

---

## Ghi chú kỹ thuật

Viết tay bằng Canvas 2D thuần, không engine, không thư viện.

- **Toàn bộ hình ảnh sinh bằng code** — nhân vật, quái, boss, nền từng màn đều vẽ bằng `fillRect` và path với bảng màu cố định. Mỗi sprite có viền tối tự động: render vào canvas phụ, lấy silhouette tô tối rồi dập 4 hướng.
- **Chân dung** vẽ bằng đường cong spline, chuyển sắc và ánh sáng viền ở độ phân giải gấp đôi, rồi thu nhỏ một lần và lưu vào bộ đệm theo bộ tạo hình.
- **Supersampling 2×** — canvas nội bộ 1024×576, `setTransform(2,2)` nên code vẽ dùng toạ độ 512×288. Chữ sắc nét kể cả khi thu nhỏ trên điện thoại.
- **Kiến trúc tự sinh theo bản đồ**: cột và vòm đỡ dưới mọi tầng đá dày 2 ô, chia đều theo chiều dài; xích treo cho bục lơ lửng ở màn trong nhà; ray trần cho bục di chuyển; cầu thang vẽ thành khối xây liền.
- **Kiểm tra màn chơi tự động mỗi lần dựng màn**:
  - Cầu thang tự căn khớp mép tầng (bậc không đè gạch, đỉnh có sàn, chân có đất).
  - Tìm đường theo tầm nhảy thật của nhân vật để chắc mọi khu đều tới được.
  - Kiểm tra điểm hồi sinh không đặt trên gai hay hố, quái không kẹt trong tường.
  - Nến phải đứng trên sàn, không nằm dưới nước, không đứng sát nhau.
  - Ánh sáng đặt theo kiến trúc: đèn lồng dưới vòm, trụ đèn ở chân cầu thang và đấu trường.
- **Ánh sáng động** bằng lớp tối có khoét lỗ sáng quanh nhân vật, nến, đèn, kèm ba mức độ sáng.
- **Điều khiển có bộ đệm nhảy và coyote time**, lái nhẹ trên không. Cảm ứng hit-test theo toạ độ thay vì gắn event lên từng nút, để trượt ngón giữa các nút vẫn đổi hướng được.
- **Âm thanh**: 7 bản nhạc chip (màn chính, lâu đài, tháp, đại điện, vực, boss, trận cuối) và mọi hiệu ứng âm thanh đều tổng hợp bằng WebAudio.
- **Lưu trữ** qua `window.storage` với các khoá `nguyethuyet:prof:v1` (hồ sơ), `nguyethuyet:run:v1` (lượt chơi), `nguyethuyet:opt:v1` (cài đặt), `nguyethuyet:scores:v2` (điểm cao). Game vẫn chạy bình thường khi không có bộ lưu.

---

## Chạy tại máy

Chỉ cần mở `index.html` bằng trình duyệt, không cần server.

Nếu muốn chạy qua HTTP:

```bash
python3 -m http.server 8000
# rồi mở http://localhost:8000
```

**Đưa lên GitHub Pages:** đẩy `index.html` lên repo, vào *Settings → Pages*, chọn nhánh `main` và thư mục gốc. Vài phút sau game chạy ở `https://devain.github.io/lau-dai-nguyet-huyet/`.

---

## Giấy phép

MIT — xem file [LICENSE](LICENSE). Dùng, sửa, chia sẻ thoải mái.

---

<details>
<summary><b>English summary</b></summary>

A Castlevania-style action platformer that runs entirely in the browser from a **single HTML file** — no build step, no dependencies, no server, and no image or audio assets.

**Content:** seven stages, each with a unique multi-phase boss and its own hand-drawn background. Two playable characters with different mechanics: Kiên has an invulnerable dash attack, Nguyệt is faster with a higher jump. Both get bust portraits in story scenes, and each has a separate first-person storyline with its own ending.

**Loot and progression:** 20 weapons across eight attack styles — including ten "mythic" weapons with special effects such as piercing beams, chain lightning, death explosions, projectile reflection and boss-slaying damage. Weapons drop by rarity with a bad-luck protection system. A persistent armory upgrades duplicates, and better pickups are equipped automatically while weaker ones go to your bag. Levels up to 20 unlock armor, boots, charms and four costumes per character. A training ground lets you test every weapon against dummies with a live DPS readout.

**Saves:** per-character save slots with autosave at checkpoints, plus persistent settings and a top-5 high score table.

**Technical notes:** hand-written Canvas 2D with no engine. All art is generated procedurally; sprites get an automatic dark outline via an offscreen silhouette pass, and portraits are drawn with splines at 2× and downsampled. Each stage is validated whenever it is built: stairs snap to ledges, a reachability search uses the characters' real jump arcs, candles and checkpoints are checked for valid footing, and lighting and supporting architecture (pillars, arches, hanging chains) are placed from the level geometry. Music and SFX are synthesised with WebAudio.

**Controls:** arrows/WASD to move, `X` jump, `Z` attack, `↓`+`Z` dash (Kiên) or low slash (Nguyệt), `↑`+`Z` sub-weapon, `C` switch weapon, `V` save, `G` equipment, `T` training ground, `F` fullscreen. On mobile, rotate to landscape.

</details>
