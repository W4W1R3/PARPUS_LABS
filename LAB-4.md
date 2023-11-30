# Network Traffic Capture with Wireshark

## Introduction
In this lab, we will explore the process of capturing and analyzing network traffic using Wireshark. Wireshark is a powerful network protocol analyzer that allows us to inspect the data traveling back and forth on a network.

## Objectives
- Install and configure Wireshark on both Windows and Linux.
- Select a network interface for capturing traffic.
- Start and stop traffic capture using Wireshark.
- Analyze source and destination IP addresses, port numbers, and protocols.
- Extract files from captured traffic.
- Analyze potential malware in network traffic.

## Steps

### 1. Installing Wireshark
- **Windows:**
  - [Download Wireshark](https://www.wireshark.org/download.html) for Windows.
  - Follow the installation instructions.

- **Linux:**
  - Use the package manager to install Wireshark. For example, on Debian-based systems:
    ```bash
    sudo apt-get update
    sudo apt-get install wireshark
    ```
    Ensure your user is added to the `wireshark` group:
    ```bash
    sudo usermod -aG wireshark $USER
    ```
    Log out and log back in for the changes to take effect.

### 2. Configuring Wireshark
- Open Wireshark and select the network interface to capture traffic.

### 3. Capturing Traffic
- Start capturing traffic.
- Perform network activities to generate traffic.
- Stop the capture.

### 4. Analyzing Captured Traffic
- Analyze source and destination IP addresses.
- Identify port numbers and protocols.
- Extract files if any.

### 5. Analyzing Malware
- Look for suspicious patterns in the captured traffic.
- Identify potential malware based on behavior.

## Conclusion
Wireshark provides valuable insights into network activities, allowing us to troubleshoot issues, analyze security threats, and understand the flow of data on a network.

Feel free to explore additional features and functionalities offered by Wireshark to enhance your network analysis skills.
