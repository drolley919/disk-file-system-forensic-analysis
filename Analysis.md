# Forensic Analysis

This section documents the analytical process used to examine the NTFS file system and interpret recovered artifacts. The analysis focuses on identifying evidence of user activity, validating file interactions, and correlating artifacts to establish a coherent investigative narrative.

---

## File System Overview

The disk image was examined to identify the NTFS file system structure, including system directories, user-created files, and system-generated artifacts.

Analysis focused on:
- User directories
- File metadata and timestamps
- NTFS allocation status
- System and application artifacts relevant to user interaction

---

## Registry Artifact Analysis – Recent File Activity

Windows Registry artifacts were examined to determine whether recovered documents had been actively accessed by a user.

The **WordPad Recent File List** registry key was reviewed to identify evidence of application-level interaction with recovered files.

The presence of user-created Rich Text Format (RTF) documents within this registry key indicates intentional file access rather than passive file existence.

---

## Supporting Evidence – WordPad Recent File Registry Entry

The following registry artifact confirms that the file **`Rolley.rtf`** was opened using WordPad.

This finding supports:
- Verified application execution
- Direct user interaction with the document
- Correlation between file system artifacts and registry activity

![WordPad Recent File Registry Artifact](Assets/screenshots/wordpad-recent-file-registry.png)

---

## User File Artifact Examination

User-created documents were reviewed to identify artifacts of forensic relevance.

The file **`Devin.rtf`** was identified within the user directory and examined using FTK Imager. The file contained user-generated content and displayed valid NTFS metadata, including creation, modification, and access timestamps.

File attributes and size information were consistent with a legitimate document created through normal user activity.

---

## Supporting Evidence – User File Metadata and Content

The following screenshot documents the file metadata and content view for **`Devin.rtf`**, demonstrating:
- Valid NTFS timestamps
- User-generated document content
- Consistency with expected file system behavior

![FTK user file metadata and content](Assets/screenshots/ftk-user-file-metadata-devin-rtf.png)

---

## User Artifact Correlation and Timeline Consistency

Further examination of the user directory revealed multiple user-created RTF files, including **`Devin.rtf`** and **`Rolley.rtf`**.

These files:
- Resided within the same directory
- Exhibited closely aligned creation and modification timestamps
- Displayed consistent NTFS metadata attributes

This correlation supports the conclusion that the files were generated during routine system use by the same user account rather than through automated processes or malicious activity.

---

## Supporting Evidence – Multiple User File Correlation

The following screenshot illustrates the correlation of multiple user-created documents and their associated metadata within FTK Imager.

![FTK multiple user file metadata correlation](Assets/screenshots/ftk-multiple-user-files-metadata-correlation.png)

---

## Analytical Conclusion

The combined file system, registry, and metadata analysis supports the conclusion that:
- User-created documents were actively accessed and modified
- Application-level interaction occurred through WordPad
- File timestamps and registry artifacts align consistently
- No indicators of automated or malicious file creation were identified

These findings establish a clear pattern of legitimate user activity within the examined NTFS file system.
