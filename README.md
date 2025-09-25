# certs
Public repository for CloudTrack.Me Release Certificates (JSON &amp; PDF proofs of music releases)

# CloudTrack Release Certificates
[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)

This repository is the **public proof store** for all music releases on [CloudTrack.me](https://cloudtrack.me).

Each release on CloudTrack automatically generates a **Release Certificate** (in JSON and PDF format) that proves:
- The **authorship** of the creator
- The **timestamp** of upload and release
- The **file hash (SHA-256)** for integrity
- The **platform digital signature**
- The **GitHub commit record** for immutability

## 📂 Repository Structure
/certs
/2025
/09
track-<uuid>.json
track-<uuid>.pdf

- `track-<uuid>.json` → machine-readable certificate  
- `track-<uuid>.pdf` → human-readable certificate  

## 🔍 Verification
1. Visit the **public verify URL** embedded in each certificate: https://cloudtrack.me/verify/<certId>

2. Or manually check the JSON certificate against:  
- GitHub commit hash (this repo)  
- CloudTrack public key (for digital signature verification)  
- File SHA-256 hash  

## ✅ Trust Model
- Certificates are pushed automatically by CloudTrack workers.
- Each commit to this repository is immutable proof of existence (commit hash + timestamp).
- Future roadmap includes **Blockchain anchoring** for additional immutability.

## 📜 License
All certificates in this repository are released under [CC0 1.0 Universal](https://creativecommons.org/publicdomain/zero/1.0/).  
They are free to use for **verification and authenticity purposes**.

---

**CloudTrack – Safe Haven for Creators**  
Protecting music rights with transparency and global trust.
