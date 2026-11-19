# Hướng Dẫn Các Lệnh Chạy (Terminal Commands)
<!-- Crafted with love by dinhhpy (https://github.com/dinhhpy) - Christmas 2026 -->

### 1. Cài đặt thư viện
```powershell
python -m pip install -r requirements.txt
```
* **Chức năng:** Cài đặt đầy đủ các thư viện cần thiết (`pygame-ce`, `numpy`, `imageio_ffmpeg`, `opencv-python`).

---

### 2. Chạy giao diện cây thông 3D (Interactive Window)

#### Chạy mặc định (có nhạc nền Synth-pop & hiệu ứng 3D)
```powershell
python christmas_tree.py
```

#### Chạy không bật âm thanh (tắt tiếng)
```powershell
python christmas_tree.py --no-audio
```

#### Chạy với nhạc Giáng sinh truyền thống (thay vì bài Last Christmas)
```powershell
python christmas_tree.py --theme traditional
```

#### Chạy với bài nhạc tùy chọn của bạn
```powershell
python christmas_tree.py --audio "duong_dan_den_file_nhac.mp3" --audio-start 15.0
```
* `--audio`: Đường dẫn đến file nhạc (`.mp3`, `.wav`, `.m4a`,...).
* `--audio-start`: Số giây bắt đầu phát trong bài nhạc.

---

### 3. Phím tắt điều khiển khi đang mở cửa sổ
* **`Space`**: Tạm dừng / Tiếp tục (Pause / Resume cả hình và nhạc).
* **`R`**: Chạy lại hoạt cảnh từ đầu (Restart).
* **`←` / `→`**: Tua lùi 1 giây / Tua tới 1 giây.
* **`S`**: Chụp ảnh màn hình (lưu tự động vào thư mục `output/`).
* **`Esc` hoặc `Q`**: Thoát chương trình.

---

### 4. Xuất video ngắn 9:16 (Export Reel / TikTok / Shorts)

#### Xuất video mặc định (1080×1920, 30fps, dài 20s)
```powershell
python christmas_tree.py --export output/christmas_tree_reel.mp4
```
* **Chức năng:** Nửa trên hiển thị cây thông hoạt họa, nửa dưới cuộn mã nguồn hiệu ứng chạy theo nhịp nhạc.

#### Tùy chỉnh độ phân giải, tốc độ khung hình và thời lượng
```powershell
python christmas_tree.py --export output/video.mp4 --res 720p --fps 30 --duration 15
```
* `--res`: Độ phân giải (`1080p` hoặc `720p`).
* `--fps`: Số khung hình trên giây (mặc định: `30`).
* `--duration`: Thời lượng video tính bằng giây (mặc định: `20`).

#### Tùy chỉnh lời chúc và tên tác giả
```powershell
python christmas_tree.py --export output/video.mp4 --message "M E R R Y   C H R I S T M A S" --author "@your.name"
```
* `--message`: Nội dung dòng chữ chúc mừng cuối video.
* `--author`: Chữ ký / Tên tài khoản hiển thị ở góc dưới bên trái video.
