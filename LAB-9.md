# Data and Password Recovery Procedures

This document outlines practical steps for data and password recovery in various scenarios. It covers retrieving files, recovering passwords, and conducting forensic analyses.

## 1. Retrieving SAM and SYSTEM Files from an Offline Windows OS

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

## 6. Using Autopsy, FTK, etc., for Forensic Analyses

1. Install and configure the forensic analysis tool (e.g., Autopsy, FTK).
2. Load the forensic image for analysis.
3. Conduct various analyses such as file recovery, timeline analysis, etc.

## 7. Extracting Evidence and Providing Expert Opinion

1. Utilize the chosen forensic tool to extract relevant evidence.
2. Document findings and provide an expert opinion based on the analysis.

---

**Note:** Always adhere to legal and ethical guidelines when performing forensic analyses and data recovery.

Feel free to modify and expand on each section based on your specific lab requirements.
