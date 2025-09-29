# 🔐 CipherGuard — Secure Browser Password Manager

**CipherGuard** is a secure browser extension that manages and protects your login credentials **locally**.  
All encryption happens **within your browser** — even if your local storage is compromised, attackers only see encrypted data.

---

## ✨ Features

- Master Password Protection – Unlock your vault with a single master password  
- Auto & Manual Lock – Vault automatically locks after inactivity; manually lock anytime  
- Credential Management – Add, edit, delete, search, and copy credentials  
- Autofill Support – Automatically fill login forms on saved websites  
- Context Menu Integration – Right-click in username/password fields to fill credentials  
- Password Generation – Generate strong random passwords with customizable length, symbols, and numbers  

---

## 🛡️ Tech Stack & Security

| Component         | Details                                                                 |
|-------------------|-------------------------------------------------------------------------|
| **Frontend**      | Browser extension UI (popup, options page, content scripts)             |
| **Background**    | Service Worker handles encryption, vault state, and extension events    |
| **Storage**       | Encrypted vault stored locally using IndexedDB                          |
| **Encryption**    | AES-256-GCM for confidentiality and integrity                           |
| **Key Derivation**| PBKDF2 stretches master password into a cryptographic key               |
| **Password Gen**  | Uses `crypto.getRandomValues()` for secure randomness                   |

🔒 **All sensitive data is stored locally — nothing is sent to external servers.**

---

## 🚀 Installation

### 1. Clone or Download Repo
```bash
git clone https://github.com/Cyber-Security-July-Dec-2025/B3.git
```

## ⚡Load Extension
### Google Chrome
1. Open `chrome://extensions`
2. Enable **Developer mode**
3. Click **Load unpacked** → select the `extension/` folder
---
## 📌 Pin the Extension

1. Click the **puzzle icon** in the toolbar  
2. Pin **CipherGuard** for quick access  
---
## 🔑 Usage

- Unlock the vault with your **master password**  
- Add new credentials (Website, Username, Password)  
- Generate **strong passwords** instantly  
- Search credentials by site or username  
- Use the **lock button** to secure vault instantly  
- Visit a saved website → fields are **autofilled** 
---
## 📂 Project Structure

- README.md
- extension/
  - background.js
  - content.js
  - manifest.json
  - options.css
  - options.html
  - options.js
  - popup.css
  - popup.html
  - popup.js
- assets/
  - icon.svg
- scripts/
  - crypto.js
  - generator.js
  - storage.js



---
## 🔒 Security Highlights

- **Local-Only Encryption** → Everything stays on your device  
- **AES-256-GCM** → Ensures confidentiality & integrity  
- **PBKDF2 Key Derivation** → Strengthens your master password  
- **Auto & Manual Locking** → Prevents unauthorized access  
---
## 📸 Screenshots

### Unlock Vault
<img width="520" height="315" alt="image" src="https://github.com/user-attachments/assets/3d6e3fd6-8048-4606-b5e0-3e9ff137e90f" />


### Search Credentials
<img width="532" height="362" alt="image" src="https://github.com/user-attachments/assets/77028afb-3c75-48c4-b4bc-e3f0a684730b" />


### Autofill
<img width="774" height="702" alt="Screenshot 2025-09-30 000408" src="https://github.com/user-attachments/assets/ed28f155-e65d-468d-8c19-c68176843ca8" />


### Generate Password
<img width="503" height="120" alt="image" src="https://github.com/user-attachments/assets/df7787bf-5397-4aa0-ac9c-b5a5661e2dec" />


### Lock Vault
<img width="524" height="480" alt="image" src="https://github.com/user-attachments/assets/7bc53960-2eb9-463b-bef5-c3697106310b" />
### Options
<img width="1906" height="804" alt="Screenshot 2025-09-30 024755" src="https://github.com/user-attachments/assets/abcd8753-2136-4ecb-bfa3-433477ce4375" />

---
## 📄 License

This project is **MIT licensed** — see the `LICENSE` file for details.


