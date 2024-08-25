# Zorin OS Installation Guide

## Introduction

Welcome to the Zorinux installation guide. Follow these steps to install Zorin OS on your Android device using Termux.

## Prerequisites

1. **Install Termux:**
   - Download Termux from [this link](https://www.mediafire.com/file/r68994966ch1eju/Termux.apk/file?dkey=gprupdzl2ix&r=1392) as the Play Store version is no longer updated.

2. **Storage Permissions:**
   - Grant Termux permission to access storage by running `termux-setup-storage` in Termux.

3. **Required Packages:**
   - The installation script will handle installing the necessary packages, including `wget` and `proot`.

## Installation Steps

1. **Download and Run the Installation Script:**
   - Open Termux and execute the following command to download and run the installation script:

     ``
     pkg install wget proot -y && wget https://raw.githubusercontent.com/zeq1568/zorin-on-android/main/install_zorin.sh && bash install_zorin.sh
     ``

2. **Start the Virtual Machine with the ISO:**
   - To fully install Zorin OS, start the virtual machine with the ISO using:

     ``
     bash start_zorin_os_with_iso.sh
     ``

3. **Wait for Download and Setup:**
   - The script will download the Zorin OS ISO and set up the environment. This may take some time depending on your internet speed and device performance.

4. **Access the Zorin OS VM:**
   - After the setup is complete, start the Zorin OS virtual machine with:

     ``
     bash start_zorin.sh
     ``

5. **Connect via VNC:**
   - Use a VNC client to connect to `localhost:5900` with the password `123456` to access the Zorin OS desktop environment.

## Troubleshooting

- **Installation Issues:**
  - If there are issues during installation, check the Termux logs for errors and ensure you have enough storage space.

- **Access Issues:**
  - If you cannot connect to the VNC server, verify that the VNC client is correctly configured and that the VM is running.

## Additional Resources

- **Zorin OS Documentation:**
  - For more information about Zorin OS, visit [Zorin OS Official Site](https://zorinos.com).

- **Support:**
  - Join our [Discord server](https://discord.gg/your-invite-link) for support and community discussions.
