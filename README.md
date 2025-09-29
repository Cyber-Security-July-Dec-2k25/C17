# CipherGuard — Secure Browser Password Manager

![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg) ![Language](https://img.shields.io/badge/Language-JavaScript-F7DF1E.svg) ![Platform](https://img.shields.io/badge/Platform-Chrome%20%7C%20Edge-blue.svg)

**CipherGuard** is a secure browser extension that manages and protects your login credentials locally. All encryption happens within your browser — even if your local storage is compromised, attackers only see encrypted data.

---

## 🚀 Features

-   **Master Password Protection**: Unlock your vault with a single master password.
-   **Auto & Manual Lock**: Vault automatically locks after inactivity; manually lock anytime.
-   **Credential Management**: Add, edit, delete, search, and copy credentials.
-   **Autofill Support**: Automatically fill login forms on saved websites.
-   **Context Menu Integration**: Right-click in username/password fields to fill credentials.
-   **Password Generation**: Generate strong random passwords with customizable length, symbols, and numbers.
-   **Save Prompt**: Detect new logins and prompt to save credentials.

---

## 🛠️ Tech Stack & Security

-   **Frontend**: Browser extension UI (popup, options page, content scripts)
-   **Background / Service Worker**: Handles encryption, vault state, and extension events
-   **Storage**: Encrypted vault stored locally using IndexedDB
-   **Encryption**: `AES-256-GCM` for confidentiality and integrity
-   **Key Derivation**: `PBKDF2` stretches master password into a cryptographic key
-   **Password Generation**: Uses `crypto.getRandomValues()` for secure randomness

✅ **All sensitive data is stored locally — nothing is sent to external servers.**

---

## 📦 Installation

### Clone or Download Repo

```bash
git clone [https://github.com/Cyber-Security-July-Dec-2025/B3.git](https://github.com/Cyber-Security-July-Dec-2025/B3.git)
Or download the ZIP → extract → open the cipherguard/ folder.

Load Extension
Google Chrome

Open chrome://extensions

Enable Developer mode

Click Load unpacked → select the extension folder

Microsoft Edge

Open edge://extensions

Enable Developer mode

Click Load unpacked → select the extension folder

Pin the Extension
Click the puzzle icon in the toolbar → pin CipherGuard.

🔑 Usage
Unlock the vault with your master password.

Add new credentials (Website, Username, Password).

Generate strong passwords as needed.

Search for stored credentials by site or username.

Use the lock button to secure the vault instantly.

Visit a website with saved credentials → fields are autofilled.

New login detected → prompted to save credentials.

📂 Project Structure
.
├── README.md
└── extension/
    ├── background.js
    ├── content.js
    ├── manifest.json
    ├── options.css
    ├── options.html
    ├── options.js
    ├── popup.css
    ├── popup.html
    ├── popup.js
    ├── assets/
    │   └── icon.svg
    ├── scripts/
    │   ├── crypto.js
    │   ├── generator.js
    │   └── storage.js
    └── snapshots/
        ├── autofill.png
        ├── confirm.png
        ├── generate.png
        ├── homepage.png
        ├── lock.png
        ├── master.png
        ├── password.png
        ├── rightclick.png
        └── search.png
🔒 Security Highlights
Local-Only Encryption: Everything stays on your device.

AES-256-GCM: Protects both the confidentiality and integrity of your data.

PBKDF2 Key Derivation: Strengthens your master password against brute-force attacks.

Auto & Manual Locking: Prevents unauthorized access when you're away from your computer.

📸 Screenshots
Unlock Vault	Search Credentials	Autofill
Generate Password	Confirm Save	Lock Vault

Export to Sheets
🤝 Contributing
Contributions are welcome! 🎉

Follow the existing folder structure.

Write clear and descriptive commit messages.

Keep sensitive data out of the repository.

Submit an issue or pull request anytime.

📄 License
This project is licensed under the MIT License — see the LICENSE file for details.
