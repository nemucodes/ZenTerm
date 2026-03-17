<p align="center">
  <img src="ZenTerm-logo-128.png" alt="ZenTerm" width="128" height="128">
</p>

<h1 align="center">ZenTerm</h1>

<p align="center">
  <strong>Claude CodeとAI開発者のためのAndroid SSHターミナル</strong>
</p>

<p align="center">
  <a href="#機能">機能</a> •
  <a href="#スクリーンショット">スクショ</a> •
  <a href="#推奨セットアップ">セットアップ</a> •
  <a href="#ダウンロード">ダウンロード</a> •
  <a href="PRIVACY_POLICY.md">プライバシーポリシー</a>
</p>

<p align="center">
  <a href="README.md">English</a>
</p>

---

既存のSSHクライアントはサーバーに繋いで設定を確認して切断、という短時間の作業を想定して作られています。ZenTermは違います。リモートマシンにSSHしてAIエージェントを動かし、出力を確認し、フローを維持する——ノートPCなしで。

tmuxみたいないい技術があるのだから、ただ「たまたま動く」んじゃなくて、ちゃんと活かすアプリが欲しかった。

## 機能

### 音量ボタン → カーソルキー

モバイルでのターミナル操作で最大の壁はカーソル移動。ZenTermは音量ボタンを矢印キーにマッピングします。方向の反転やロングプレスも設定可能。外付けキーボードなしでClaude Codeのメニュー操作を快適にナビゲートできます。

### Claude Code に最適化

- Claude Code 動作中を自動検出 → ツールバーが自動で切り替わる
- ワンタップ起動: `claude` / `--dangerously-skip-permissions` / `--resume`
- カスタマイズ可能なコマンドボタン: `/clear`, `/new`, `/model`, `^C`, `^D` など
- 256色 + トゥルーカラー対応

### tmuxネイティブな操作体験

- 接続時にtmuxセッションを自動作成 or 既存セッションにアタッチ
- マルチタブ対応（最大5タブ）、各タブが独立したtmuxウィンドウ
- ツールバーからペイン分割（水平/垂直）・ナビゲーション・削除
- **Monitorモード**: 外部tmuxセッションに読み取り専用でアタッチ——長時間動くAIエージェントの進捗を、うっかりキーを押す心配なく眺められる
- プレフィックスキー設定可能（C-b / C-a / C-space またはカスタム）

### SFTPファイルブラウザ

- 20以上の言語に対応したシンタックスハイライト（Dart, Python, JS, Rust, Go など）
- Markdownレンダリング（ソース表示への切り替え可能）
- 画像プレビュー＋ピンチズーム（PNG / JPG / GIF / WebP）

### 音声入力

Google Speech Servicesを使って、音声でターミナルにコマンドを入力できます。

### セキュリティ設計

- SSH認証情報はAndroid Keystoreで暗号化（平文保存なし）
- アナリティクスなし・テレメトリなし——データはデバイスの外に出ない
- 権限はINTERNETのみ。連絡先・ストレージ・位置情報へのアクセスなし
- dartssh2（Pure Dart SSH）採用——ネイティブバイナリなし、隠れた通信なし

## スクリーンショット

<p align="center">
  <img src="screenshots/01_splash.png" width="180">
  <img src="screenshots/02_claude.png" width="180">
  <img src="screenshots/03_settings.png" width="180">
  <img src="screenshots/04_pane.png" width="180">
</p>

<p align="center">
  <img src="screenshots/05_sftp.png" width="180">
  <img src="screenshots/06_syntax.png" width="180">
  <img src="screenshots/07_markdown.png" width="180">
  <img src="screenshots/08_voice.png" width="180">
</p>

## 推奨セットアップ

```
Androidスマートフォン / タブレット
     ↓ Tailscale経由でSSH
自宅PC / 開発サーバー（tmuxインストール済み）
     ↓
tmux上で動くClaude Code
```

[Tailscale](https://tailscale.com/)を両デバイスにインストールするだけで、ポート開放不要・VPN設定不要で自宅マシンに安全にアクセスできます。

> **注意:** ZenTermはリモートサーバーにtmuxがインストールされている必要があります。マルチタブ・Monitorモード・ペイン操作などの主要機能はtmux統合に依存しています。

## ダウンロード

<!-- Play Storeバッジは公開後に追加 -->
**Google Playで近日公開** — 買い切り、サブスクリプションなし。

## サポート

- お問い合わせ: nemucodes@gmail.com
- プライバシーポリシー: [PRIVACY_POLICY.md](PRIVACY_POLICY.md)

## 技術スタック

[Flutter](https://flutter.dev/) と [dartssh2](https://pub.dev/packages/dartssh2) で構築。

---

<p align="center">
  <strong>nemucodes</strong><br>
  Building tools for lazy hackers.
</p>
