# Privacy Policy for ZenTerm

**Last updated: March 6, 2026**

ZenTerm ("the App") is an Android SSH client developed by Nemu ("the Developer"). This Privacy Policy explains our practices regarding the collection, use, and disclosure of information when you use our App.

## 1. Data Collection and Usage (Zero Telemetry)
**ZenTerm does NOT collect, store, or transmit any personal data, analytics, crash logs, or usage statistics to the Developer or any third-party servers.** 

We believe your terminal sessions and coding habits are your own business.

## 2. Local Storage and Encryption
To function as an SSH client, ZenTerm stores necessary connection details locally on your device:
*   **SSH Credentials:** Passwords, private keys (e.g., ED25519, RSA), hostnames, and usernames.
*   These details are securely encrypted using Android's native Keystore system (`EncryptedSharedPreferences`).
*   This data **never** leaves your device, except when actively establishing an SSH connection to the server you explicitly configure.

## 3. Network Access
The App requires network permissions (`INTERNET`) solely to establish SSH connections to the servers you specify. It does not communicate with any other servers or tracking services.

## 4. Changes to This Privacy Policy
We may update our Privacy Policy from time to time. We will notify you of any changes by posting the new Privacy Policy on this page and updating the "Last updated" date at the top.

## 5. Contact Us
If you have any questions or suggestions about our Privacy Policy, do not hesitate to contact us by creating an Issue on our GitHub repository or contacting us at: `nemucodes@gmail.com`
