# Changelog

<p align="right">
  <strong>English</strong> · <a href="./CHANGELOG.zh-Hant.md">繁體中文</a> · <a href="./CHANGELOG.zh-Hans.md">简体中文</a> · <a href="./CHANGELOG.ja.md">日本語</a>
</p>

All notable changes to this project are documented in this file.

## [0.4.0] - 2026-10-17

### Added

- **Media library** — organize downloads and existing files into **sources** (local folders, network shares / NAS, and imports), **collections** and **playlists**, each card showing a thumbnail, duration and a resume bar; finished downloads can be added to the library in one click
- **AI subtitles** — generate subtitles on-device with whisper, with two recognition modes — **Standard** for dialogue and **Noise suppression** for music- or noise-heavy footage — then translate them into many languages; subtitles render as a custom overlay you can resize, reposition and drag
- **Built-in player** upgrades — playback speed (0.5–2×, remembered across videos), Picture-in-Picture, resume from where you left off, and direct playback of non-MP4 containers (mkv / avi / flv / mov / ts) via on-the-fly remux streaming
- **Export media library** — export your library to a `.nvdlib` file to carry your sources, collections, playlists and watch progress over to the nvd iOS app; files stay where they are, only the catalog moves
- **Open in nvd from Finder / Explorer** — double-click a local video to play it in nvd's built-in player

### Improved

- **Configurable simultaneous downloads** — choose how many downloads run at once; per-download connections scale down automatically to stay within a shared budget
- **Link freshness & resume** — expired links are re-sniffed for a fresh URL before downloading, and mid-download 403s recover with refreshed cookies

## [0.3.9] - 2026-06-24

### Added

- **Pause / Resume** for native HLS downloads — pause keeping progress, then continue from where you left off
- **Finish early & save** — when a download stalls or you don't want to wait, merge the already-downloaded part into a playable file
- Anonymous usage stats to help diagnose failed downloads (opt-out in Settings)

### Improved

- Better stream detection and compatibility across more sites (parse m3u8 straight from page source for MacCMS-style players)

## [0.3.6] - 2026-06-10

### Added

- **Subtitles**: pick specific subtitle languages; "all" now fetches only original subtitles to avoid throttling
- **yt-dlp concurrent fragments** (default 4) — much faster long videos
- Job list: **Clear finished**

### Changed

- **Free tier**: 7-day trial + 1080p quality cap (replaces the old 10-min / 100 MB limits); Pro unlocks 4K/8K, clip extraction, in-app playback

### Fixed

- Clip extraction: duration shown as full length, progress stuck at 0%, subtitles limited to English
- Pro downloads from clip extraction wrongly treated as free-tier limited

## [0.3.5] - 2026-05-29

### Added

- **License + Pro upgrade system**: Activate with `NVD-XXXX-XXXX-XXXX` license key, stored securely in Keychain
  - Machine binding (one license up to 3 Macs)
  - 7-day offline grace period
- **First-launch welcome guide**: 4-page onboarding introducing tools and features
- **System Chrome detection**: detects Chrome / Brave / Edge / Arc / Vivaldi at launch; shows orange banner with download CTA if none found
- **Friendly error messages**: 17 common error types mapped to actionable hints, with expandable technical details
- **Free tier limits**: video duration ≤ 10 minutes / per-download size ≤ 100 MB
- **Settings → License**: see current license status, deactivate, or open upgrade flow

### Improved

- **UI polish**: JobsView hover lift effect, status chip with animated SF Symbols
- **SubmitView redesign**: hero header + enlarged URL input + Pro chip
- **Empty states**: Jobs / Files screens show ContentUnavailableView guidance when empty

### Removed

- **Settings → Clip range**: this global setting could silently truncate downloads, moved to ClipPickerWindow where the user picks the range explicitly

### Fixed

- Auto token refresh for short-lived signed URLs (BunnyCDN etc.)
- m3u8 stream-proxy forces 200 + does not forward Range upstream, fixing AVPlayer repeatedly retrying master
- Auto-decode `Content-Encoding: gzip`
- `isAccessExpired` case-insensitive comparison

## [0.3.4] - 2026-05-27

- Generic token-refresh download retry (BunnyCDN shortcut + generic sequence-align fallback)
- Removed clip-section setting that silently truncated downloads

## [0.3.3] - 2026-05-26

- HLS stream-proxy with multi-candidate sniffing + DVR mode
- Auto refresh for short-lived signed URLs

## [0.3.2] - 2026-05-26

- Sniff fallback for PlayerWindow / ClipPickerWindow

## [0.3.1] - 2026-05-25

- Collision-safe output filenames
- Button visual improvements
- `--extractor-args generic:impersonate` for yt-dlp generic extractor

## [0.3.0] - 2026-05-25

- Tier 1–3 complete SwiftUI main UI
- Sparkle auto-update integration
- Apple Developer ID code signing + Notarize
