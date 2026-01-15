# Evidence Overview

This section documents the digital evidence examined during the forensic analysis and outlines the procedures used to preserve evidentiary integrity throughout the investigation.

All analysis was conducted using forensically sound methods in a controlled environment to ensure that original evidence remained unaltered.

---

## Evidence Description

The primary evidence consisted of a forensic disk image containing an NTFS file system. The image was analyzed in a read-only state to prevent modification of original data.

---

## Evidence Sources

| Evidence Type | Description |
|-------------|-------------|
| Disk Image | NTFS-formatted forensic disk image analyzed using FTK Imager |
| File Artifacts | User-created files and directories recovered from the file system |
| Metadata | NTFS timestamps, file attributes, and allocation data |

---

## Data Collection Methodology

FTK Imager was used to mount and examine the disk image in a read-only state. No write operations were performed on the evidence during analysis.

All findings were documented contemporaneously to maintain traceability and investigative accuracy.

---

## Cryptographic Hash Verification

Cryptographic hash values were used to verify the integrity of the forensic image and extracted artifacts.

Hash verification ensured that evidence remained unchanged during acquisition, examination, and reporting phases.

---

## Supporting Evidence – Hash File Import Validation

A CSV file containing MD5 and SHA-1 hash values was imported into a spreadsheet application to validate file integrity outside of the forensic tool.

Import settings, character encoding, and delimiters were reviewed to ensure accurate parsing of hash values and full NTFS file paths.

This step reduces the risk of data corruption or misinterpretation when validating evidence integrity externally.

![CSV hash import validation](Assets/screenshots/csv-hash-import-validation.png)

---

## Supporting Evidence – File Hash Verification (MD5 & SHA-1)

Cryptographic hash values were generated for selected user-created files and recorded alongside their full NTFS file paths.

This validation confirms that file contents remained unchanged during analysis and supports independent verification of findings.

![File hash verification](Assets/screenshots/file-hash-verification-md5-sha1-csv.png)

---

## Evidence Integrity Considerations

Evidence integrity was maintained by:
- Enforcing read-only access to the forensic image
- Verifying cryptographic hashes at multiple stages
- Documenting timestamps and file attributes
- Avoiding unnecessary system interaction

These controls ensure that all conclusions are based on verifiable, unaltered evidence.
