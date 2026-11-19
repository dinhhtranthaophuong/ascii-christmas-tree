# 3D ASCII Christmas Tree - Terminal Commands & Usage Guide
<!-- Crafted with love by dinhhpy (https://github.com/dinhhpy) - Christmas 2026 -->

### 1. Installation
```powershell
python -m pip install -r requirements.txt
```
* **Description:** Installs all required dependencies (`pygame-ce`, `numpy`, `imageio_ffmpeg`, `opencv-python`).

---

### 2. Run Interactive 3D ASCII Window

#### Default Run (Built-in 80s Synth-pop & 3D ASCII effects)
```powershell
python christmas_tree.py
```

#### Run in Silent Mode (No Audio)
```powershell
python christmas_tree.py --no-audio
```

#### Run with Traditional Holiday Carol Theme
```powershell
python christmas_tree.py --theme traditional
```

#### Run with Custom Soundtrack / Audio Track
```powershell
python christmas_tree.py --audio "path/to/song.mp3" --audio-start 15.0
```
* `--audio`: Path to custom audio/video file (`.mp3`, `.wav`, `.m4a`, `.mp4`, etc.).
* `--audio-start`: Start offset in seconds.

---

### 3. Keyboard Controls
* **`Space`**: Pause / Resume (audio and visuals).
* **`R`**: Restart animation from the beginning.
* **`←` / `→`**: Scrub -1s / +1s.
* **`S`**: Save screenshot (automatically saved to `output/`).
* **`Esc` or `Q`**: Quit the application.

---

### 4. Export 9:16 Vertical Reel (Instagram Reels / TikTok / Shorts)

#### Default Export (1080×1920 @ 30fps, 20s duration)
```powershell
python christmas_tree.py --export output/christmas_tree_reel.mp4
```
* **Description:** Splits screen into top pane (3D ASCII animation) and bottom pane (synchronized scrolling source code).

#### Custom Resolution, Framerate & Duration
```powershell
python christmas_tree.py --export output/video.mp4 --res 720p --fps 30 --duration 15
```
* `--res`: Output resolution (`1080p` or `720p`).
* `--fps`: Frame rate (default: `30`).
* `--duration`: Video duration in seconds (default: `20`).

#### Custom Holiday Greeting & Author Handle
```powershell
python christmas_tree.py --export output/video.mp4 --message "M E R R Y   C H R I S T M A S" --author "@your.name"
```
* `--message`: Text displayed during the grand finale.
* `--author`: Signature handle shown on the bottom-left corner.
