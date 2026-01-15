# Disk & File System Forensic Analysis (NTFS)

## Overview
This project demonstrates hands-on disk and NTFS file system forensic analysis performed using a forensic disk image. The investigation focused on identifying user activity, validating evidence integrity, and correlating file system artifacts to reconstruct system usage.

The analysis was conducted in a controlled forensic environment using industry-standard tools and methodologies aligned with real-world DFIR workflows.

---

## Tools & Techniques
- FTK Imager (disk image analysis, metadata review)
- Windows Registry analysis
- NTFS artifact examination ($MFT, timestamps, file attributes)
- Cryptographic hash verification (MD5, SHA-1)
- CSV-based hash validation and external verification

---

## Investigation Scope
- NTFS file system structure analysis
- User-created document identification
- Registry-based evidence of file execution
- File metadata and timestamp correlation
- Integrity verification of forensic evidence

---

## Key Findings
- Identified multiple user-created RTF documents within the NTFS volume
- Confirmed file access through application-level artifacts (WordPad registry keys)
- Validated file authenticity and integrity using cryptographic hashes
- Correlated file creation, modification, and access timestamps to normal user activity

Detailed findings and supporting evidence are documented in the sections below.

---

## Repository Structure
- **Executive-Summary.md** – High-level investigative summary
- **Evidence.md** – Evidence handling, sources, and integrity verification
- **Analysis.md** – Technical forensic analysis and artifact examination
- **Findings.md** – Interpreted results and conclusions
- **Recommendations.md** – Security and forensic best-practice recommendations
- **Assets/screenshots/** – Supporting forensic screenshots referenced throughout

---

## Analyst Focus
This project reflects applied digital forensics skills relevant to:
- SOC Analyst (Tier 1–2)
- Junior DFIR / Incident Response roles
- Entry-level Digital Forensics Analyst positions
