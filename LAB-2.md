# LAB 2: Using the Linux OS

 <h2> Installation of Linux OS: </h2>

 <h3> Choose a Linux Distribution: </h3> 
 
Select a Linux distribution suitable for information security and forensics. Popular choices include Kali Linux, Parrot Security OS, and Ubuntu (with additional security tools installed).

<h3>Download the ISO Image:</h3> 

Visit the official website of the chosen Linux distribution.

![Screenshot](https://github.com/W4W1R3/PARPUS_LABS/blob/main/Files/linux-distro-stickers.png)

Download the ISO image for your system architecture (32-bit or 64-bit).

<h3>Create a Bootable USB or DVD:</h3> 

Use a tool like Rufus (for Windows) or dd (for Linux) to create a bootable USB drive.

![Screenshot](https://github.com/W4W1R3/PARPUS_LABS/blob/main/Files/dd.png) ![Screenshot](https://github.com/W4W1R3/PARPUS_LABS/blob/main/Files/Rufus-Software.webp)

Alternatively, you can burn the ISO image to a DVD.

<h3>Boot from USB or DVD:</h3> 

Insert the USB drive or DVD into the computer. Restart the computer and enter the BIOS/UEFI settings. Set the boot order to prioritize the USB drive or DVD.

<h3>Start the Installation:</h3> 

Boot from the USB or DVD to start the Linux live environment. Explore the live environment to ensure compatibility with your hardware.

<h3> Launch the Installer:</h3>

Find the installer icon on the desktop or in the application menu.

Double-click to launch the installer.

# Follow the Installation Wizard:
The installation wizard will guide you through the process.
Choose the installation language, keyboard layout, and time zone.

<h3>Partitioning:</h3> 

Decide on the disk partitioning. For simplicity, you can choose the option to use the entire disk.

Some distributions offer guided partitioning for beginners.

<h3>Create a User Account:</h3> 

Set up a username and password for the main user account.

Optionally, create a root password.

<h3> Install the Boot Loader:</h3>

Choose the location to install the boot loader (usually the default option is the entire hard drive).

<h3>Complete the Installation:</h3> 

Review the summary of your choices. Confirm and proceed with the installation.

# Remove Installation Media:

Once the installation is complete, remove the USB drive or DVD. Restart the computer.

# First Boot:

Login with the username and password you created during the installation.

Update and Install Additional Software: Open the terminal and update the system: 

`sudo apt update && sudo apt upgrade`

Install additional software and tools relevant to information security and forensics.

Post-Installation Configuration:

Configure network settings, install security updates, and set up any additional preference

