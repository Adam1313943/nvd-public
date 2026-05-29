# Changelog

<p align="right">
  <strong>English</strong> · <a href="./CHANGELOG.zh-Hant.md">繁體中文</a> · <a href="./CHANGELOG.zh-Hans.md">简体中文</a> · <a href="./CHANGELOG.ja.md">日本語</a>
</p>

All notable changes to this project are documented in this file.

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
