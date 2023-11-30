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
#### 3.1 Start Capturing
- Open Wireshark and choose the appropriate interface.
- Click the "Start" button to begin capturing traffic.

#### 3.2 Perform Network Activities
- Conduct various network activities to generate traffic.
- This can include browsing websites, downloading files, or any network-related tasks.

#### 3.3 Stop the Capture
- Once sufficient data is captured, click the "Stop" button to end the capture.

### 4. Analyzing Captured Traffic
#### 4.1 Source and Destination IP Addresses
- Identify the source and destination IP addresses in the captured packets.
- Look for patterns or anomalies.

#### 4.2 Port Numbers and Protocols
- Analyze port numbers and protocols used in the communication.
- Determine the nature of the traffic (HTTP, FTP, etc.).

#### 4.3 Extracting Files
- If any files were transmitted, extract and analyze them for content.

### 5. Analyzing Malware
#### 5.1 Look for Suspicious Patterns
- Once you have captured some traffic, you need to identify the packets that belong to the malware communication. This can be challenging, as malware often uses encryption, obfuscation, or spoofing to evade detection. However, you can look for some clues, such as unusual ports, domains, or patterns, that can indicate malicious activity. You can also compare the traffic with a baseline of normal traffic from the same host or network.

#### 5.2 Identify Potential Malware
- Based on observed behavior, identify potential malware in the network traffic.
- Note any indicators of compromise.

## Conclusion
Wireshark provides valuable insights into network activities, allowing us to troubleshoot issues, analyze security threats, and understand the flow of data on a network.

Feel free to explore additional features and functionalities offered by Wireshark to enhance your network analysis skills.
