# Data and Password Recovery Procedures

This document outlines practical steps for data and password recovery in various scenarios. It covers retrieving files, recovering passwords, and conducting forensic analyses.

#### 1. Retrieving SAM and SYSTEM Files from an Offline Windows OS

To retrieve SAM and SYSTEM files from an offline Windows OS, follow these steps:

- Boot the system using a live USB or CD.
- Navigate to the system's Windows directory (usually C:\Windows).
- Locate and copy the SAM and SYSTEM files to an external storage device.

## 2. Recovering a Windows Logon Password (Cracking the SAM Hash)

**Disclaimer: Password cracking should only be performed legally and ethically.**

1. Acquire the SAM file from the target Windows system.
2. Use a password-cracking tool such as John the Ripper or Hashcat to crack the hashed passwords.

## 3. Recovering Data from an Android/Windows Device

### Android Device:

1. Connect the device to a computer.
2. Use data recovery software like Dr.Fone or Disk Drill to recover lost data.

### Windows Device:

1. Utilize file recovery tools like Recuva or PhotoRec.
2. Connect the storage device to another computer for recovery.

## 4. Recovering Deleted Data from HDD, Flash Disk

1. Stop using the storage device immediately to prevent overwriting.
2. Use file recovery tools to scan for and recover deleted files.

## 5. Creating Forensic Images of Different Storage Media

1. Use forensic imaging tools like dd or FTK Imager.
2. Create a bit-by-bit copy of the storage media for analysis.


# 6. Using Autopsy, FTK, etc., for Forensic Analyses

## a. File Recovery Analysis:

**Purpose:** Identify and recover deleted or hidden files from the forensic image.

**Procedure:**
- Use the file recovery feature in the chosen forensic tool.
- Examine recovered files for relevance to the investigation.

## b. Timeline Analysis:

**Purpose:** Create a chronological timeline of events based on system activities.

**Procedure:**
- Analyze system logs and timestamps.
- Use the timeline analysis feature in the forensic tool.
- Identify key events and their sequence.

## c. Keyword Search and Indexing:

**Purpose:** Locate specific terms or keywords within the forensic image.

**Procedure:**
- Perform a keyword search using the forensic tool.
- Review search results for relevant information.

## d. Registry Analysis:

**Purpose:** Examine Windows registry entries for system configuration and user activities.

**Procedure:**
- Access the registry analysis module in the forensic tool.
- Investigate registry keys related to user accounts, installed software, etc.

## e. Network Traffic Analysis:

**Purpose:** Analyze network activity to identify communication patterns and potential security incidents.

**Procedure:**
- Use network analysis features within the forensic tool.
- Examine communication logs and network connections.

## f. Metadata Analysis:

**Purpose:** Extract and analyze metadata from files to gather additional information.

**Procedure:**
- Access the metadata analysis tool in the forensic software.
- Review metadata of files for details like creation/modification timestamps, author information, etc.

## g. Hash Analysis:

**Purpose:** Verify file integrity and identify known malicious files using hash values.

**Procedure:**
- Calculate and compare hash values of files against known databases.
- Identify any files with suspicious or known malicious hashes.

## 7. Extracting Evidence and Providing Expert Opinion

1. Utilize the chosen forensic tool to extract relevant evidence.
2. Document findings and provide an expert opinion based on the analysis.

---

**Note:** Always adhere to legal and ethical guidelines when performing forensic analyses and data recovery.

Feel free to modify and expand on each section based on your specific lab requirements.
