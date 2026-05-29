# nvd

> macOS 影片下載工具,內建工具、開箱即用。

<p align="right">
  <a href="./README.md">English</a> · <strong>繁體中文</strong> · <a href="./README.zh-Hans.md">简体中文</a> · <a href="./README.ja.md">日本語</a>
</p>

<p align="center">
  <img src="docs/screenshots/hero.png" alt="nvd hero" width="720">
</p>

<p align="center">
  <a href="https://www.momosoft.one/nvd">官方網站</a> ·
  <a href="https://github.com/Adam1313943/nvd-public/releases/latest">下載最新版</a> ·
  <a href="https://www.momosoft.one/Privacy.html">隱私政策</a>
</p>

---

## 是什麼

**nvd** 是一款 macOS 原生的影片下載工具。把網路上的影片變成本機檔案 — 不用裝 Homebrew、不用裝 yt-dlp、不用敲指令。雙擊安裝就能用。

支援 YouTube、Vimeo、Twitch、niconico、Bilibili、Twitter、Facebook、Instagram、TikTok 等 **1,500 + 個影片站**。

## 三個賣點

- **🎁 開箱即用** — 內建 yt-dlp / ffmpeg,不用裝 Homebrew 或敲指令
- **🎯 智慧偵測串流** — 自動偵測網頁影片串流,連 JavaScript-only 站也找得到 manifest
- **🔄 穩定的長片下載** — 處理多種 HLS 變體與會話過期,長影片下載中途不中斷

## 系統需求

- macOS 14.0 Sonoma 以上
- Apple Silicon (M1 / M2 / M3 / M4)
- 約 250 MB 儲存空間
- **智慧偵測功能需要**:Chrome / Brave / Edge / Arc / Vivaldi 任一個(多數 Mac 已安裝)。基本 yt-dlp 支援的站不需要

## 安裝

1. 到 [Releases](https://github.com/Adam1313943/nvd-public/releases/latest) 下載最新版 `nvd-*.zip`
2. 解壓後把 `nvd.app` 拖進 `/Applications`
3. 雙擊開啟 — 首次啟動會跳出歡迎導引

第一次啟動 macOS Gatekeeper 可能會提示「來自網路下載」確認,點「打開」即可。

## 免費版 vs Pro

| 功能 | 免費版 | Pro |
|---|---|---|
| 支援 1,500 + 個影片站 | ✅ | ✅ |
| 解析度 / 字幕 / metadata / 縮圖內嵌 | ✅ | ✅ |
| 智慧偵測串流 | ✅ | ✅ |
| 瀏覽器 Cookies 整合 | ✅ | ✅ |
| Menu Bar 提示 / 通知 | ✅ | ✅ |
| 自動更新 | ✅ | ✅ |
| 影片長度上限 | **10 分鐘** | 無限制 |
| 單次下載大小 | **100 MB** | 無限制 |
| 截取片段下載 | — | ✅ |
| 內嵌影片預覽播放 | — | ✅ |

## 升級 Pro

- **價格**:NT$ 380 一次買斷(約 USD $12)
- **裝置數**:同一份授權可在最多 3 台 Mac 啟用(可隨時在裝置上停用釋出名額)
- **更新**:含 1 年內所有功能更新,1 年後可選 50% off 續約
- **退款**:7 天內無條件退款

[**到 momosoft.one 購買 Pro**](https://www.momosoft.one/nvd)

購買後 1 分鐘內會收到授權碼。開啟 nvd → 設定 → 授權 → 升級 Pro → 「已有授權碼?點此啟用」填 Email + 授權碼即可。

## 隱私

nvd 完全本地運作,**沒有任何 telemetry / analytics**。唯一會連回伺服器的時機是:
1. 啟用 Pro 授權時驗證一次
2. Sparkle 檢查更新時拉取 appcast

完整隱私政策:[momosoft.one/Privacy.html](https://www.momosoft.one/Privacy.html)

## 內含的開源元件

nvd 內建以下開源元件供下載引擎使用:

- [yt-dlp](https://github.com/yt-dlp/yt-dlp) — Unlicense
- [ffmpeg](https://ffmpeg.org/) — LGPL/GPL
- [Sparkle](https://sparkle-project.org/) — MIT

## 著作權聲明

nvd 是純粹的影片下載工具,跟 yt-dlp、ffmpeg 等開源專案一樣。使用者下載內容前請確認你具有合法權利(自製內容、有授權的內容、合理使用範圍)。

請尊重著作權人權益與各影片站服務條款。nvd 開發團隊不對使用者下載的內容負責。

## 客服與支援

- **客服信箱**:[support@momosoft.one](mailto:support@momosoft.one)
- **問題回報**:[Issues](https://github.com/Adam1313943/nvd-public/issues)
- **更新日誌**:[CHANGELOG.md](./CHANGELOG.md)

---

© 2026 [MomoSoft](https://www.momosoft.one). All rights reserved.
