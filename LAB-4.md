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

# Steps

### 1. Installing Wireshark
**Windows:**
  - [Download Wireshark](https://www.wireshark.org/download.html) for Windows.
  - Follow the installation instructions.

  **Linux:**
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

# 2. Configuring Wireshark
Open Wireshark and select the network interface to capture traffic.

### 3. Capturing Traffic
#### 3.1 Start Capturing
Open Wireshark and choose the appropriate interface. Click the "Start" button to begin capturing traffic.

#### 3.2 Perform Network Activities
Conduct various network activities to generate traffic. This can include browsing websites, downloading files, or any network-related tasks.

#### 3.3 Stop the Capture
Once sufficient data is captured, click the "Stop" button to end the capture.

### 4. Analyzing Captured Traffic
#### 4.1 Source and Destination IP Addresses
Identify the source and destination IP addresses in the captured packets.
Look for patterns or anomalies.

#### 4.2 Port Numbers and Protocols
Analyze port numbers and protocols used in the communication.
Determine the nature of the traffic (HTTP, FTP, etc.).

#### 4.3 Extracting Files
If any files were transmitted, extract and analyze them for content.

# 5. Analyzing Malware
#### 5.1 Look for Suspicious Patterns
Once you have captured some traffic, you need to identify the packets that belong to the malware communication. This can be challenging, as malware often uses encryption, obfuscation, or spoofing to evade detection. However, you can look for some clues, such as unusual ports, domains, or patterns, that can indicate malicious activity. You can also compare the traffic with a baseline of normal traffic from the same host or network.

#### 5.2 Identify Potential Malware
After you have identified the malware traffic, you can analyze the malware protocol to understand how the malware communicates with its servers, victims, or peers. You can use Wireshark's built-in tools, such as dissectors, decoders, or statistics, to examine the structure, content, and behavior of the protocol. You can also use external tools, such as hex editors, encryption tools, or scripting languages, to decode, decrypt, or manipulate the protocol.


Another useful step in analyzing malware network traffic is to extract the malware artifacts from the captured packets. These can include files, commands, credentials, or indicators of compromise, that can provide more information about the malware's functionality, purpose, or origin. You can use Wireshark's export function, or other tools, such as NetworkMiner, to extract the artifacts from the traffic.

# Conclusion
Wireshark provides valuable insights into network activities, allowing us to troubleshoot issues, analyze security threats, and understand the flow of data on a network.

Feel free to explore additional features and functionalities offered by Wireshark to enhance your network analysis skills.
