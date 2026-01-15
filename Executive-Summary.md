# Executive Summary

This investigation involved forensic analysis of an NTFS-formatted disk image to identify user activity, validate evidence integrity, and assess file system artifacts relevant to potential investigative scenarios.

Using industry-standard forensic tools and established DFIR methodologies, the analysis focused on examining file system structures, user-created documents, application artifacts, and cryptographic hash verification to ensure evidentiary accuracy.

The investigation identified multiple user-generated Rich Text Format (RTF) files stored within user-accessible directories. Registry artifacts associated with the WordPad application confirmed that at least one document was actively opened by the user, indicating intentional interaction rather than passive file presence.

File metadata analysis demonstrated consistent NTFS timestamps for file creation, modification, and access, supporting a timeline of normal user activity. Cryptographic hash verification (MD5 and SHA-1) confirmed the integrity of the forensic image and extracted artifacts, ensuring that no evidence alteration occurred during analysis.

Overall, the findings demonstrate a clear, defensible methodology for validating user activity and file authenticity within a Windows NTFS environment. This investigation reflects practical digital forensics skills applicable to incident response, endpoint investigations, and entry-level DFIR operations.
