# Zorin OS Uninstallation Guide

## Introduction

If you need to remove Zorin OS from your Android device, follow these steps to uninstall it using Termux.

## Uninstallation Steps

1. **Download and Run the Uninstallation Script:**
   - Open Termux and execute the following command to download and run the uninstallation script:

     ``
     pkg install wget proot -y && wget https://raw.githubusercontent.com/zeq1568/zorin-on-android/main/uninstall_zorin.sh && bash uninstall_zorin.sh
     ``

2. **Wait for Uninstallation:**
   - The script will remove the Zorin OS installation and clean up the associated files. This may take some time depending on your device performance.

3. **Verify Removal:**
   - Check that all Zorin OS files have been removed from your storage directory. Ensure the `ISOs` directory and other related files are deleted.

4. **Script Self-Destruct:**
   - After the uninstallation is complete, the script will delete itself to prevent any further use.

## Troubleshooting

- **Uninstallation Issues:**
  - If the uninstallation script encounters errors, check Termux logs for details and ensure you have the necessary permissions.

- **Leftover Files:**
  - If some files remain, manually delete them from `/storage/emulated/0/ISOs` and any other directories where Zorin OS files were stored.

## Additional Resources

- **Zorin OS Documentation:**
  - For more information about Zorin OS, visit [Zorin OS Official Site](https://zorinos.com).

- **Support:**
  - Join our [Discord server](https://discord.gg/your-invite-link) for support and community discussions.
