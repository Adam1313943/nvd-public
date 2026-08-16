# nvd

> Video downloader for macOS & Windows — bundled tools, media library and AI subtitles. Ready out of the box.

<p align="right">
  <strong>English</strong> · <a href="./README.zh-Hant.md">繁體中文</a> · <a href="./README.zh-Hans.md">简体中文</a> · <a href="./README.ja.md">日本語</a>
</p>

<p align="center">
  <a href="https://www.momosoft.one/nvd">Website</a> ·
  <a href="https://github.com/Adam1313943/nvd-public/releases/latest">Download</a> ·
  <a href="https://www.momosoft.one/Privacy.html">Privacy</a>
</p>

---

## What is nvd

**nvd** is a video downloader for **macOS and Windows**. Turn any web video into a local file — no Homebrew, no yt-dlp setup, no terminal. Just install and go.

Works with **1,500+ video sites** including YouTube, Vimeo, Twitch, niconico, Bilibili, Twitter, Facebook, Instagram, TikTok and more.

## Key strengths

- **🎁 Ready out of the box** — yt-dlp, ffmpeg and a built-in stream sniffer bundled inside; no external browser or setup needed
- **🎯 Smart stream detection** — finds m3u8 even on JavaScript-heavy pages
- **📚 Media library** — organize downloads into sources, collections and playlists, with thumbnails
- **💬 AI subtitles** — generate subtitles on-device with whisper, then translate to many languages
- **▶️ Built-in player** — speed control, PiP, resume, and a subtitle overlay (size / position / drag to place)

## System Requirements

- **macOS** 14.0 Sonoma or later, Apple Silicon (M1 / M2 / M3 / M4)
- **Windows** 10 / 11, 64-bit
- ~300 MB disk space (AI subtitle models download on demand)

## Install

- **macOS** — download `nvd-*-mac-arm64.zip` from [Releases](https://github.com/Adam1313943/nvd-public/releases/latest), unzip, and drag `nvd.app` into `/Applications`.
- **Windows** — download `nvd-*-setup.exe` from [Releases](https://github.com/Adam1313943/nvd-public/releases/latest) and run the installer.

First launch shows a welcome guide. macOS Gatekeeper / Windows SmartScreen may warn on first open — choose **Open** / **Run anyway**.

## Free vs Pro

**Free** includes a **7-day trial**. After the trial, downloading and subtitle transcription require Pro.

| Feature | Free (7-day trial) | After trial | Pro |
|---|---|---|---|
| Download (1,500+ sites) | ✅ | Pro required | ✅ Unlimited |
| Media library / built-in player | ✅ | ✅ | ✅ |
| AI subtitles — transcription | ✅ | Pro required | ✅ Unlimited |
| AI subtitles — translation | Pro required | Pro required | ✅ 5 videos / month |

## Upgrade to Pro

- **Price**: US$15 one-time
- **Devices**: One license activates up to 3 devices (macOS / Windows); deactivate anytime to free a slot
- **Updates**: 1 year of feature updates included, then 50% off renewal
- **Refund**: 7-day no-questions-asked refund

[**Buy Pro on momosoft.one**](https://www.momosoft.one/nvd)

After purchase you'll receive the license key within 1 minute by email. Open nvd → Settings → License → Upgrade Pro → "Already have a key? Activate" — fill in your email and key.

## Privacy

nvd runs on your own machine. Outbound connections:

1. License verification (on activation)
2. Update check (`version.json`)
3. Anonymous usage analytics — on by default, can be turned off in Settings
4. Subtitle translation — only when you use it; sends the subtitle text to the translation service

Full policy: [momosoft.one/Privacy.html](https://www.momosoft.one/Privacy.html)

## Bundled Open Source

nvd ships with the following open-source components:

- [yt-dlp](https://github.com/yt-dlp/yt-dlp) — Unlicense
- [ffmpeg](https://ffmpeg.org/) — LGPL/GPL
- [whisper.cpp](https://github.com/ggml-org/whisper.cpp) — MIT (AI subtitle transcription)
- [Deno](https://deno.com/) — MIT (JavaScript runtime for some sites)
- [Electron](https://www.electronjs.org/) / Chromium — MIT / BSD

## Copyright Notice

nvd is a video downloader, much like yt-dlp and ffmpeg. Make sure you have the legal right to download any content (your own work, properly licensed material, or fair use). Respect copyright holders and the terms of service of each video site. nvd's authors are not responsible for the content users download.

## Support

- **Email**: [support@momosoft.one](mailto:support@momosoft.one)
- **Issues**: [GitHub Issues](https://github.com/Adam1313943/nvd-public/issues)
- **Changelog**: [CHANGELOG.md](./CHANGELOG.md)

---

© 2026 [MomoSoft](https://www.momosoft.one). All rights reserved.
