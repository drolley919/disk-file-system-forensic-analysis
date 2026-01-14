# Forensic Findings

## Summary of Findings

The forensic examination of the NTFS disk image identified multiple user-created files and supporting system artifacts indicating normal user activity within the examined environment. Analysis focused on file system structure, registry artifacts, file metadata, and cryptographic hash validation to determine whether recovered files had been intentionally accessed or modified.

No indicators of malware execution, unauthorized persistence mechanisms, or anomalous system behavior were identified during the investigation.

---

## User File Activity Findings

Multiple Rich Text Format (RTF) files, including `Devin.rtf` and `Rolley.rtf`, were identified within the user desktop directory. These files contained user-generated content and exhibited valid NTFS metadata, including created, modified, and accessed timestamps consistent with routine user document creation and interaction.

The presence of readable content, appropriate file size, and intact metadata supports the conclusion that these files were created and maintained through standard user actions rather than automated or malicious processes.

---

## Registry Artifact Findings

Windows Registry analysis revealed entries within the WordPad `Recent File List` indicating that the file `Rolley.rtf` had been opened using the WordPad application. This artifact confirms application-level interaction and demonstrates that the file was actively accessed by the user rather than passively stored on the system.

Registry timestamps were consistent with file metadata timestamps, further reinforcing the conclusion of intentional user interaction during the examined timeframe.

---

## File Metadata and Timeline Consistency

File system analysis identified consistent NTFS timestamp values across multiple user-created files within the same directory. The proximity of creation and modification timestamps among related artifacts suggests normal workflow behavior, such as file creation, editing, and saving during a single user session.

No evidence of timestamp manipulation, anti-forensic activity, or anomalous file attribute behavior was observed.

---

## Cryptographic Hash Verification Findings

Cryptographic hash values (MD5 and SHA-1) were generated for selected user-created files to support evidence integrity verification. Hash values were successfully exported, validated, and documented using external tools without alteration to the original evidence.

The consistency of hash values confirms that file contents remained unchanged throughout the analysis process, supporting the integrity and reliability of the forensic findings.

---

## Absence of Malicious Indicators

Throughout the examination, no indicators of compromise were identified. Specifically:

- No suspicious executables or scripts were observed
- No anomalous registry persistence mechanisms were detected
- No evidence of automated or unauthorized file creation was found

Observed artifacts align with expected system and user behavior within a standard Windows operating environment.

No integrity issues were identified; forensic image hash verification confirmed the evidence remained unchanged throughout analysis.

An executable file was identified within the NTFS root directory using a non-standard filename and no file extension. Hex analysis confirmed the presence of a Windows PE header (`MZ`), indicating intentional obfuscation of executable content.

Cryptographic hash validation confirmed the integrity of multiple files identified within the NTFS partition using both MD5 and SHA1 algorithms.

Low-level NTFS analysis identified files with system-generated names that contained valid metadata, consistent timestamps, and structured binary content, indicating legitimate file system artifacts rather than corruption or random data.

NTFS ownership analysis identified a specific user account associated with files located in the SECRET partition. Owner SID correlation linked the artifact to a documented user and workstation, enabling reliable user attribution.

---
## Conclusion

Based on file system analysis, registry artifact examination, metadata correlation, and cryptographic verification, the recovered artifacts reflect legitimate user-generated document activity. The findings support the conclusion that the examined files were intentionally created and accessed by the user and do not indicate malicious activity or system compromise.

These findings are consistent with normal system usage and demonstrate proper evidence handling, artifact interpretation, and forensic analysis methodology.
