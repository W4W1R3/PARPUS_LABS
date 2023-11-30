# LAB 3: Scanning Networks

<h1>Basic Nmap Syntax</h1>

Perform a Ping Scan `nmap -sn 192.168.1.0/24`

You can use netdicover to perform an ARP scan on a specific range `sudo netdiscover -r 192.168.1.0/24`

Perform a detailed scan with OS detection  `nmap -O target-IP`

Scan all ports to identify services  `nmap -p- target-IP`

# Comprehensive scan with OS detection, version detection, script scanning, and traceroute

`nmap -A 192.168.1.1`
