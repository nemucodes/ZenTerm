# Privacy Policy — ZenTerm

**Last updated: March 17, 2026**
**Developer: nemucodes**
**Contact: nemucodes@gmail.com**

---

## Overview

ZenTerm is an SSH terminal application for Android designed for developers.
We are committed to protecting your privacy. This policy explains what data ZenTerm collects, how it is stored, and what is shared with third parties.

**The short version: ZenTerm collects no personal data and sends nothing to our servers. Ever.**

---

## 1. Data Collected and Storage

### SSH Credentials

ZenTerm stores SSH connection credentials (hostnames, usernames, passwords, and private keys) that you enter manually.

- All credentials are encrypted and stored exclusively on your device using **Android Keystore** (hardware-backed secure storage).
- Credentials are **never transmitted** to nemucodes or any third-party server.
- Credentials are **never stored in plaintext**.

### Connection Metadata

Non-sensitive connection profile information (hostname, port, username, connection timeout settings) is stored locally in Android SharedPreferences.

### Settings and Bookmarks

App settings (font size, volume key configuration, toolbar customization, cd bookmarks) are stored locally on your device only.

---

## 2. Data We Do NOT Collect

ZenTerm does **not** collect, transmit, or store any of the following:

- Personal identification information
- Device identifiers or advertising IDs
- Location data
- Usage analytics or telemetry
- Crash reports sent to external services
- Terminal session content or command history
- SFTP file contents or directory listings
- Any data from your SSH sessions

---

## 3. Network Access

ZenTerm makes network connections **only** to the SSH servers that you explicitly configure in the app. The app does not contact nemucodes servers or any third-party analytics, advertising, or tracking services.

---

## 4. Third-Party Libraries

ZenTerm uses the following open-source libraries, none of which collect personal data:

| Library | Purpose |
|---------|---------|
| dartssh2 | SSH and SFTP protocol implementation (pure Dart — no native binary) |
| xterm.dart | Terminal emulation |
| flutter_secure_storage | Android Keystore integration |
| flutter_highlight | Syntax highlighting for file preview |
| flutter_markdown | Markdown rendering for file preview |
| Provider | State management |

---

## 5. Permissions

| Permission | Reason |
|-----------|--------|
| `INTERNET` | Required to establish SSH connections to your servers |

No other permissions are requested. ZenTerm does not access your contacts, storage, location, camera, or microphone.

---

## 6. Children's Privacy

ZenTerm is a developer tool intended for adults. We do not knowingly collect any information from children under the age of 13.

---

## 7. Data Deletion

Since all data is stored locally on your device, you can delete all app data at any time by:

- Clearing app data via Android Settings → Apps → ZenTerm → Clear Data
- Uninstalling the app

No data exists on our servers, so no additional deletion request is necessary.

---

## 8. Changes to This Policy

We may update this Privacy Policy from time to time. Any changes will be reflected by updating the "Last updated" date at the top of this page. Continued use of ZenTerm after changes constitutes acceptance of the updated policy.

---

## 9. Contact

If you have any questions about this Privacy Policy, please contact:

**nemucodes**
Email: nemucodes@gmail.com
GitHub: https://github.com/nemucodes/ZenTerm

---

*This privacy policy applies to ZenTerm for Android published on Google Play by nemucodes.*
