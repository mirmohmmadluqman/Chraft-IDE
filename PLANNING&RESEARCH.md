# 📋 Chraft IDE — Planning & Research

---

## 🔰 1. Project Vision

**Goal:**  
Create a **browser-based smart contract IDE**, later we will create **downloadable(application) smart contract IDE** that combines the simplicity of **Remix** with the advanced testing and deployment features of **Foundry and Hardhat** all without using the terminal.

---

## ⚙️ 2. Core Features (MVP)

| Feature         | Description                                                  |
|----------------|--------------------------------------------------------------|
| Solidity Editor | Monaco-based editor with syntax highlighting, autocomplete  |
| Run Tests       | Button to run `forge test` and show test results in UI       |
| Fuzz Testing    | Toggle to enable `forge test --fuzz`                         |
| Gas Reports     | Visual display of `forge test --gas-report`                 |
| Deploy Scripts  | Click-to-deploy smart contracts with inputs                 |
| Fork Mainnet    | Enable mainnet fork with RPC input using `anvil`            |
| Logs & Traces   | Visual output panel for console logs and trace reports      |
| File Manager    | File explorer panel similar to Remix                         |
| User Auth       | Firebase or GitHub login system                              |

---

## 🧪 3. Optional Advanced Features

| Feature          | Benefit                                                     |
|------------------|-------------------------------------------------------------|
| AI Assistant      | GPT-powered test suggestions, debug explainers             |
| Auto Save & Sync  | Save code to Firebase / IndexedDB                          |
| GitHub Sync       | Import/export projects from GitHub                         |
| Live Collaboration| Multi-user real-time editing                               |
| Solidity Linter   | Show warnings using `solhint` or `solc`                    |
| Plugin System     | Add security tools like Slither, MythX, or Certora         |

---

## 🛠️ 4. Tech Stack

| Layer            | Technology                                                  |
|------------------|-------------------------------------------------------------|
| **Frontend**     | React + Vite (or SvelteKit), TailwindCSS, Monaco Editor     |
| **Backend**      | Node.js (or Rust) as wrapper for Foundry CLI                |
| **Smart Contract Engine** | Foundry (`forge`, `anvil`, `cast`)                  |
| **Hosting**      | Vercel / Netlify                                            |
| **Auth & DB**    | Firebase (Authentication + Firestore)                       |
| **Optional**     | GPT API, Docker (for CLI isolation)                         |

---

## 📁 5. Suggested Folder Structure

chraft-ide/
├── frontend/
│ ├── components/
│ ├── pages/
│ └── utils/
├── backend/
│ ├── routes/
│ └── forge-wrapper.js
├── editor/ # Monaco + file system
├── scripts/ # Deploy scripts
├── test/ # Contract test files
├── public/
├── README.md
└── package.json

### It will be changed if required


---

## 🔍 6. Competitor Research

| Tool        | Strengths                                 | Weaknesses                                                      |
|-------------|-------------------------------------------|-----------------------------------------------------------------|
| **Remix**   | In-browser, easy to use                   | No automated testing, no fuzzing                                |
| **Foundry** | Fast, fuzzing, gas reports, CLI powerful  | No GUI, hard for beginners, time consuming                      |
| **Hardhat** | Flexible, plugin ecosystem                | Needs setup, not browser-based, much harder, more time consuming|
| **ChainIDE**| Web IDE for Solidity                      | Limited features, not fully open-source                         |

---

## ✅ Summary

Chraft IDE aims to provide a full dev + audit environment in the browser.  
Simple like Remix, powerful like Foundry.

Test, fuzz, deploy, and audit — with just one click.

---
