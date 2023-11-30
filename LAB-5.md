# Metasploit Basics Guide

## 5. Using Metasploit through msfconsole

Metasploit is a powerful penetration testing framework. Here's a guide on basic commands and tasks within msfconsole.

### Msfconsole Basic Commands

1. **Starting msfconsole:**
    ```bash
    msfconsole
    ```

2. **Help Command:**
    ```bash
    help
    ```

3. **Search for Modules:**
    ```bash
    search [keyword]
    ```

### Setting up Workspaces

Metasploit allows you to organize your work using workspaces.

1. **Creating a Workspace:**
    ```bash
    workspace -a [workspace_name]
    ```

2. **Switching Workspace:**
    ```bash
    workspace [workspace_name]
    ```

### Loading and Configuring Modules

1. **Loading a Module:**
    ```bash
    use [module_name]
    ```

2. **Showing Module Info:**
    ```bash
    info
    ```

3. **Configuring Module Options:**
    ```bash
    set [option_name] [value]
    ```

### Launching Exploits Remotely

1. **Selecting a Payload:**
    ```bash
    set payload [payload_name]
    ```

2. **Setting the Target IP:**
    ```bash
    set RHOST [target_ip]
    ```

3. **Exploiting:**
    ```bash
    exploit
    ```

### Creating File-Format Exploits

Metasploit supports various file-format exploits. Examples include:

- WinRAR Name Spoofing
- Office Word Macro

### Using Meterpreter and Shell Payloads

1. **Meterpreter Payload:**
    ```bash
    set payload windows/meterpreter/reverse_tcp
    ```

2. **Shell Payload:**
    ```bash
    set payload cmd/unix/reverse
    ```

### Handling Meterpreter and Shell Sessions

1. **Interacting with Sessions:**
    ```bash
    sessions -i [session_id]
    ```

2. **Post-Exploitation Tasks:**
    - Explore the compromised system
    - Gather information
    - Execute commands

## Conclusion

This guide covers the basics of using Metasploit through msfconsole. Remember to use this tool responsibly and only in ethical hacking scenarios.
