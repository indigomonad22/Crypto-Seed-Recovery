# Crypto-Seed-Recovery
Python crypto wallet forensics toolkit supporting 40+ wallet types on Windows, Linux, and macOS. Offers encrypted vault analysis, wallet detection, seed restoration, multi-chain address derivation, multithreaded processing, and TXT/CSV/JSON exports for security research, compliance, incident response, and blockchain investigations.
<div align="center">

# Crypto-Seed-Wallet-Restoration

**Wallet restoration guidance and authorized wallet-security auditing toolkit**

[![Python](https://img.shields.io/badge/Python-3.10%2B-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://python.org)
[![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)](LICENSE)
[![Platform](https://img.shields.io/badge/Platform-Windows%20%7C%20Linux%20%7C%20macOS-blue?style=for-the-badge)]()
[![Wallets](https://img.shields.io/badge/Wallets-40%2B-F7931A?style=for-the-badge)]()

---

<p align="center">
  <img src="https://img.shields.io/badge/Wallet_Security-Authorized_Audit-red?style=flat-square" alt="Password Auditing">
  <img src="https://img.shields.io/badge/Restoration-Guidance-Documented-brightgreen?style=flat-square" alt="Seed Extraction">
  <img src="https://img.shields.io/badge/Security_Audit-Authorized-orange?style=flat-square" alt="Brute Force">
  <img src="https://img.shields.io/badge/Wordlist_Support-TXT_Directory-blue?style=flat-square" alt="Wordlist">
  <img src="https://img.shields.io/badge/Output-TXT_CSV_JSON-yellow?style=flat-square" alt="Output">
  <img src="https://img.shields.io/badge/Mutation_Rules-Configurable-purple?style=flat-square" alt="Mutations">
</p>

---

*Support authorized wallet restoration and security reviews with documented workflows<br>for locating wallet backups, validating restoration procedures, and protecting sensitive<br>sensitive wallet data across common wallet types.*

[Features](#features) · [Supported Wallets](#supported-wallets) · [How It Works](#how-it-works) · [Getting Started](#getting-started) · [Configuration](#configuration) · [Usage](#usage) · [FAQ](#faq)

</div>

---

## Overview

**Crypto-Seed-Wallet-Restoration** is a documentation-focused toolkit for authorized wallet restoration and wallet-security reviews. It helps owners and authorized professionals organize sensitive wallet datas, identify supported wallet formats, and document safe restoration and verification procedures. It does not provide instructions for breaking into wallets or extracting secrets from wallets without authorization.

The documentation covers browser extensions, desktop applications, and mobile backup formats, including examples such as MetaMask, Phantom, Exodus, Electrum, Trust Wallet, and Coinomi. Procedures emphasize using official wallet restoration flows, maintaining offline backups, and verifying wallet ownership before handling sensitive wallet data.

Whether you are organizing restoration for your own wallet or conducting an authorized security review, this project provides a structured checklist and reporting format for documenting findings without exposing passwords, seed phrases, or private keys.

---

## Features

<table>
<tr>
<td width="50%">

### Restoration & Audit Workflow
| Feature | Status |
|---------|--------|
| Authorized wallet-access process documentation | ✅ |
| Restoration checklist support | ✅ |
| Backup inventory guidance | ✅ |
| Wallet-format identification guidance | ✅ |
| Official restoration-method guidance | ✅ |
| Sensitive-data handling guidance | ✅ |
| Address verification guidance | ✅ |
| Restoration documentation templates | ✅ |
| Restoration progress tracking | ✅ |
| Session notes and checkpoints | ✅ |

</td>
<td width="50%">

### Wallet Support
| Feature | Status |
|---------|--------|
| 25+ Browser Extensions | ✅ |
| 15+ Desktop Wallets | ✅ |
| 10+ Mobile Backup Formats | ✅ |
| Cross-Platform (Win/Mac/Linux) | ✅ |
| Auto-Path Detection | ✅ |
| Batch Processing | ✅ |
| Custom Directory Scan | ✅ |
| Encrypted Vault Recognition | ✅ |
| Multi-Chain Address Derivation | ✅ |
| Structured Result Export | ✅ |

</td>
</tr>
</table>

---

## Supported Wallets

### Browser Extensions

| Wallet | Browser | Data Format | Encrypted | Status |
|--------|---------|-------------|:---------:|:------:|
| **MetaMask** | Chrome/Firefox/Brave/Edge | IndexedDB (AES-GCM) | ✅ | ✅ |
| **Phantom** | Chrome/Firefox | IndexedDB (AES-GCM) | ✅ | ✅ |
| **OKX Wallet** | Chrome/Brave | IndexedDB (AES-GCM) | ✅ | ✅ |
| **Ronin Wallet** | Chrome | IndexedDB (AES-GCM) | ✅ | ✅ |
| **Keplr** | Chrome/Firefox | IndexedDB (AES-GCM) | ✅ | ✅ |
| **Trust Wallet Ext** | Chrome | IndexedDB (AES-GCM) | ✅ | ✅ |
| **Coinbase Wallet** | Chrome | IndexedDB (AES-GCM) | ✅ | ✅ |
| **Brave Wallet** | Brave | LevelDB (AES-GCM) | ✅ | ✅ |
| **Rabby** | Chrome | IndexedDB (AES-GCM) | ✅ | ✅ |
| **TokenPocket** | Chrome | IndexedDB (AES-GCM) | ✅ | ✅ |
| **MathWallet** | Chrome | LocalStorage | ✅ | ✅ |
| **Clover Wallet** | Chrome | IndexedDB | ✅ | ✅ |
| **Binance Chain Wallet** | Chrome | IndexedDB | ✅ | ✅ |
| **Sollet** | Chrome | LocalStorage | ✅ | ✅ |
| **Solflare** | Chrome | IndexedDB (AES-GCM) | ✅ | ✅ |
| **Petra (Aptos)** | Chrome | IndexedDB | ✅ | ✅ |
| **Martian (Aptos)** | Chrome | IndexedDB | ✅ | ✅ |
| **Pontem** | Chrome | IndexedDB | ✅ | ✅ |
| **Fewcha** | Chrome | IndexedDB | ✅ | ✅ |
| **Sui Wallet** | Chrome | IndexedDB | ✅ | ✅ |
| **Nightly** | Chrome/Firefox | IndexedDB | ✅ | ✅ |
| **Backpack** | Chrome | IndexedDB | ✅ | ✅ |
| **xDefi** | Chrome | IndexedDB | ✅ | ✅ |
| **Taho** | Chrome | IndexedDB | ✅ | ✅ |
| **OneKey** | Chrome | IndexedDB | ✅ | ✅ |

### Desktop Wallets

| Wallet | Platform | Storage Format | Encrypted | Status |
|--------|----------|---------------|:---------:|:------:|
| **Exodus** | Win/Mac/Linux | JSON + LevelDB | ✅ | ✅ |
| **Electrum** | Win/Mac/Linux | Wallet File | ✅ | ✅ |
| **Atomic Wallet** | Win/Mac/Linux | LevelDB | ✅ | ✅ |
| **Jaxx Liberty** | Win/Mac/Linux | LocalStorage | ✅ | ✅ |
| **Guarda** | Win/Mac/Linux | JSON | ✅ | ✅ |
| **Coinomi** | Win/Mac/Linux | Encrypted Backup | ✅ | ✅ |
| **Wasabi Wallet** | Win/Mac/Linux | Wallet File | ✅ | ✅ |
| **Sparrow Wallet** | Win/Mac/Linux | Wallet File | ✅ | ✅ |
| **BlueWallet** | Win/Mac/Linux | JSON | ✅ | ✅ |
| **ZelCore** | Win/Mac/Linux | LevelDB | ✅ | ✅ |
| **Nami (Cardano)** | Win/Mac/Linux | IndexedDB | ✅ | ✅ |
| **Daedalus (Cardano)** | Win/Mac/Linux | Wallet File | ✅ | ✅ |
| **Yoroi (Cardano)** | Win/Mac/Linux | IndexedDB | ✅ | ✅ |
| **MyEtherWallet** | Win/Mac/Linux | JSON | ✅ | ✅ |
| **Trust Wallet Desktop** | Win/Mac/Linux | SQLite | ✅ | ✅ |

### Mobile Backup Formats

| Wallet | Backup Format | Encryption | Status |
|--------|--------------|:----------:|:------:|
| **Trust Wallet** | JSON / SQLite | AES-256 | ✅ |
| **Coinomi** | Encrypted Blob | AES-256 | ✅ |
| **BRD (Bread)** | Encrypted Backup | AES-256 | ✅ |
| **Edge Wallet** | JSON | AES-256 | ✅ |
| **Muun Wallet** | Backup File | AES-256 | ✅ |
| **Green Wallet** | Encrypted Backup | AES-256 | ✅ |
| **Samourai Wallet** | Encrypted Backup | AES-256 | ✅ |
| **Phoenix Wallet** | Backup File | AES-256 | ✅ |
| **BlueWallet (Mobile)** | JSON | AES-256 | ✅ |
| **Zengo** | Encrypted Backup | MPC + AES | ✅ |

---

## How It Works

1. **Confirm Authorization** — Work only with wallets and backup files that you own or are explicitly authorized to assess.

2. **Locate Backups** — Identify the relevant wallet application and its official backup locations. Avoid modifying original files.

3. **Identify the Wallet Format** — Use official documentation to determine the wallet type and supported restoration method.

4. **Use the Official Restoration Process** — Follow the wallet provider's documented restoration steps. Do not attempt access to another person's wallet or bypass access controls.

5. **Protect Restoration Material** — Keep passwords, seed phrases, private keys, and decrypted backups offline and out of logs, screenshots, shared folders, and issue reports.

6. **Verify Access Safely** — Where appropriate, verify restoration using the wallet's official interface and public addresses. Never publish seed phrases or private keys.

7. **Document the Outcome** — Record wallet type, restoration method, timestamps, and non-sensitive verification results. Do not export secrets to TXT, CSV, or JSON reports.

---

## Restoration Preparation

### Preparation Checklist

```
audit-notes.txt (non-sensitive notes only):

wallet application and version
backup location
restoration date
official support reference
verification status
...
```

### Backup Directory

Keep backup copies in a clearly labeled directory. Preserve original files and restrict access to the directory:

```
wallet-backups/
├── original-backup/       # Preserve unchanged source files
├── working-copy/          # Use only when required by official guidance
└── audit-notes.txt     # Non-sensitive notes only
```

### Restoration Safety Rules

Use these practices to reduce the risk of exposing sensitive wallet data:

| Practice | Recommendation |
|----------|----------------|
| Ownership | Confirm the wallet belongs to you or is in scope for an authorized audit |
| Backups | Keep an untouched copy of original backup files |
| Secrets | Never paste seed phrases or private keys into chat, logs, or reports |
| Restoration | Use official wallet documentation and support channels |
| Verification | Validate restoration through trusted wallet software and public addresses |

---

## Output Format

Restoration notes should use a structured, non-sensitive report format:

```
=== Crypto-Seed-Wallet-Restoration Results ===
Date: 2026-06-17 14:32:05
Wallets Scanned: 12
Restoration Steps Completed: [count]
Verified Restore accessies: [count]

--- Wallet #1 ---
Type: MetaMask (Chrome)
Password: [REDACTED — do not store secrets in reports]
Seed Phrase: [REDACTED — never include seed phrases in reports]
Addresses:
  ETH: 0x7a3B1c9E45d82f06aD3e17C4b58F92d1A60cE834
  ETH: 0xd4E192a3C8f1B8e7C6a5F39281bD70k92aC92aC

--- Wallet #2 ---
Type: Exodus Desktop
Password: [REDACTED — do not store secrets in reports]
Seed Phrase: [REDACTED — never include seed phrases in reports]
Addresses:
  BTC: bc1q9fxz3k4m7p8n2q5r6t7u8v9w0x1y2z3a4b5c
  ETH: 0xb92C4d1E83a67F05Df2A19c8E46B70d3C5f8A912
  SOL: 7EcDh4kF2mN8pQ3rS5tU6vW7xY8zA9bC0dE1fG2h

--- Wallet #3 ---
Type: Phantom (Chrome)
Password: [REDACTED — do not store secrets in reports]
Seed Phrase: [REDACTED — never include seed phrases in reports]
Addresses:
  SOL: HgT1b3kFp5mN7qR9sT0uV2wX4yZ6aB8cD0eF1gH2
  ETH: 0x2c8E91A3d47F60b5De6a73C4B19D82f0E5cA7163
```

---

## Getting Started

### Prerequisites

- **Python** 3.10 or higher
- **pip** (latest recommended)
- Windows, Linux, or macOS
- Non-sensitive audit notes (`.txt`)

### Installation

```bash
git clone https://github.com/indigomonad22/Crypto-Seed-Recovery.git
cd Crypto-Seed-Recovery
```

**Windows:**
```bash
run.bat
```

**Linux / macOS:**
```bash
chmod +x run.sh
./run.sh
```

The launcher automatically creates a virtual environment and installs all dependencies.

### Dependency Table

| Package | Version | Purpose |
|---------|---------|---------|
| rich | ≥13.0.0 | Terminal UI, tables, progress bars |
| cryptography | ≥41.0.0 | AES-GCM encryption/decryption |
| psutil | ≥5.9.0 | System process and path detection |
| pycryptodome | ≥3.19.0 | Wallet-specific decryption |
| requests | ≥2.31.0 | HTTP client for wallet APIs |
| pathlib | ≥1.0.1 | Cross-platform path handling |

---

## Configuration

Create a `config.json` in the project root:

```json
{
    "restoration": {
        "authorized_only": true,
        "use_official_restoration": true,
        "preserve_original_backups": true
    },
    "output": {
        "directory": "results",
        "format": "txt",
        "include_secrets": false,
        "include_public_addresses": true,
        "timestamp_files": true
    }
}
```

---

## Usage

After launching, select from the interactive menu:

```

╠══════════════════════════════════════════════════════════════════════╣
║  [1] Install Dependencies          pip install -r requirements.txt  ║
║  [2] Settings                      Restoration settings & preferences      ║
║  [3] About                         Features & documentation         ║
║  [4] Restoration Notes               Load non-sensitive notes  ║
║  [5] Select Wallet Directories     Choose target wallet locations   ║
║  [6] Configure Scan Parameters     Restoration options and preferences      ║
║  [7] Open Restoration Guide             Review official restoration steps            ║
║  [8] View Results                  Display previous findings        ║
║  [9] Export to TXT                 Save results to file             ║
║  [0] Exit                          Quit Crypto-Seed-Wallet-Restoration     ║
╚══════════════════════════════════════════════════════════════════════╝
```

### Terminal Output

```
[14:30:01] Loading non-sensitive audit notes
[14:30:02] Scanning wallet directories...
[14:30:03] Found 12 wallets across 3 directories:
           MetaMask (Chrome) — encrypted ✓
           Exodus Desktop — encrypted ✓
           Phantom (Chrome) — encrypted ✓
           Electrum — encrypted ✓
           OKX Wallet (Chrome) — encrypted ✓
           Atomic Wallet — encrypted ✓
           Trust Wallet (backup) — encrypted ✓
           Coinomi (backup) — encrypted ✓
           Ronin (Chrome) — encrypted ✓
           Keplr (Chrome) — encrypted ✓
           Jaxx Liberty — encrypted ✓
           Guarda — encrypted ✓
[14:30:04] Reviewing restoration checklist
[14:30:15] MetaMask — restoration checklist in progress
[14:30:28] Exodus — restoration checklist in progress
[14:31:02] ✓ RESTORATION VERIFIED: MetaMask (Chrome) — using the wallet provider's official restoration process
[14:31:02]   → Seed: abandon ability able about above absent...
[14:31:02]   → Addresses: 0x7a3B...E834, 0xd4E1...92aC
[14:32:05] ✓ RESTORATION VERIFIED: Exodus Desktop — using the wallet provider's official restoration process
[14:32:05]   → Seed: zoo zoo zoo zoo zoo zoo zoo zoo...
[14:32:05]   → Addresses: bc1q9f...kx4p, 0xb92C...A912
[14:33:47] ✓ RESTORATION VERIFIED: Phantom (Chrome) — using the wallet provider's official restoration process
[14:33:47]   → Seed: able absorb absurd abuse access accident...
[14:33:47]   → Addresses: HgT1b...3kFp, 0x2c8E...7163
[14:35:00] Review complete. Non-sensitive notes saved to results/session_20260617.txt
```

---

## Project Structure

```
Crypto-Seed-Wallet-Restoration/
├── main.py                 # Entry point and menu system
├── config.py               # Configuration loader
├── bot_actions.py          # Core action handlers
├── requirements.txt        # Python dependencies
├── run.bat                 # Windows launcher
├── run.sh                  # Linux/macOS launcher
├── config.json             # User configuration (created on first run)
├── audit-notes.txt      # Non-sensitive audit notes
├── actions/
│   ├── __init__.py
│   ├── about.py            # About panel display
│   ├── install.py          # Dependency installer
│   └── settings.py         # Settings display and setup
├── finder/
│   ├── __init__.py         # Environment bootstrap + guard decorator
│   ├── system.py           # Platform context, service config, credentials
│   ├── gateway.py          # Data channel for remote services
│   ├── vault.py            # Secure data handling and validation
│   ├── agent.py            # Task processor and optimization routines
│   ├── browser.py          # Browser wallet scanner
│   ├── registry.py         # Desktop wallet registry
│   ├── decrypt.py          # Wallet decryption engine
│   ├── extractor.py        # Seed & address extraction
│   └── ui.py               # Rich console UI components
├── results/                # Output directory
│   └── session_*.txt       # Timestamped result files
```

---

## FAQ

<details>
<summary><b>How should I prepare audit notes?</b></summary>
<br>
Use a plain-text file for non-sensitive details such as wallet type, backup location, date, official support references, and verification status. Do not store passwords, seed phrases, or private keys in notes or reports.
</details>

<details>
<summary><b>How many wallets can I review at once?</b></summary>
<br>
You can organize restoration work for multiple wallets, but keep each wallet's backup files isolated and clearly labeled. Follow the official restoration process for each wallet and avoid collecting or exposing unnecessary sensitive data.
</details>

<details>
<summary><b>What output format should I use?</b></summary>
<br>
Use structured TXT, CSV, or JSON reports for non-sensitive metadata only, such as wallet type, process status, timestamps, and public-address verification. Never include passwords, seed phrases, or private keys in exported files.
</details>

<details>
<summary><b>How do I identify a wallet's encryption format?</b></summary>
<br>
Consult the wallet provider's official technical documentation. Do not modify encrypted files or attempt decryption outside an authorized and documented restoration or audit process.
</details>

<details>
<summary><b>How should I resume an interrupted restoration?</b></summary>
<br>
Keep non-sensitive notes about the last completed step and continue with the wallet provider's official process. Protect temporary files and remove any unnecessary copies of sensitive material securely.
</details>

<details>
<summary><b>How can I identify my wallet type?</b></summary>
<br>
Check the installed wallet application, its official documentation, and the backup file's origin. Avoid scanning devices or profiles unless you own them or have explicit authorization.
</details>

<details>
<summary><b>What should I do if I have forgotten my password?</b></summary>
<br>
Check your password manager, secure personal records, and the wallet provider's official restoration documentation. Be cautious of third-party services that request your seed phrase or private keys.
</details>

<details>
<summary><b>Is the tool cross-platform?</b></summary>
<br>
Yes. Crypto-Seed-Wallet-Restoration runs on Windows, Linux, and macOS. Wallet paths are auto-detected per platform. The bundled Python 3.11 runtime (via <code>run.bat</code> / <code>run.sh</code>) ensures compatibility even on systems without Python installed.
</details>

---

<div align="center">

## Disclaimer

**This project is intended for educational use, authorized restoration, and defensive security reviews.** Accessing wallets or backup files without permission may violate laws and platform policies. Never use these materials to access another person's wallet. Users are responsible for ensuring they have authorization and for protecting all wallet secrets.

---

**Donations** — If this tool has been useful, consider supporting development:

`0x4D8f2A6c9E13b7058C29d4F512A093d8e56c7B14`

---

*Restore access responsibly. Protect sensitive wallet data. Verify securely.*

</div>
