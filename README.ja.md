# nvd

> macOS と Windows 向けの動画ダウンローダー。ツール内蔵・メディアライブラリ・AI 字幕、すぐに使えます。

<p align="right">
  <a href="./README.md">English</a> · <a href="./README.zh-Hant.md">繁體中文</a> · <a href="./README.zh-Hans.md">简体中文</a> · <strong>日本語</strong>
</p>

<p align="center">
  <a href="https://www.momosoft.one/nvd">公式サイト</a> ·
  <a href="https://github.com/Adam1313943/nvd-public/releases/latest">最新版をダウンロード</a> ·
  <a href="https://www.momosoft.one/Privacy.html">プライバシー</a>
</p>

---

## nvd とは

**nvd** は **macOS と Windows** 向けの動画ダウンローダーです。Web 上の動画をローカルファイルに — Homebrew も yt-dlp のセットアップもターミナルも不要。インストールするだけで使えます。

YouTube、Vimeo、Twitch、niconico、Bilibili、Twitter、Facebook、Instagram、TikTok など **1,500 以上の動画サイト**に対応。

## 主な特長

- **🎁 すぐに使える** — yt-dlp / ffmpeg とストリーム検出エンジンを内蔵。別途ブラウザやセットアップは不要
- **🎯 スマートなストリーム検出** — JavaScript 主体のページでも m3u8 を検出
- **📚 メディアライブラリ** — ダウンロードをソース・コレクション・プレイリストで整理、サムネイル表示
- **💬 AI 字幕** — ローカルの whisper で字幕を生成し、多言語へ翻訳
- **▶️ 内蔵プレーヤー** — 速度・PiP・再開、字幕オーバーレイ（サイズ / 位置 / ドラッグ移動）

## 動作環境

- **macOS** 14.0 Sonoma 以降、Apple Silicon (M1 / M2 / M3 / M4)
- **Windows** 10 / 11、64bit
- 約 300 MB の空き容量（AI 字幕モデルは使用時にダウンロード）

## インストール

- **macOS** — [Releases](https://github.com/Adam1313943/nvd-public/releases/latest) から `nvd-*-mac-arm64.zip` をダウンロードし、解凍して `nvd.app` を `/Applications` へドラッグ。
- **Windows** — [Releases](https://github.com/Adam1313943/nvd-public/releases/latest) から `nvd-*-setup.exe` をダウンロードしてインストーラーを実行。

初回起動時にようこそガイドが表示されます。初回は macOS Gatekeeper / Windows SmartScreen が警告する場合があります。「**開く**」/「**実行**」を選んでください。

## 無料版 vs Pro

**無料版**には **7 日間のトライアル**が含まれます。トライアル終了後、ダウンロードと字幕の文字起こしには Pro が必要です。

| 機能 | 無料（トライアル 7 日間） | トライアル終了後 | Pro |
|---|---|---|---|
| ダウンロード（1,500 以上のサイト） | ✅ | Pro が必要 | ✅ 無制限 |
| メディアライブラリ / 内蔵プレーヤー | ✅ | ✅ | ✅ |
| AI 字幕 — 文字起こし | ✅ | Pro が必要 | ✅ 無制限 |
| AI 字幕 — 翻訳 | Pro が必要 | Pro が必要 | ✅ 月 5 本 |

## Pro へアップグレード

- **価格**：US$15 買い切り
- **デバイス数**：1 ライセンスで最大 3 台（macOS / Windows）まで有効化。いつでも解除して枠を空けられます
- **アップデート**：1 年間の機能アップデート込み、以降は 50% off で更新可
- **返金**：7 日間の無条件返金

[**momosoft.one で Pro を購入**](https://www.momosoft.one/nvd)

購入後 1 分以内にライセンスキーがメールで届きます。nvd → 設定 → ライセンス → Pro へアップグレード →「キーをお持ちの方はこちら」でメールとキーを入力してください。

## プライバシー

nvd は基本的にお使いの端末のローカルで動作します。外部への通信は次の場合のみ：

1. アクティベーション時のライセンス検証
2. アップデート確認（`version.json`）
3. 匿名の利用状況分析 — 既定でオン、「設定」でオフにできます
4. 字幕翻訳 — 使用時のみ。字幕テキストを翻訳サービスへ送信します

プライバシーポリシー全文：[momosoft.one/Privacy.html](https://www.momosoft.one/Privacy.html)

## 同梱のオープンソース

nvd は以下のオープンソースコンポーネントを同梱しています：

- [yt-dlp](https://github.com/yt-dlp/yt-dlp) — Unlicense
- [ffmpeg](https://ffmpeg.org/) — LGPL/GPL
- [whisper.cpp](https://github.com/ggml-org/whisper.cpp) — MIT（AI 字幕の文字起こし）
- [Deno](https://deno.com/) — MIT（一部サイト向けの JS ランタイム）
- [Electron](https://www.electronjs.org/) / Chromium — MIT / BSD

## 著作権について

nvd は yt-dlp や ffmpeg と同様、純粋な動画ダウンローダーです。ダウンロードするコンテンツについて、正当な権利（自作物、適切にライセンスされた素材、フェアユースの範囲）を有していることを確認してください。著作権者の権利と各動画サイトの利用規約を尊重してください。ユーザーがダウンロードしたコンテンツについて、nvd の作者は責任を負いません。

## サポート

- **メール**：[support@momosoft.one](mailto:support@momosoft.one)
- **不具合報告**：[Issues](https://github.com/Adam1313943/nvd-public/issues)
- **変更履歴**：[CHANGELOG.md](./CHANGELOG.md)

---

© 2026 [MomoSoft](https://www.momosoft.one). All rights reserved.
