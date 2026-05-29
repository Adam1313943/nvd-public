# nvd

> macOS 向け動画ダウンローダー。ツール内蔵、インストール後すぐに使えます。

<p align="right">
  <a href="./README.md">English</a> · <a href="./README.zh-Hant.md">繁體中文</a> · <a href="./README.zh-Hans.md">简体中文</a> · <strong>日本語</strong>
</p>

<p align="center">
  <img src="docs/screenshots/hero.png" alt="nvd hero" width="720">
</p>

<p align="center">
  <a href="https://www.momosoft.one/nvd">公式サイト</a> ·
  <a href="https://github.com/Adam1313943/nvd-public/releases/latest">最新版をダウンロード</a> ·
  <a href="https://www.momosoft.one/Privacy.html">プライバシーポリシー</a>
</p>

---

## nvd とは

**nvd** は macOS ネイティブの動画ダウンローダーです。ウェブの動画をローカルファイルに変換 — Homebrew や yt-dlp のセットアップ不要、ターミナル操作不要。ダブルクリックで起動するだけです。

YouTube、Vimeo、Twitch、niconico、Bilibili、Twitter、Facebook、Instagram、TikTok など **1,500 以上の動画サイト** に対応しています。

## 三つの強み

- **🎁 すぐに使える** — yt-dlp / ffmpeg を内蔵。Homebrew のインストールやコマンド操作は不要
- **🎯 スマートなストリーム検出** — JavaScript で動的に読み込まれるページでも m3u8 を自動検出
- **🔄 安定した長尺ダウンロード** — 複数の HLS バリアントとセッション更新を自動処理し、長時間動画でも途中で止まらない

## 動作環境

- macOS 14.0 Sonoma 以上
- Apple Silicon (M1 / M2 / M3 / M4)
- 約 250 MB のディスク容量
- **スマート検出機能には以下が必要**:Chrome / Brave / Edge / Arc / Vivaldi のいずれか一つ(多くの Mac にはすでにインストール済み)。標準的な yt-dlp 対応サイトでは不要

## インストール

1. [Releases](https://github.com/Adam1313943/nvd-public/releases/latest) から最新版の `nvd-*.zip` をダウンロード
2. 解凍して `nvd.app` を `/Applications` にドラッグ
3. ダブルクリックで起動 — 初回起動時にウェルカムガイドが表示されます

初回起動時に macOS Gatekeeper の「インターネットからダウンロードされた」確認が出る場合があります。「開く」をクリックしてください。

## 無料版 vs Pro

| 機能 | 無料版 | Pro |
|---|---|---|
| 1,500+ サイト対応 | ✅ | ✅ |
| 解像度 / 字幕 / メタデータ / サムネイル埋め込み | ✅ | ✅ |
| スマートなストリーム検出 | ✅ | ✅ |
| ブラウザ Cookies 統合 | ✅ | ✅ |
| メニューバー通知 | ✅ | ✅ |
| 自動アップデート | ✅ | ✅ |
| 動画の長さ上限 | **10 分** | 無制限 |
| 1 回のダウンロードサイズ | **100 MB** | 無制限 |
| クリップ範囲ダウンロード | — | ✅ |
| アプリ内プレビュー再生 | — | ✅ |

## Pro へのアップグレード

- **価格**:¥ 1,500 買い切り(NT$ 380 / USD $12 相当)
- **デバイス数**:1 ライセンスで最大 3 台の Mac でアクティベート可能(いつでも解除可能)
- **アップデート**:1 年間のすべての機能アップデートを含む。1 年後は 50% 割引で更新可能
- **返金**:7 日以内なら無条件返金

[**momosoft.one で Pro を購入**](https://www.momosoft.one/nvd)

購入後 1 分以内にライセンスキーがメールで届きます。nvd を起動 → 設定 → ライセンス → Pro にアップグレード → 「ライセンスをお持ちの方はこちら」を選択 → メールアドレスとキーを入力してください。

## プライバシー

nvd は完全にローカルで動作し、**テレメトリや解析は一切行いません**。サーバー通信が発生するのは以下のみ:
1. Pro ライセンス認証時の検証
2. Sparkle によるアップデート確認

完全なポリシー: [momosoft.one/Privacy.html](https://www.momosoft.one/Privacy.html)

## 同梱されているオープンソース

nvd には以下のオープンソースコンポーネントがダウンロードエンジンとして同梱されています:

- [yt-dlp](https://github.com/yt-dlp/yt-dlp) — Unlicense
- [ffmpeg](https://ffmpeg.org/) — LGPL/GPL
- [Sparkle](https://sparkle-project.org/) — MIT

## 著作権について

nvd は yt-dlp や ffmpeg と同様、純粋な動画ダウンロードツールです。コンテンツをダウンロードする前に、合法的な権利があることをご確認ください(自作コンテンツ、適切にライセンスされたもの、フェアユース範囲内など)。

著作権者の権利と各動画サイトの利用規約を尊重してください。nvd の開発者は、ユーザーがダウンロードしたコンテンツについて責任を負いません。

## サポート

- **メール**:[support@momosoft.one](mailto:support@momosoft.one)
- **Issues**:[GitHub Issues](https://github.com/Adam1313943/nvd-public/issues)
- **変更履歴**:[CHANGELOG.md](./CHANGELOG.md)

---

© 2026 [MomoSoft](https://www.momosoft.one). All rights reserved.
