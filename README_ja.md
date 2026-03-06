# ZenTerm 🧘‍♂️📱

<div align="center">
  <img src="ZenTerm-logo-128.png" alt="ZenTerm Banner">
</div>


**"ベッドから出るな。寝ながらAIを操れ。"**

ZenTermは、Claude CodeやローカルLLMなどの「AI CLIツール」を、Androidスマートフォンから快適に操作するために開発された**変態的**なSSHターミナルアプリです。
既存のターミナルアプリが抱える「日本語入力のストレス」と「スマホでのキー操作のしんどさ」を、物理ボタンのハックと独自UIで完全に解決しました。

---

## 🔥 キラー機能 (Features)

### 1. 音量ボタンによるCLI操作ハック 🎛️
ソフトウェアキーボードの矢印キーやEnterキーをちまちま押す必要はもうありません。
Androidの物理的な**「音量UP / DOWNボタン」**をターミナルの「↑ / ↓」キーに変換。画面を見ずに、片手でプロンプト履歴や選択肢をサクサク移動できます。

### 2. フリック＆音声入力に完全対応 🗣️
xterm.jsベースのターミナルに独自のインライン入力オーバーレイを被せています。
Gboard等の日本語フリック入力や音声入力が**一切文字化けせず、完璧に動作します**。寝言でコーディングが可能です。

### 3. Tmux特化のシームレス復帰 🔄
スマホ特有の「画面スリープによる接続切れ」を前提とした設計。
アプリを開き直した際、切断されていてもワンタップ（または自動）で元のTmuxセッションに `tmux attach` し、前の作業状態に一瞬で復帰します。

### 4. AI操作に特化した専用ツールバー 🛠️
「Ctrl+C」「Esc」「Tab」など、LLMとの対話やエディタ操作に必須のキーをツールバーに常時配置。親指一つでAIの暴走を止められます。

---

## 📥 ダウンロード (Download)
[![Get it on Google Play](https://play.google.com/intl/en_us/badges/static/images/badges/en_badge_web_generic.png)](https://play.google.com/store/apps/details?id=com.nemucodes.zenterm)  
*(※現在審査中 / Coming Soon)*

---

## ⚙️ 使い方・設定 (How to Use)

### 音量ボタンハックの設定
1. アプリ右上の「歯車（Settings）」アイコンをタップします。
2. 「Volume Button Hack」のトグルをONにします。
   * *※この設定がONの間、ターミナル画面を開いている時はスマホのメディア音量は変更できなくなります。*
3. ターミナルに戻り、音量UPを押すとコマンド履歴が一つ前に戻り（↑キー）、DOWNを押すと次へ進みます（↓キー）。

### 音声入力でプロンプトを投げる
1. ツールバーの「マイク」アイコン（または入力フィールド）をタップします。
2. Google音声入力等で「ここをリファクタリングして」と喋ります。
3. そのまま送信（Enter）を押すと、ターミナルに日本語文字列が流し込まれます。

---

## 🐛 バグ報告と機能要望 (Support \u0026 Issues)

ZenTermは個人開発のプロジェクトです。
バグを見つけた場合や、「こんなマクロボタンが欲しい！」という要望がある場合は、このリポジトリの [Issues](https://github.com/nemucodes/ZenTerm-Docs/issues) からお気軽に報告してください。

* **[Create a New Issue](https://github.com/nemucodes/ZenTerm-Docs/issues/new)**

---

## 👤 開発者 (Developer)
**Nemu** ([@nemucodes](https://x.com/nemucodes))  
*Building tools for lazy hackers.*
