# LAB 1: Setting Up Simple Networks and Address Assignment

Objective: Understand the basics of network setup and address assignment.

`I'll be using packettracer to demo this lab`

## {1A} Connecting Two Computers Directly

Task: Connect two computers using a crossover cable.

Steps:

    • Assign static IP addresses to each computer.
    • Set a static IP address (e.g., 192.168.1.1 or 192.168.1.10 ) with subnet mask 255.255.255.0.
    • Verify connectivity using basic commands (ping).
    
# {1B} Connecting More Than Two Computers Using a Switch

## Task: Set up a small network with three or more computers using a switch.

### Steps:

1. **Configure the Switch:**

            - Connect the switch to a power source.
            - Connect computers to the switch using Ethernet cables.
            - Power on the switch.

2. **Assign IP Addresses using DHCP:**

            - Ensure that DHCP is enabled on the switch.
            - Computers connected to the switch will automatically receive IP addresses from the DHCP server.
            - To verify assigned IP addresses on each computer, follow these steps:

        ```bash
        # Display IP configuration on Windows
        ipconfig

        # Display IP configuration on Linux
        ifconfig
        ```

3. **Test Network Connectivity:**

    - Open a command prompt or terminal on each computer.

    - Ping other computers in the network to test connectivity:

        ```bash
        # Ping another computer by its IP address
        ping [target-IP]

        # Example: ping 192.168.1.2
        ```

    - Ensure successful ping replies, indicating network connectivity.

    - For additional testing, try accessing shared resources or services on other computers.

### Notes:

- If DHCP is not available or you want to assign static IP addresses:

    - Manually configure IP addresses on each computer within the same subnet.

    - Example for Linux:

        ```bash
        sudo ifconfig eth0 [desired-IP] netmask [subnet-mask]
        ```
    
# {1C} Connecting Two Networks Through a Router

## Task Overview

Introduce a router to connect two separate networks and ensure seamless communication between devices on these networks.

## Steps

### 1. Configure Router Interfaces

#### a. Access Router CLI

Access the command-line interface (CLI) of the router. This can be done through a console connection or a management interface.

```
router> enable
router# configure terminal
```
#### b. Enter Interface Configuration Mode

Navigate to the interface configuration mode for the interfaces connecting to each network.

`
router(config)# interface <interface_type> <interface_number>
`

Replace <interface_type> and <interface_number> with the actual interface type and number (e.g., GigabitEthernet0/0).

#### c. Configure IP Addresses

Assign IP addresses to the router interfaces within the respective network subnets.

`
router(config-if)# ip address <ip_address> <subnet_mask>
router(config-if)# no shutdown
`

Replace <ip_address> and <subnet_mask> with the specific IP address and subnet mask for each interface.

### 2. Set Up Routing Tables

a. Configure Static Routes

Define static routes on the router to reach networks on the opposite side.

bash

router(config)# ip route <destination_network> <subnet_mask> <next_hop>

Replace <destination_network>, <subnet_mask>, and <next_hop> with the details of the target network and next-hop router.
3. Test Communication
a. Ping Test

From devices on Network A, attempt to ping a device on Network B, and vice versa.

bash

DeviceA> ping <ip_address_of_deviceB>

Ensure successful pings indicate proper communication between the two networks
    
# {1D} Setting Up Static and DHCP

Task: Understand the difference between static and dynamic IP assignment.

Steps:

    • Assign static IP addresses to devices in a network.
    • Enable DHCP on a server and configure clients to obtain IP dynamically.
    • Analyze the advantages and disadvantages of static vs. dynamic addressing.
