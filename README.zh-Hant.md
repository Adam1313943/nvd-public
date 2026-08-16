# nvd

> macOS 與 Windows 影片下載工具，內建工具、媒體庫、AI 字幕，開箱即用。

<p align="right">
  <a href="./README.md">English</a> · <strong>繁體中文</strong> · <a href="./README.zh-Hans.md">简体中文</a> · <a href="./README.ja.md">日本語</a>
</p>

<p align="center">
  <a href="https://www.momosoft.one/nvd">官方網站</a> ·
  <a href="https://github.com/Adam1313943/nvd-public/releases/latest">下載最新版</a> ·
  <a href="https://www.momosoft.one/Privacy.html">隱私政策</a>
</p>

---

## 是什麼

**nvd** 是一款 **macOS 與 Windows** 的影片下載工具。把網路上的影片變成本機檔案 — 不用裝 Homebrew、不用裝 yt-dlp、不用敲指令。安裝就能用。

支援 YouTube、Vimeo、Twitch、niconico、Bilibili、Twitter、Facebook、Instagram、TikTok 等 **1,500 + 個影片站**。

## 主要特色

- **🎁 開箱即用** — 內建 yt-dlp / ffmpeg 與串流嗅探器；不需另外安裝瀏覽器或敲指令
- **🎯 智慧偵測串流** — 自動偵測網頁影片串流，連 JavaScript-only 站也找得到 manifest
- **📚 媒體庫** — 把下載的影片整理成來源、合輯、播放清單，附縮圖檢視
- **💬 AI 字幕** — 用本機 whisper 產生字幕，並可翻譯成多國語言
- **▶️ 內建播放器** — 速度、子母畫面、續播，字幕疊層（大小 / 位置 / 拖曳定位）

## 系統需求

- **macOS** 14.0 Sonoma 以上，Apple Silicon (M1 / M2 / M3 / M4)
- **Windows** 10 / 11，64 位元
- 約 300 MB 儲存空間（AI 字幕模型於使用時下載）

## 安裝

- **macOS** — 到 [Releases](https://github.com/Adam1313943/nvd-public/releases/latest) 下載 `nvd-*-mac-arm64.zip`，解壓後把 `nvd.app` 拖進 `/Applications`。
- **Windows** — 到 [Releases](https://github.com/Adam1313943/nvd-public/releases/latest) 下載 `nvd-*-setup.exe`，執行安裝程式。

首次啟動會跳出歡迎導引。第一次開啟時 macOS Gatekeeper / Windows SmartScreen 可能會警告，選「**打開**」/「**仍要執行**」即可。

## 免費版 vs Pro

**免費版**含 **7 天試用**。試用結束後，下載與字幕辨識需要 Pro。

| 功能 | 免費（7 天試用內） | 試用結束後 | Pro |
|---|---|---|---|
| 下載（1,500 + 站） | ✅ | 需 Pro | ✅ 無限 |
| 媒體庫 / 內建播放器 | ✅ | ✅ | ✅ |
| AI 字幕 — 原文辨識 | ✅ | 需 Pro | ✅ 無限 |
| AI 字幕 — 翻譯 | 需 Pro | 需 Pro | ✅ 每月 5 部 |

## 升級 Pro

- **價格**：US$15 一次買斷
- **裝置數**：同一份授權可在最多 3 台裝置啟用（macOS / Windows），可隨時停用釋出名額
- **更新**：含 1 年內所有功能更新，1 年後可選 50% off 續約
- **退款**：7 天內無條件退款

[**到 momosoft.one 購買 Pro**](https://www.momosoft.one/nvd)

購買後 1 分鐘內會收到授權碼。開啟 nvd → 設定 → 授權 → 升級 Pro → 「已有授權碼？點此啟用」填 Email + 授權碼即可。

## 隱私

nvd 主要在你的裝置本機運作。會對外連線的時機：

1. 啟用授權時驗證一次
2. 檢查更新（`version.json`）
3. 匿名使用分析 — 預設開啟，可在「設定」關閉
4. 字幕翻譯 — 僅在你使用時；會把字幕文字傳送到翻譯服務

完整隱私政策：[momosoft.one/Privacy.html](https://www.momosoft.one/Privacy.html)

## 內含的開源元件

nvd 內建以下開源元件：

- [yt-dlp](https://github.com/yt-dlp/yt-dlp) — Unlicense
- [ffmpeg](https://ffmpeg.org/) — LGPL/GPL
- [whisper.cpp](https://github.com/ggml-org/whisper.cpp) — MIT（AI 字幕辨識）
- [Deno](https://deno.com/) — MIT（部分站台的 JS runtime）
- [Electron](https://www.electronjs.org/) / Chromium — MIT / BSD

## 著作權聲明

nvd 是純粹的影片下載工具，跟 yt-dlp、ffmpeg 等開源專案一樣。使用者下載內容前請確認你具有合法權利（自製內容、有授權的內容、合理使用範圍）。

請尊重著作權人權益與各影片站服務條款。nvd 開發團隊不對使用者下載的內容負責。

## 客服與支援

- **客服信箱**：[support@momosoft.one](mailto:support@momosoft.one)
- **問題回報**：[Issues](https://github.com/Adam1313943/nvd-public/issues)
- **更新日誌**：[CHANGELOG.md](./CHANGELOG.md)

---

© 2026 [MomoSoft](https://www.momosoft.one). All rights reserved.
