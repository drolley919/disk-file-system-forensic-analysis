# Findings

This section summarizes the key forensic findings identified during analysis of the NTFS file system. Findings are derived from validated file system artifacts, registry analysis, and metadata correlation.

Each finding reflects observable evidence and supports conclusions regarding user activity and system usage.

---

## Finding 1: Verified User-Created Documents

Multiple user-created Rich Text Format (RTF) documents were identified within the NTFS file system, including **`Devin.rtf`** and **`Rolley.rtf`**.

These files:
- Were located within a user-accessible directory
- Contained user-generated content
- Displayed valid NTFS metadata attributes

The presence of these documents indicates legitimate file creation rather than system-generated artifacts or automated processes.

---

## Finding 2: Confirmed Application-Level File Access

Windows Registry analysis revealed entries within the **WordPad Recent File List**, confirming that **`Rolley.rtf`** was actively opened using WordPad.

This finding demonstrates:
- Application execution
- Intentional user interaction
- Active document access rather than passive file storage

Registry evidence corroborates file system findings and supports timeline reconstruction.

---

## Finding 3: Consistent NTFS Timestamp Correlation

The examined user-created files exhibited closely aligned:
- Creation timestamps
- Modification timestamps
- Access timestamps

Timestamp consistency across multiple artifacts suggests routine user activity conducted within a narrow time window. No anomalies indicative of timestamp manipulation or automated file generation were observed.

---

## Finding 4: File Integrity and Authenticity Validated

Cryptographic hash values were generated and reviewed for selected user-created files using industry-standard algorithms (MD5 and SHA-1).

Hash validation confirms:
- File integrity was preserved during analysis
- No modification occurred after acquisition
- Artifacts are suitable for independent verification

This supports the reliability of all associated findings.

---

## Finding 5: No Indicators of Malicious or Automated Activity

Analysis of file content, metadata attributes, registry artifacts, and timestamps revealed no indicators of:
- Malware execution
- Automated script-driven file creation
- Obfuscation or anti-forensic techniques

Observed activity aligns with normal user behavior on a Windows system.

---

## Summary of Findings

Collectively, the findings establish that:
- User-created documents existed within the NTFS file system
- Files were actively accessed through WordPad
- Registry and file system artifacts correlate consistently
- Evidence integrity was preserved throughout analysis

These findings support a defensible conclusion of legitimate user activity with no evidence of malicious behavior.
