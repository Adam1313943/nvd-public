# Changelog

<p align="right">
  <a href="./CHANGELOG.md">English</a> · <a href="./CHANGELOG.zh-Hant.md">繁體中文</a> · <strong>简体中文</strong> · <a href="./CHANGELOG.ja.md">日本語</a>
</p>

所有重要的版本变更记录在这个文件。

## [0.4.0] - 2026-10-17

### 新增

- **媒体库**：把下载与既有文件整理成**来源**（本机文件夹、网络共享 / NAS、导入）、**合辑**与**播放列表**；每张卡片显示缩略图、时长与续播进度条；下载完成可一键加入媒体库
- **AI 字幕**：在本机用 whisper 生成字幕，提供两种识别模式——**标准**（对白）与**抑制噪声**（音乐、噪声较多的内容）——再翻译成多国语言；字幕以可调整大小、位置、可拖拽的自定义叠层呈现
- **内置播放器增强**：播放速度（0.5–2×，跨视频记住）、画中画（PiP）、记忆进度续播，以及非 MP4 容器（mkv / avi / flv / mov / ts）通过实时 remux 串流直接播放
- **导出媒体库**：把媒体库导出成 `.nvdlib` 文件，将来源、合辑、播放列表与观看进度带到 nvd iOS App；文件本体留在原处，只搬管理数据
- **从访达 / 资源管理器以 nvd 打开**：双击本机视频即可用 nvd 内置播放器播放

### 改进

- **可设置同时下载数**：自定义同时进行几个下载；每个下载的连接数会自动调降，维持在共用的连接预算内
- **链接新鲜度与续传**：下载前会重新探测过期链接获取新网址，下载途中遇到 403 也会用更新后的 cookie 续传

## [0.3.9] - 2026-06-24

### 新增

- **暂停 / 继续**（原生 HLS 下载）：下载中可暂停并保留进度，之后从当前进度续传
- **提前完成并保存**：下载卡住、或不想等整支完成时，把已下载的部分合并成可播放的视频
- 匿名使用统计，帮助诊断下载失败原因（可在设置中关闭）

### 改进

- 改善对更多流媒体网站的探测与兼容性（MacCMS 类播放器直接从页面源码解析 m3u8）

## [0.3.6] - 2026-06-10

### 新增

- **字幕**：可手动勾选 / 指定字幕语言；「all」改成只抓原始字幕，避免被限流
- **yt-dlp 分段并行下载**（默认 4），长视频大幅加速
- 任务列表：**清除已完成**

### 变更

- **免费版改制**：7 天免费试用 + 画质上限 1080p（取代旧的 10 分钟 / 100 MB 限制）；Pro 解锁 4K/8K、截取片段、内嵌播放

### 修复

- 截取片段：长度显示成整支、进度卡 0%、字幕只抓到英文
- Pro 从截取片段下载被误当免费版限制

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
