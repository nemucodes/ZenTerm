# Features of ZenTerm 🧘‍♂️📱

ZenTerm is built with a singular focus: **Making LLM CLI tools (like Claude Code) usable and relaxing on Android.** We stripped away the bloat of traditional SSH clients and engineered specific hacks to overcome the limitations of mobile keyboards.

Here is what makes ZenTerm unique:

## ⚡ Claude Code Optimization (The Killer Features)

* **Physical Volume Button Hack**: We intercept Android's native volume buttons via MethodChannel. 
  * `Volume Up` sends `↑` (previous command).
  * `Volume Down` sends `↓` (next command).
  * `Long Press` sends `Enter` (Submit).
  * *You can literally navigate histories and select options with one hand without looking at the screen.*
* **Dynamic Claude Toolbar**: Automatically detects if `claude` or `node` is running in the current tmux pane.
  * **Not running**: Shows 1-tap launch buttons for `claude`, `bypass (--dangerously-skip-permissions)`, and `resume`.
  * **Running**: Switches to LLM interaction keys like `Mode (Shift+Tab)` to switch between Plan/Act/Auto-Edit, `^C` to stop generation, and `^D`.
* **Integrated Stderr**: Claude Code renders its UI via `stderr`. Most SSH clients hide or buffer this incorrectly. ZenTerm merges `stdout` and `stderr` streams seamlessly so the Claude UI renders perfectly in real-time.
* **Inline Voice & CJK Input Overlay**: Traditional `xterm.js` struggles with Android's Gboard (flick input/voice typing). We built a dedicated floating overlay that lets you dictate your prompts naturally in Japanese/English, edit the text, and inject it cleanly into the terminal.

## 🔄 Bulletproof Tmux Integration

Mobile connections drop when your screen turns off. Instead of fighting Android's background execution limits, ZenTerm embraces Tmux as the backbone of session management.

* **Auto-Tmux Wrapping**: If tmux is installed on your server, ZenTerm wraps your SSH session automatically.
* **Linked Sessions Architecture**: Each tab in ZenTerm is a separate, linked tmux window (`tmux new-session -t`). You can manage multiple tabs natively in the app, but they share the same underlying session group.
* **Silent Reconnects**: If you lose connection on a train, tap "Reconnect" and your exact window state, running commands, and scrollback are restored instantly.
* **Read-only Monitor Mode**: Started a long Claude Code task on your desktop? Open ZenTerm in bed, connect, and view the live tmux session in read-only mode to watch the AI work without accidentally sending keystrokes.
* **Native Touch Scroll in Tmux**: We translate your vertical swipe gestures directly into tmux `copy-mode` commands, allowing smooth scrolling even when tmux has hijacked the standard terminal scroll buffer.

## 🛠️ Developer Quality of Life

* **Quick CD \u0026 Bookmarks**: An inline toolbar to jump between directories. Long paths are cleanly truncated.
* **Pane Management**: Split panes horizontally or vertically (`Sp─`, `Sp|`), navigate between them, or kill panes directly from the touch toolbar.
* **Key Modifier Row**: Persistent row for `ESC`, `Tab`, `^Z`, `/`, and an `@` key (specifically exposed by setting the keyboard type to `emailAddress` for easy Claude file referencing).
* **TrueColor Support**: Full `xterm-256color` and `truecolor` rendering.

---

*ZenTerm is not trying to be a full Linux desktop replacement. It is a highly specialized weapon for lazy, efficient prompting.*
