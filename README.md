# 🐲 Bash Ghidra Installer

![Poster](https://github.com/asankaSovis/Ghidra_Installer/assets/46389631/93a61bf4-c6ce-4092-ad58-453c81a602eb)

---

**Ghidra Installer** is a third-party installer meant to easily set up Ghidra on Linux systems. It is currently written to install Ghidra v11.0.3 and Java Development Kit 22. It will install and set up the dash launcher for easy launching of the program. On top of this, it also supports the uninstalling of an existing Ghidra installation. Written in Bash, this is intended to be used in Linux environments that support Bash scripts.

This program is licensed under the **[MIT License](https://github.com/asankaSovis/Ghidra_Installer/blob/main/LICENSE)**.
Other components might be licensed under other licenses.
- Ghidra: [Apache License 2.0](https://github.com/NationalSecurityAgency/ghidra/blob/master/LICENSE)
- Java: [Oracle No-Fee Terms and Conditions (NFTC)](https://www.oracle.com/downloads/licenses/no-fee-license.html)

![Technologies](https://skillicons.dev/icons?i=bash,linux)

## 🐲 Prerequisites

The installer will run on almost any x64-based hardware system with any Linux distribution supporting **Bash**. [Java](https://www.oracle.com/java/) and [Ghidra](https://github.com/NationalSecurityAgency/ghidra) might have their requirements which can be found on their respective websites. An active internet connection is required to download the required components. Make sure not to run the script with `sudo` access as this might be too risky.

## 🐲 How to Install

Installation is straightforward. You'll need to follow the below steps to install Ghidra on your Linux environment.

1. Download a preferred release from the [Releases](https://github.com/asankaSovis/Ghidra_Installer/releases) section.
2. Optionally you can check the SHA-256 with a relevant tool.
3. Extract the zip file in a convenient location. You can use an archive program provided by your distribution.
4. Open a terminal on the location of the script file extracted. For this navigate to the extracted folder and right-click > *Open in Terminal*. This should be the procedure in most distributions.
5. Enter the following command to enable execution permission for the script.

    `chmod +x ./ghidra_install.sh`

6. In the same terminal enter the following command to start the installation.

    `./ghidra_install.sh`
  
7. Follow the instructions given on the terminal to install Ghidra.

## 🐲 Additional Options

You can provide additional arguments when running the installer under **Step 6** above.

### 1. Default Install

This will install Ghidra in the default location picked by the installer which is `~/Apps`.
- Command Structure: `./ghidra_install.sh`
- Example `./ghidra_install.sh`

### 2. Install Ghidra without Opening

The `-x` will install Ghidra but will not open Ghidra automatically after the installation is completed.
- Command Structure: `./ghidra_install.sh -x`
- Example `./ghidra_install.sh -x`

### 3. Install Ghidra with Custom Path

The `-i` or `--install` will allow the user to install Ghidra in a preferred location given under *[PATH]*. Please note that this folder must be within the user *home directory* and must already be present.
- Command Structure: `./ghidra_install.sh -i [PATH]` `./ghidra_install.sh --install [PATH]`
- Example `./ghidra_install.sh -i ~/path/to/install` `./ghidra_install.sh --install ~/path/to/install`

### 4. Install Ghidra with Custom Path Without Opening

The `-iX` will allow the user to install Ghidra in a preferred location. Please note that this folder must be within the user *home directory* and must already be present. This option also prevents Ghidra from opening automatically after installation.
- Command Structure: `./ghidra_install.sh -iX [PATH]`
- Example `./ghidra_install.sh -iX ~/path/to/install` `./ghidra_install.sh --install ~/path/to/install`

### 5. Uninstall Ghidra

The `-u` or `--uninstall` will uninstall an existing Ghidra installation.
- Command Structure: `./ghidra_install.sh -u` `./ghidra_install.sh --uninstall`
- Example `./ghidra_install.sh -u` `./ghidra_install.sh --uninstall`

### 6. Uninstall Ghidra with Custom Path

The `-u [PATH]` or `--uninstall [PATH]` will uninstall an existing Ghidra installation from a location provided in *[PATH]*. Please note that this folder must be within the user *home directory*.
- Command Structure: `./ghidra_install.sh -u [PATH]` `./ghidra_install.sh --uninstall [PATH]`
- Example `./ghidra_install.sh -u ~/path/to/uninstall` `./ghidra_install.sh --uninstall ~/path/to/uninstall`

### 7. Uninstall Ghidra but Leave JDK

The `-uJ` will uninstall an existing Ghidra installation but will leave the JDK intact.
- Command Structure: `./ghidra_install.sh -uJ`
- Example `./ghidra_install.sh -uJ`

### 8. Uninstall Ghidra with Custom Path but Leave JDK

The `-uJ [PATH]`  will uninstall an existing Ghidra installation from a location provided under *[PATH]* but will leave the JDK intact. Please note that this folder must be within the user *home directory*.
- Command Structure: `./ghidra_install.sh -uJ [PATH]`
- Example `./ghidra_install.sh -uJ ~/path/to/uninstall`

### 9. Check Version

The `-v` or `--version` will display version information for the program.
- Command Structure: `./ghidra_install.sh -v` `./ghidra_install.sh --version`
- Example `./ghidra_install.sh -v` `./ghidra_install.sh --version`

### 10. Display Parameters

The `-p` or `--parameters` will display all default parameters that will be used for installation including default install location, JDK download link and Ghidra download link.
- Command Structure: `./ghidra_install.sh -p` `./ghidra_install.sh --parameters`
- Example `./ghidra_install.sh -p` `./ghidra_install.sh --parameters`

### 11. Display Help

The `-h` or `--help` will output help information for the program.
- Command Structure: `./ghidra_install.sh -h` `./ghidra_install.sh --help`
- Example `./ghidra_install.sh -h` `./ghidra_install.sh --help`

## 🐲 Reporting Bugs and Requesting Features

To report bugs and request features, go to [issues](https://github.com/asankaSovis/Ghidra_Installer/issues) and create a new Issue. Make sure to include the terminal output and a clear explanation of what you were trying to do and what happened. Also, include device information such as the distro and install path. It will take some time to provide support.

## 🐲 Contributing

Anyone can contribute to this project. If you're a bash programmer, any new features or bug fixes are greatly appreciated. Any suggestions are also appreciated along with documentation improvements. The same goes for any bug reporting and feature suggestions. Also, if you're willing to, consider trying all features of this script in your distro and providing any feedback; especially if you're on a different distro.

---

> Tested on Ubuntu 23.10
> 
> ![Tested list](https://skillicons.dev/icons?i=ubuntu)

`© 2024 Asanka Sovis`
