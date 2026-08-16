# nvd

> macOS 与 Windows 视频下载工具，内置工具、媒体库、AI 字幕，开箱即用。

<p align="right">
  <a href="./README.md">English</a> · <a href="./README.zh-Hant.md">繁體中文</a> · <strong>简体中文</strong> · <a href="./README.ja.md">日本語</a>
</p>

<p align="center">
  <a href="https://www.momosoft.one/nvd">官方网站</a> ·
  <a href="https://github.com/Adam1313943/nvd-public/releases/latest">下载最新版</a> ·
  <a href="https://www.momosoft.one/Privacy.html">隐私政策</a>
</p>

---

## 是什么

**nvd** 是一款 **macOS 与 Windows** 的视频下载工具。把网络上的视频变成本地文件 — 不用装 Homebrew、不用装 yt-dlp、不用敲命令。安装即用。

支持 YouTube、Vimeo、Twitch、niconico、Bilibili、Twitter、Facebook、Instagram、TikTok 等 **1,500 + 个视频站**。

## 主要特色

- **🎁 开箱即用** — 内置 yt-dlp / ffmpeg 与流嗅探器；无需另装浏览器或敲命令
- **🎯 智能检测流** — 自动检测网页视频流，连 JavaScript-only 站也能找到 manifest
- **📚 媒体库** — 把下载的视频整理成来源、合辑、播放列表，附缩略图视图
- **💬 AI 字幕** — 用本地 whisper 生成字幕，并可翻译成多国语言
- **▶️ 内置播放器** — 速度、画中画、续播，字幕叠层（大小 / 位置 / 拖拽定位）

## 系统需求

- **macOS** 14.0 Sonoma 以上，Apple Silicon (M1 / M2 / M3 / M4)
- **Windows** 10 / 11，64 位
- 约 300 MB 存储空间（AI 字幕模型于使用时下载）

## 安装

- **macOS** — 到 [Releases](https://github.com/Adam1313943/nvd-public/releases/latest) 下载 `nvd-*-mac-arm64.zip`，解压后把 `nvd.app` 拖进 `/Applications`。
- **Windows** — 到 [Releases](https://github.com/Adam1313943/nvd-public/releases/latest) 下载 `nvd-*-setup.exe`，运行安装程序。

首次启动会弹出欢迎向导。第一次打开时 macOS Gatekeeper / Windows SmartScreen 可能会警告，选「**打开**」/「**仍要运行**」即可。

## 免费版 vs Pro

**免费版**含 **7 天试用**。试用结束后，下载与字幕识别需要 Pro。

| 功能 | 免费（7 天试用内） | 试用结束后 | Pro |
|---|---|---|---|
| 下载（1,500 + 站） | ✅ | 需 Pro | ✅ 无限 |
| 媒体库 / 内置播放器 | ✅ | ✅ | ✅ |
| AI 字幕 — 原文识别 | ✅ | 需 Pro | ✅ 无限 |
| AI 字幕 — 翻译 | 需 Pro | 需 Pro | ✅ 每月 5 部 |

## 升级 Pro

- **价格**：US$15 一次买断
- **设备数**：同一份授权可在最多 3 台设备启用（macOS / Windows），可随时停用释放名额
- **更新**：含 1 年内所有功能更新，1 年后可选 50% off 续订
- **退款**：7 天内无条件退款

[**到 momosoft.one 购买 Pro**](https://www.momosoft.one/nvd)

购买后 1 分钟内会收到授权码。打开 nvd → 设置 → 授权 → 升级 Pro → 「已有授权码？点此启用」填 Email + 授权码即可。

## 隐私

nvd 主要在你的设备本地运行。会对外连接的时机：

1. 启用授权时验证一次
2. 检查更新（`version.json`）
3. 匿名使用分析 — 默认开启，可在「设置」关闭
4. 字幕翻译 — 仅在你使用时；会把字幕文字发送到翻译服务

完整隐私政策：[momosoft.one/Privacy.html](https://www.momosoft.one/Privacy.html)

## 内含的开源组件

nvd 内置以下开源组件：

- [yt-dlp](https://github.com/yt-dlp/yt-dlp) — Unlicense
- [ffmpeg](https://ffmpeg.org/) — LGPL/GPL
- [whisper.cpp](https://github.com/ggml-org/whisper.cpp) — MIT（AI 字幕识别）
- [Deno](https://deno.com/) — MIT（部分站点的 JS runtime）
- [Electron](https://www.electronjs.org/) / Chromium — MIT / BSD

## 版权声明

nvd 是纯粹的视频下载工具，跟 yt-dlp、ffmpeg 等开源项目一样。用户下载内容前请确认你具有合法权利（自制内容、有授权的内容、合理使用范围）。

请尊重著作权人权益与各视频站服务条款。nvd 开发团队不对用户下载的内容负责。

## 客服与支持

- **客服邮箱**：[support@momosoft.one](mailto:support@momosoft.one)
- **问题反馈**：[Issues](https://github.com/Adam1313943/nvd-public/issues)
- **更新日志**：[CHANGELOG.md](./CHANGELOG.md)

---

© 2026 [MomoSoft](https://www.momosoft.one). All rights reserved.
