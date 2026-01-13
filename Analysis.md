# Forensic Analysis

## File System Overview
The disk image was examined to identify the NTFS file system structure, including directories, user files, and system-generated artifacts.

### User File Artifact Examination

During file system analysis, user-created documents were reviewed to identify artifacts of forensic relevance. The file `Devin.rtf` was identified within a user directory and examined using FTK Imager.

The artifact contained user-generated content and displayed valid NTFS metadata, including created, modified, and accessed timestamps. File attributes and size information were consistent with a legitimate document created through normal user activity.

#### Supporting Evidence – User File Metadata and Content (FTK Imager)
![FTK user file metadata and content view](Assets/screenshots/ftk-user-file-metadata-devin-rtf.png)

### User Artifact Correlation and Timeline Consistency

Further examination of the user directory revealed multiple user-created Rich Text Format (RTF) files, including `Devin.rtf` and `Rolley.rtf`. These artifacts were located within the same directory and exhibited closely aligned creation and modification timestamps.

The proximity of timestamps and consistent NTFS metadata attributes suggest normal user activity rather than automated or malicious file creation. This correlation supports the conclusion that the files were generated during routine system use by the same user account.

#### Supporting Evidence – Multiple User File Correlation (FTK Imager)
![FTK multiple user file metadata correlation](Assets/screenshots/ftk-multiple-user-files-metadata-correlation.png)
