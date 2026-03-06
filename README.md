# ZenTerm 🧘‍♂️📱

[日本語 (Japanese)](./README_ja.md)

<div align="center">
  <img src="ZenTerm-logo-128.png" alt="ZenTerm Banner">
</div>

**"Don't leave your bed. Hack AI while lying down."**

ZenTerm is a highly specialized Android SSH client designed for lazy hackers who want to control AI CLI tools (like Claude Code or local LLMs) straight from their beds. 

We completely eliminated the stress of "clunky arrow keys" and "broken CJK input" found in traditional mobile terminals by implementing hardware button hacks and a custom inline UI.

---

## 🔥 Killer Features

### 1. Volume Button CLI Hack 🎛️
Stop struggling with the tiny arrow keys on your soft keyboard.
ZenTerm intercepts your Android's physical **Volume UP / DOWN buttons** and converts them into `↑` and `↓` arrow key strokes in the terminal. Navigate prompt history and CLI menus flawlessly with one hand, without even looking at the screen.

### 2. Flawless IME & Voice Input 🗣️
Using a custom inline input overlay over xterm.js, ZenTerm provides 100% stable support for Gboard and other IME keyboards (including Japanese flick input and Voice Typing). No more garbled characters. Code with your voice.

### 3. Tmux-Optimized Seamless Resume 🔄
Mobile connections drop when the screen sleeps. ZenTerm is built with this in mind.
When you reopen the app, it reconnects and automatically runs `tmux attach`, restoring your exact workspace in a split second.

### 4. AI-Focused Toolbar 🛠️
Essential keys for LLM interaction and Vim (`Ctrl+C`, `Esc`, `Tab`, `Shift`) are permanently docked on the toolbar. Stop rogue AI loops with a single tap of your thumb.

### 5. Zero-Config Claude Code Buttons ⚡
No need to set up custom macros. ZenTerm comes pre-loaded with a dedicated "Claude" toolbar menu. Instantly launch Claude, run the verbose `--dangerously-skip-permissions` flag, or hit `--resume` with a single tap. It also includes built-in quick keys for LLM interactions, such as `Mode Switch (Shift+Tab)`, `^C`, and `^D`.

---

## 📥 Download
[![Get it on Google Play](https://play.google.com/intl/en_us/badges/static/images/badges/en_badge_web_generic.png)](https://play-lh.googleusercontent.com/...)
*(Coming Soon)*

---

## ⚙️ How to Use

### Enabling Volume Button Hack
1. Tap the **Settings (Gear)** icon in the top right corner.
2. Toggle on **"Volume Button Hack"**.
   * *Note: While enabled and the terminal is active, you cannot change your device's media volume.*
3. Go back to the terminal. Press `Volume UP` to navigate to the previous command (Up Arrow), and `Volume DOWN` for the next command (Down Arrow).

---

## 🐛 Support & Issues

ZenTerm is an indie project. If you find a bug or want to request a new macro button, please open an issue in this repository.

* **[Create a New Issue](https://github.com/nemucodes/ZenTerm/issues/new)**

---

## 👤 Developer
**Nemu** ([@nemucodes](https://x.com/nemucodes))  
*Building tools for lazy hackers.*
