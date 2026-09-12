# 🎵 All-in-One LRC Maker & Tap Marker

<p align="center">
  <a href="#english"><b>English</b></a> | <a href="#繁體中文"><b>繁體中文</b></a>
</p>

> A lightweight, zero-dependency, browser-based LRC generator and beat-tapping marker tool.  
> 輕量、零依賴、純前端執行的全能型 LRC 歌詞製作與純音樂節奏打點工具。

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Pure HTML5](https://img.shields.io/badge/HTML5-Single_File-orange?logo=html5)](LrcMarkerTool.html)
[![Offline Ready](https://img.shields.io/badge/Offline-100%25-brightgreen)](#)

---

<div id="english"></div>

## English

### ✨ Key Features

- **Dual Work Modes**:
  - 🎵 **Instrumental Tap Mode** — Tailored for instrumentals, soundtracks, and beat tracking. Supports custom prefixes and auto-incrementing numbers (e.g. `Marker 1`, `Section 2`).
  - 📝 **Lyrics Sync Mode** — Paste your lyrics and tap to stamp line by line with clear Previous / Current / Next line visibility.
- **Industry-Standard Undo & Audio Rewind**:
  - Press <kbd>Ctrl</kbd>+<kbd>Z</kbd> or <kbd>Backspace</kbd> to undo.
  - Clears the current line's timestamp and **automatically rewinds audio to the previous line ($N-1$) timestamp**, providing natural reaction runway to re-time the lyric accurately.
- **Synchronized Playback Highlighting**:
  - Live audio playback synchronizes with the list: the active lyric or marker glows in cyan and automatically smooth-scrolls into view.
  - Click any row in the list to jump playback and re-sync from that position.
- **Flexible & Responsive Layout**:
  - Draggable splitter divider to adjust control and preview panel widths.
  - Quick width presets (`440px`, `640px`).
  - Auto word-wrap toggle to prevent long lyrics from being cut off.
- **Fine Timing Nudge**:
  - Each marker or line has `[-0.1s]` and `[+0.1s]` nudge buttons for millisecond precision tuning.
- **Multi-Language Support (i18n)**:
  - English (`en`, default)
  - Traditional Chinese (`zh-TW`)
  - Simplified Chinese (`zh-CN`)
  - Preferences are automatically saved in `localStorage`.
- **Export & Compatibility**:
  - Instant one-click copy to clipboard.
  - One-click `.lrc` file download formatted with standard metadata (`[ti: ...]`, `[ar: ...]`, `[mm:ss.xx]`).
  - Fully compatible with game engines (Unity, Unreal), media players, and mobile music apps.
- **Zero Dependencies**:
  - Single standalone HTML file, runs completely client-side in any modern browser without network access or installation.

### ⌨️ Keyboard Shortcuts

| Shortcut | Action |
| :--- | :--- |
| <kbd>Space</kbd> / <kbd>Enter</kbd> | Instrumental Mode: Drop Marker<br>Lyrics Mode: Stamp current line & advance |
| <kbd>Ctrl</kbd> + <kbd>Z</kbd> / <kbd>Backspace</kbd> | Undo previous line & **rewind audio to previous timestamp** |
| <kbd>P</kbd> | Play / Pause audio |
| <kbd>←</kbd> / <kbd>J</kbd> | Rewind audio 2 seconds |
| <kbd>→</kbd> / <kbd>L</kbd> | Fast-forward audio 2 seconds |

*(Shortcuts are automatically bypassed when typing in text fields).*

### 🚀 Getting Started

1. Open `LrcMarkerTool.html` in any modern web browser.
2. Drag & drop an audio file (`.mp3`, `.wav`, `.ogg`, `.flac`, `.m4a`).
3. Choose **Instrumental Mode** or **Lyrics Sync Mode**.
4. Play the audio and press <kbd>Space</kbd> on the beat.
5. Review the live preview on the right and click **Download .LRC File**!

---

<div id="繁體中文"></div>

## 繁體中文

### ✨ 核心功能

- **雙模式自由切換 (Dual Modes)**：
  - 🎵 **純音樂打點 (Instrumental Tap)**：專為純音樂、遊戲配樂、打擊點設計，支援自訂標籤前綴與自動編號（如 `Marker 1`、`Section 2`）。
  - 📝 **歌詞逐句同步 (Lyrics Sync)**：貼上純文字歌詞，逐句跟隨音樂敲擊空白鍵打點，即時提供「上一句 / 當前句 / 下一句」清晰視野導引。
- **對齊業界標準的 Undo 音樂回溯 (Undo & Rewind)**：
  - 支援 <kbd>Ctrl</kbd>+<kbd>Z</kbd> 或 <kbd>Backspace</kbd> 復原。
  - 復原時不僅清除當前句的時間戳，**音樂會自動倒帶回前一句（$N-1$ 行）的時間戳**，為當前句留出充足的聽音與反應裕度。
- **打點清單播放同步 (Playback Synchronization)**：
  - 播放時，當前發聲的句子/時間點會呈現青色光暈高亮，並自動平滑滾動至可見區域。
  - 點擊清單中任一行可直接跳轉音樂播放，並從該行重新開始同步。
- **長歌詞與彈性版面**：
  - 中間分隔線支援滑鼠拖曳調整預覽區寬度，並提供 `440px` 與 `640px` 快速按鈕。
  - 預設開啟自動折行（Wrap Lines），避免長歌詞橫向截斷；亦可切換為橫向滾動模式。
- **毫秒微調 (Fine Nudge)**：
  - 每個時間點皆配有 `[-0.1s]` 與 `[+0.1s]` 微調按鈕，方便微調時間偏差。
- **多語系介面 (i18n)**：
  - 英文（English，預設）
  - 繁體中文（繁體中文）
  - 簡體中文（简体中文）
  - 偏好自動持久化於 `localStorage`。
- **匯出支援**：
  - 一鍵複製內容至剪貼簿。
  - 一鍵下載標準 `.lrc` 檔案（自動包含 `[ti: ...]`、`[ar: ...]` 等元資料標籤）。
- **零依賴與離線可用**：
  - 單一 HTML 檔，無需伺服器、無需 Node.js、無需安裝，雙擊即可在任何瀏覽器離線運行。

### ⌨️ 快捷鍵表

| 快捷鍵 | 功能說明 |
| :--- | :--- |
| <kbd>Space</kbd> 或 <kbd>Enter</kbd> | 純音樂模式：記錄時間點<br>歌詞模式：為當前句打點並跳至下一行 |
| <kbd>Ctrl</kbd> + <kbd>Z</kbd> 或 <kbd>Backspace</kbd> | 復原上一句，並**將音樂倒帶至上一句時間點** |
| <kbd>P</kbd> | 播放 / 暫停音樂 |
| <kbd>←</kbd> 或 <kbd>J</kbd> | 快退 2 秒 |
| <kbd>→</kbd> 或 <kbd>L</kbd> | 快進 2 秒 |

*(在文字輸入框中打字時會自動停用全域快捷鍵)*

### 🚀 使用指南

1. 直接以瀏覽器開啟 `LrcMarkerTool.html`。
2. 點擊或拖曳音訊檔至視窗中（支援 `.mp3`、`.wav`、`.ogg`、`.flac`、`.m4a`）。
3. 選擇「純音樂打點模式」或「歌詞同步模式」。
4. 播放音樂，跟隨節奏按 <kbd>Space</kbd> 打點。
5. 右側預覽無誤後，點擊 **「下載 .LRC 檔」** 即可。

---

## 📄 授權 / License

Distributed under the [MIT License](LICENSE).
