PowerShell Installation Script for Linux

This script automates the installation of PowerShell on a Linux system. It updates the system’s package list, installs required dependencies, downloads the latest PowerShell .deb package, installs it, and finally removes the installation file to keep your system clean.
Prerequisites

    A Debian-based Linux distribution (e.g., Ubuntu)

    wget package (automatically installed by the script)

Steps Performed by the Script

    Updates package list using sudo apt-get update.

    Installs wget, which is required to download the PowerShell .deb package.

    Downloads the PowerShell package version 7.5.2 from GitHub.

    Installs the downloaded .deb package using dpkg.

    Fixes any missing dependencies using sudo apt-get install -f.

    Removes the downloaded PowerShell package to clean up the system.

    Starts PowerShell using the pwsh command.

Requirements

    A working internet connection to download the PowerShell package.

Usage

    Clone the repository or download the script.

    Run the script with the following command:

sudo bash install-powershell.sh

After successful installation, PowerShell can be launched by running:

    pwsh

License

This project is licensed under the MIT License - see the LICENSE file for details.
