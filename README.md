# nvd

> Native video downloader for macOS — bundled tools, ready out of the box.

<p align="right">
  <strong>English</strong> · <a href="./README.zh-Hant.md">繁體中文</a> · <a href="./README.zh-Hans.md">简体中文</a> · <a href="./README.ja.md">日本語</a>
</p>

<p align="center">
  <img src="docs/screenshots/hero.png" alt="nvd hero" width="720">
</p>

<p align="center">
  <a href="https://www.momosoft.one/nvd">Website</a> ·
  <a href="https://github.com/Adam1313943/nvd-public/releases/latest">Download</a> ·
  <a href="https://www.momosoft.one/Privacy.html">Privacy</a>
</p>

---

## What is nvd

**nvd** is a native macOS video downloader. Turn any web video into a local file — no Homebrew, no yt-dlp setup, no terminal. Just double-click and go.

Works with **1,500+ video sites** including YouTube, Vimeo, Twitch, niconico, Bilibili, Twitter, Facebook, Instagram, TikTok and more.

## Three key strengths

- **🎁 Ready out of the box** — yt-dlp and ffmpeg bundled inside the app
- **🎯 Smart stream detection** — finds m3u8 even on JavaScript-heavy pages
- **🔄 Stable long-form downloads** — handles HLS variants and session refresh automatically

## System Requirements

- macOS 14.0 Sonoma or later
- Apple Silicon (M1 / M2 / M3 / M4)
- ~250 MB disk space
- **Smart detection requires**: Chrome / Brave / Edge / Arc / Vivaldi (any one — most Macs already have one). Standard yt-dlp sites do not need this.

## Install

1. Download the latest `nvd-*.zip` from [Releases](https://github.com/Adam1313943/nvd-public/releases/latest)
2. Unzip and drag `nvd.app` into `/Applications`
3. Double-click to open — first launch shows a welcome guide

On first launch, macOS Gatekeeper may show a download confirmation. Click "Open" to continue.

## Free vs Pro

| Feature | Free | Pro |
|---|---|---|
| 1,500+ supported sites | ✅ | ✅ |
| Resolution / subtitle / metadata / thumbnail embed | ✅ | ✅ |
| Smart stream detection | ✅ | ✅ |
| Browser cookies integration | ✅ | ✅ |
| Menu Bar status / notifications | ✅ | ✅ |
| Auto update | ✅ | ✅ |
| Video duration limit | **10 minutes** | Unlimited |
| Per-download size limit | **100 MB** | Unlimited |
| Clip selection download | — | ✅ |
| In-app preview playback | — | ✅ |

## Upgrade to Pro

- **Price**: NT$ 380 one-time (~USD $12)
- **Devices**: One license activates up to 3 Macs (deactivate any anytime to free a slot)
- **Updates**: 1 year of feature updates included, then 50% off renewal
- **Refund**: 7-day no-questions-asked refund

[**Buy Pro on momosoft.one**](https://www.momosoft.one/nvd)

After purchase you'll receive the license key within 1 minute by email. Open nvd → Settings → License → Upgrade Pro → "Already have a key? Activate" — fill in your email and key.

## Privacy

nvd runs entirely on your Mac. **No telemetry, no analytics.** The only outbound connections:
1. License verification on activation
2. Sparkle update check (appcast.xml)

Full policy: [momosoft.one/Privacy.html](https://www.momosoft.one/Privacy.html)

## Bundled Open Source

nvd ships with the following open-source download engine components:

- [yt-dlp](https://github.com/yt-dlp/yt-dlp) — Unlicense
- [ffmpeg](https://ffmpeg.org/) — LGPL/GPL
- [Sparkle](https://sparkle-project.org/) — MIT

## Copyright Notice

nvd is a video downloader, much like yt-dlp and ffmpeg. Make sure you have the legal right to download any content (your own work, properly licensed material, or fair use). Respect copyright holders and the terms of service of each video site. nvd's authors are not responsible for the content users download.

## Support

- **Email**: [support@momosoft.one](mailto:support@momosoft.one)
- **Issues**: [GitHub Issues](https://github.com/Adam1313943/nvd-public/issues)
- **Changelog**: [CHANGELOG.md](./CHANGELOG.md)

---

© 2026 [MomoSoft](https://www.momosoft.one). All rights reserved.
