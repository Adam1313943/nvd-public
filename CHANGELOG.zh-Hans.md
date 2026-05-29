# Changelog

<p align="right">
  <a href="./CHANGELOG.md">English</a> · <a href="./CHANGELOG.zh-Hant.md">繁體中文</a> · <strong>简体中文</strong> · <a href="./CHANGELOG.ja.md">日本語</a>
</p>

所有重要的版本变更记录在这个文件。

## [0.3.5] - 2026-05-29

### 新增

- **License + Pro 升级系统**:支持 NVD-XXXX-XXXX-XXXX 授权码激活,使用 Keychain 安全存储
  - 设备绑定(同一份授权可在 3 台 Mac 激活)
  - 7 天离线宽限期
- **欢迎引导**:首次启动 4 页 onboarding,介绍工具与功能
- **系统 Chrome 检测**:启动时检测 Chrome / Brave / Edge / Arc / Vivaldi,没装会在主界面显示提示横幅引导下载
- **错误信息友好化**:17 种常见错误类型对应友好提示,可展开技术细节
- **免费版限制**:视频长度上限 10 分钟 / 单次下载上限 100 MB
- **设置 → 授权**:可看到当前授权状态、停用、升级入口

### 改进

- **UI polish**:JobsView 加 hover lift 效果、状态 chip 加 SF Symbol 动态 icon
- **SubmitView 重设计**:hero header + 加大 URL 输入框 + 按钮层次重排
- **Empty states**:任务 / 文件页没内容时显示 ContentUnavailableView

### 移除

- **设置 → 区段剪辑**:这个全局设置残留值会偷偷砍下载长度,移到 ClipPickerWindow 内当下决定

### 修正

- 对 BunnyCDN 等短期 token 站的自动续期与重试逻辑
- m3u8 stream-proxy 强制回 200 + 不转发 Range,修正 AVPlayer 反复 retry master 卡住问题
- gzip 自动解 Content-Encoding
- isAccessExpired 改 case-insensitive

## [0.3.4] - 2026-05-27

- 通用 token-refresh download retry(BunnyCDN shortcut + 通用 sequence-align fallback)
- 移除设置内 sections 残留值砍下载长度的 bug

## [0.3.3] - 2026-05-26

- HLS stream-proxy 多 candidate sniff + DVR 模式
- 短期 token 自动续期

## [0.3.2] - 2026-05-26

- Sniff fallback 给 PlayerWindow / ClipPickerWindow

## [0.3.1] - 2026-05-25

- Collision-safe filename
- 按钮视觉改进
- yt-dlp generic 加上 `--extractor-args generic:impersonate`

## [0.3.0] - 2026-05-25

- 进入 Tier 1-3 完整 SwiftUI 主界面
- Sparkle 自动更新集成
- Apple Developer ID 签署 + Notarize
