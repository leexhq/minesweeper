# 精致扫雷 | Minesweeper Modern & Classic

<p align="center">
  <img src="https://img.shields.io/badge/License-MIT-blue.svg" alt="License: MIT">
  <img src="https://img.shields.io/badge/HTML5-Pure_Frontend-orange.svg" alt="Pure Frontend">
  <img src="https://img.shields.io/badge/Dependencies-Zero-green.svg" alt="Zero Dependencies">
  <img src="https://img.shields.io/badge/Audio-Web_Audio_API-purple.svg" alt="Web Audio API">
</p>

<p align="center">
  一个优雅、精致、高颜值且遵循经典扫雷规则的现代网页版扫雷游戏。<br>
  零外部依赖，单文件极速加载，原生支持 4 套视觉主题，适配电脑与移动端触摸操作。
</p>

<p align="center">
  <strong><a href="#简体中文">简体中文</a></strong> | <strong><a href="#english">English</a></strong>
</p>

---

## 简体中文

### 🌟 核心亮点

- **首击大片空白保底 (Opening Guarantee)**：
  - 彻底告别“首击只开出一个孤零零空白”的糟糕体验！
  - 参考成熟官方方案，第一击保证绝对安全，并智能划定连续的安全中心，点击必定连带翻开一大片开阔的空白与边缘数字。
- **全域连锁波纹扩散 (Flood Fill Cascade)**：
  - 递归扩散遇空白自动向周围 8 个方向展开，辅以顺滑的中心向外波纹微动效（Ripple Animation），爽快感拉满。
- **4 套高颜值主题即时切换**：
  - ✨ **现代雅致 (Modern Slate)**：深蓝渐变卡片、微凹质感、立体微浮雕键位与鲜艳的高对比度数字。
  - 🕹️ **经典复古 (Retro Win98)**：$1:1$ 还原 Windows 95/98 经典银灰浮雕框、红色 7 段 LED 数显与经典笑脸。
  - 🍃 **清新明亮 (Clean Light)**：简约淡雅白灰卡片质感，适合日间游玩。
  - 🌌 **深邃霓虹 (Cyber Neon)**：OLED 纯黑暗夜搭配青粉荧光线条。
- **纯 Web Audio 动态合成音效**：
  - 无需下载或请求任何外部 MP3/WAV 音频文件。翻开短促敲击音（音调随扩散深度提升）、插旗声、踩雷低频震颤与通关琶音全由浏览器原生合成，零加载延迟。
- **智能快速连开 (Chord / 双击展开)**：
  - 当数字周围已标旗数量达到该数字时，双击数字或直接单点该数字即可瞬间安全展开周围未标记格子。
- **移动端深度适配**：
  - 支持触摸长按插旗（附带设备震动触觉反馈）、右上角专属“插旗模式”切换开关。
- **战绩系统与通关彩蛋**：
  - 自动记录初级、中级、高级的历史最佳秒数（保存于本地 `localStorage`）。
  - 通关胜利时触发全屏 Canvas 独立轻量彩带撒花与战绩面板。

---

### 🎮 游戏规则与操作

| 操作 | 电脑端 | 手机 / 平板端 |
| :--- | :--- | :--- |
| **翻开格子** | 鼠标左键点击 | 点击格子 |
| **标记旗帜 🚩 / 问号 ❓** | 鼠标右键点击 | 长按格子（触发震动）或开启【🚩 插旗模式】点击 |
| **快速展开周边 (Chord)** | 双击已翻开数字 / 单点已满足条件的数字 | 双击数字 |
| **重新开始** | 点击顶部笑脸表情 😊 或按快捷键 `R` | 点击顶部笑脸表情 😊 |

#### 常用快捷键
- `R`：重新开局
- `F` 或 `空格`：切换插旗模式
- `1` / `2` / `3`：快速选择 初级 (9×9) / 中级 (16×16) / 高级 (30×16)
- `Esc`：关闭弹窗

---

### 🚀 快速运行与在线部署

#### 本地游玩
本项目仅包含原生 HTML/CSS/JavaScript，**无需任何构建环境与依赖**：
1. 下载或克隆本仓库到本地。
2. 双击打开 `index.html`，即可在任意现代浏览器（Edge、Chrome、Safari、Firefox）离线流畅游玩。

#### 开启 GitHub Pages 在线体验
1. 在仓库的 **Settings** -> **Pages** 中。
2. **Branch** 选择 `main` 分支，路径选择 `/ (root)`。
3. 点击 **Save**，即可获得专属在线网页链接！

---

## English

### 🌟 Key Features

- **Guaranteed Large Opening**:
  - Eliminates frustrating single-tile openings! The initial click guarantees a generous open lake of zeros surrounded by numbered boundary cells, perfectly mirroring modern competitive and casual Minesweeper designs.
- **Recursive Flood Fill with Ripple Cascade**:
  - Empty zero-cells smoothly fan out in all 8 directions with an eye-pleasing radial delay, creating a satisfying water-ripple unveiling effect.
- **4 Beautiful Visual Themes**:
  - ✨ **Modern Slate** (Default): Glassmorphism card, recessed cells, soft 3D buttons, and vivid contrasting number typography.
  - 🕹️ **Retro Win98**: Authentic Windows 95/98 silver-gray beveled borders, classic red 7-segment LED counters, and iconic smiley face.
  - 🍃 **Clean Light**: Minimalist paper-white theme, soft drop shadows, easy on the eyes.
  - 🌌 **Cyber Neon**: Deep OLED pitch-black with vibrant cyberpunk neon accents.
- **Zero-Latency Web Audio Synthesizer**:
  - Procedural sound effects generated entirely via the Web Audio API without any external audio asset downloads (rising cascade tones, flag placement, explosion rumble, and victorious victory fanfare).
- **Smart Chord / Fast Clear**:
  - When the flags surrounding a number match its value, double-clicking (or single-clicking) reveals all adjacent unflagged cells immediately.
- **Mobile & Touch Optimized**:
  - Long-press to flag with haptic vibration (`navigator.vibrate`), plus a floating "Flag Mode" button for effortless single-hand touch play.
- **Local Records & Celebration**:
  - Persists personal best times for each difficulty level via `localStorage`. Fullscreen Canvas confetti bursts upon victory!

---

### 🎮 Controls & Shortcuts

| Action | Desktop | Mobile / Touch |
| :--- | :--- | :--- |
| **Reveal Cell** | Left click | Tap |
| **Flag 🚩 / Question ❓** | Right click | Long press (with vibration) or enable "Flag Mode" |
| **Chord (Quick Clear)** | Double click number | Double tap number |
| **Restart** | Click smiley face 😊 or press `R` | Tap smiley face 😊 |

#### Keyboard Shortcuts
- `R`: Restart game
- `F` or `Space`: Toggle flag mode
- `1` / `2` / `3`: Switch between Easy / Medium / Hard
- `Esc`: Close open modal dialogues

---

### 🚀 Usage & Deployment

#### Run Locally
No build tools, npm, or servers required:
1. Clone or download this repository.
2. Double-click `index.html` to play instantly in any modern web browser.

#### Deploy with GitHub Pages
1. Go to repository **Settings** -> **Pages**.
2. Set **Branch** to `main` and folder to `/ (root)`.
3. Click **Save** to publish your live online Minesweeper game.

---

### 📄 License

This project is licensed under the [MIT License](LICENSE) - feel free to use, modify, and distribute!
