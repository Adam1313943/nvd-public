# nvd

> macOS 视频下载工具,内置全套工具、开箱即用。

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

**nvd** 是一款 macOS 原生的视频下载工具。把网络上的视频变成本地文件 — 不用装 Homebrew、不用装 yt-dlp、不用敲指令。双击安装就能用。

支持 YouTube、Vimeo、Twitch、niconico、Bilibili、Twitter、Facebook、Instagram、TikTok 等 **1,500 + 个视频站**。

## 三个卖点

- **🎁 开箱即用** — 内置 yt-dlp / ffmpeg,不用装 Homebrew 或敲指令
- **🎯 智能检测流媒体** — 自动检测网页视频流,连 JavaScript-only 站也能找到 manifest
- **🔄 稳定的长视频下载** — 处理多种 HLS 变体与会话过期,长视频下载中途不中断

## 系统要求

- macOS 14.0 Sonoma 以上
- Apple Silicon (M1 / M2 / M3 / M4)
- 约 250 MB 存储空间
- **智能检测功能需要**:Chrome / Brave / Edge / Arc / Vivaldi 任一个(多数 Mac 已安装)。基本 yt-dlp 支持的站不需要

## 安装

1. 到 [Releases](https://github.com/Adam1313943/nvd-public/releases/latest) 下载最新版 `nvd-*.zip`
2. 解压后把 `nvd.app` 拖进 `/Applications`
3. 双击打开 — 首次启动会跳出欢迎引导

第一次启动 macOS Gatekeeper 可能会提示「来自网络下载」确认,点「打开」即可。

## 免费版 vs Pro

| 功能 | 免费版 | Pro |
|---|---|---|
| 支持 1,500 + 个视频站 | ✅ | ✅ |
| 分辨率 / 字幕 / metadata / 缩略图嵌入 | ✅ | ✅ |
| 智能检测流媒体 | ✅ | ✅ |
| 浏览器 Cookies 整合 | ✅ | ✅ |
| Menu Bar 提示 / 通知 | ✅ | ✅ |
| 自动更新 | ✅ | ✅ |
| 视频长度上限 | **10 分钟** | 无限制 |
| 单次下载大小 | **100 MB** | 无限制 |
| 截取片段下载 | — | ✅ |
| 内嵌视频预览播放 | — | ✅ |

## 升级 Pro

- **价格**:NT$ 380 一次买断(约 USD $12)
- **设备数**:同一份授权可在最多 3 台 Mac 启用(可随时在设备上停用释出名额)
- **更新**:含 1 年内所有功能更新,1 年后可选 50% off 续约
- **退款**:7 天内无条件退款

[**到 momosoft.one 购买 Pro**](https://www.momosoft.one/nvd)

购买后 1 分钟内会收到授权码。打开 nvd → 设置 → 授权 → 升级 Pro → 「已有授权码?点此启用」填 Email + 授权码即可。

## 隐私

nvd 完全本地运行,**没有任何 telemetry / analytics**。唯一会连回服务器的时机是:
1. 启用 Pro 授权时验证一次
2. Sparkle 检查更新时拉取 appcast

完整隐私政策:[momosoft.one/Privacy.html](https://www.momosoft.one/Privacy.html)

## 内含的开源组件

nvd 内置以下开源组件供下载引擎使用:

- [yt-dlp](https://github.com/yt-dlp/yt-dlp) — Unlicense
- [ffmpeg](https://ffmpeg.org/) — LGPL/GPL
- [Sparkle](https://sparkle-project.org/) — MIT

## 著作权声明

nvd 是纯粹的视频下载工具,跟 yt-dlp、ffmpeg 等开源项目一样。用户下载内容前请确认你具有合法权利(自制内容、有授权的内容、合理使用范围)。

请尊重著作权人权益与各视频站服务条款。nvd 开发团队不对用户下载的内容负责。

## 客服与支持

- **客服邮箱**:[support@momosoft.one](mailto:support@momosoft.one)
- **问题反馈**:[Issues](https://github.com/Adam1313943/nvd-public/issues)
- **更新日志**:[CHANGELOG.md](./CHANGELOG.md)

---

© 2026 [MomoSoft](https://www.momosoft.one). All rights reserved.
