# Changelog

<p align="right">
  <a href="./CHANGELOG.md">English</a> · <a href="./CHANGELOG.zh-Hant.md">繁體中文</a> · <a href="./CHANGELOG.zh-Hans.md">简体中文</a> · <strong>日本語</strong>
</p>

このプロジェクトの重要な変更履歴を記録しています。

## [0.3.5] - 2026-05-29

### 追加

- **ライセンス + Pro アップグレードシステム**:`NVD-XXXX-XXXX-XXXX` 形式のライセンスキーで認証、Keychain で安全に保存
  - デバイスバインディング(1 ライセンスで最大 3 台の Mac)
  - 7 日間のオフライン猶予期間
- **初回起動時のウェルカムガイド**:4 ページのオンボーディングでツールと機能を紹介
- **システム Chrome 検出**:起動時に Chrome / Brave / Edge / Arc / Vivaldi を検出。見つからない場合はメイン画面にダウンロード案内のバナーを表示
- **エラーメッセージのわかりやすい表示**:17 種類の一般的なエラーをユーザー向けのヒントにマッピング、技術詳細は展開可能
- **無料版の制限**:動画の長さ 10 分以下 / 1 回のダウンロード 100 MB 以下
- **設定 → ライセンス**:現在のライセンス状態を確認、解除、アップグレード入口

### 改善

- **UI 改良**:JobsView の hover lift 効果、ステータスチップに SF Symbol のアニメーションアイコン
- **SubmitView 再設計**:hero header + 大きめの URL 入力欄 + Pro chip
- **Empty states**:タスク / ファイル画面が空のときに ContentUnavailableView でガイド表示

### 削除

- **設定 → クリップ範囲**:このグローバル設定が残っているとダウンロードが意図せず短く切られる問題があったため、ClipPickerWindow 側でその場で選ぶ方式に変更

### 修正

- BunnyCDN など短時間トークンサイトの自動更新と再試行ロジック
- m3u8 stream-proxy が 200 を強制、Range をアップストリームに転送しないように修正(AVPlayer が master を繰り返し再試行する問題)
- `Content-Encoding: gzip` の自動デコード
- `isAccessExpired` を case-insensitive に修正

## [0.3.4] - 2026-05-27

- 汎用 token-refresh ダウンロード再試行(BunnyCDN ショートカット + 汎用 sequence-align フォールバック)
- 設定内の sections 残存値でダウンロードが切られるバグを修正

## [0.3.3] - 2026-05-26

- HLS stream-proxy のマルチ候補 sniff + DVR モード
- 短時間トークンの自動更新

## [0.3.2] - 2026-05-26

- PlayerWindow / ClipPickerWindow に sniff フォールバック

## [0.3.1] - 2026-05-25

- 衝突を避けるファイル名生成
- ボタンのビジュアル改善
- yt-dlp generic に `--extractor-args generic:impersonate` を追加

## [0.3.0] - 2026-05-25

- Tier 1-3 完全な SwiftUI メイン画面
- Sparkle 自動アップデート統合
- Apple Developer ID コード署名 + Notarize
