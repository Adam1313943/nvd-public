# Changelog

<p align="right">
  <a href="./CHANGELOG.md">English</a> · <strong>繁體中文</strong> · <a href="./CHANGELOG.zh-Hans.md">简体中文</a> · <a href="./CHANGELOG.ja.md">日本語</a>
</p>

所有重要的版本變更記錄在這個檔案。

## [0.3.9] - 2026-06-24

### 新增

- **暫停 / 繼續**（原生 HLS 下載）:下載中可暫停並保留進度,之後從目前進度續抓
- **提早完成並存檔**:下載到一半卡住、或不想等整支完成時,把已下載的部分合併成可播放的影片
- 匿名使用統計,協助診斷下載失敗原因(可於設定關閉)

### 改進

- 改善對更多串流網站的偵測與相容性(MacCMS 類播放器直接從頁面原始碼解析 m3u8)

## [0.3.6] - 2026-06-10

### 新增

- **字幕**:可手動勾選 / 指定字幕語言;「all」改成只抓原本字幕,避免被限流
- **yt-dlp 分段並行下載**(預設 4),長片大幅加速
- 任務清單:**清除已完成**

### 變更

- **免費版改制**:7 天免費試用 + 畫質上限 1080p(取代舊的 10 分鐘 / 100 MB 限制);Pro 解鎖 4K/8K、截取片段、內嵌播放

### 修正

- 截取片段:長度顯示成整支、進度卡 0%、字幕只抓到英文
- Pro 從截取片段下載被誤當免費版限制

## [0.3.5] - 2026-05-29

### 新增

- **License + Pro 升級系統**:支援 NVD-XXXX-XXXX-XXXX 授權碼啟用,使用 Keychain 安全儲存
  - 機器綁定(同一份授權可在 3 台 Mac 啟用)
  - 7 天離線寬限期
- **歡迎導引**:首次啟動 4 頁 onboarding,介紹工具與功能
- **系統 Chrome 偵測**:啟動時偵測 Chrome / Brave / Edge / Arc / Vivaldi,沒裝會在主畫面顯示提示橫幅引導下載
- **錯誤訊息友善化**:17 種常見錯誤類型對應友善提示,可展開技術細節
- **免費版限制**:影片長度上限 10 分鐘 / 單次下載上限 100 MB
- **設定 → 授權**:可看到目前授權狀態、停用、升級入口

### 改進

- **UI polish**:JobsView 加 hover lift 效果、狀態 chip 加 SF Symbol 動態 icon
- **SubmitView 重設計**:hero header + 加大 URL 輸入框 + 按鈕層次重排
- **Empty states**:任務 / 檔案頁沒內容時顯示 ContentUnavailableView

### 移除

- **設定 → 區段剪輯**:這個全域設定殘留值會偷偷砍下載長度,移到 ClipPickerWindow 內當下決定

### 修正

- 對 BunnyCDN 等短期 token 站的自動續期與重試邏輯
- m3u8 stream-proxy 強制回 200 + 不轉發 Range,修正 AVPlayer 反覆 retry master 卡住問題
- gzip 自動解 Content-Encoding
- isAccessExpired 改 case-insensitive

## [0.3.4] - 2026-05-27

- 通用 token-refresh download retry(BunnyCDN shortcut + 通用 sequence-align fallback)
- 移除設定內 sections 殘留值砍下載長度的 bug

## [0.3.3] - 2026-05-26

- HLS stream-proxy 多 candidate sniff + DVR 模式
- 短期 token 自動續期

## [0.3.2] - 2026-05-26

- Sniff fallback 給 PlayerWindow / ClipPickerWindow

## [0.3.1] - 2026-05-25

- Collision-safe filename
- 按鈕視覺改進
- yt-dlp generic 加上 `--extractor-args generic:impersonate`

## [0.3.0] - 2026-05-25

- 進入 Tier 1-3 完整 SwiftUI 主畫面
- Sparkle 自動更新整合
- Apple Developer ID 簽署 + Notarize
