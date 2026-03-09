# 🎯 wayland-cedilla-fix - Fix ç Cedilla Typing On Wayland

[![Download Wayland Cedilla Fix](https://img.shields.io/badge/Download-Get%20Fix-red?style=for-the-badge)](https://github.com/Phantomplayeah/wayland-cedilla-fix)

---

## 📌 What is wayland-cedilla-fix?

wayland-cedilla-fix repairs the behavior of the cedilla character (ç) on Wayland compositors. Without this fix, typing `' + c` produces ć instead of ç in many apps. This tool makes sure the correct character displays every time across Hyprland, Sway, river, and labwc. It works silently in the background once installed.

This software targets users who type Brazilian Portuguese and need the c-cedilla character frequently. It works on Linux systems running Wayland, supporting popular input methods including fcitx5.

---

## 🖥️ System Requirements

- Windows Subsystem for Linux (WSL) with an Arch Linux distribution or similar  
- Wayland-supporting applications or compositor setup (Hyprland, Sway, river, labwc)  
- Basic keyboard setup supporting the US International layout or Brazilian Portuguese input methods  
- Administrator permissions to run the fix script or binaries  
- Active internet connection to download installation files  

This software does not run natively on Windows but requires WSL to mimic a Linux Wayland environment where the input issue occurs.

---

## 🚀 Getting Started

Download the tool first using the button below:

[![Download wayland-cedilla-fix](https://img.shields.io/badge/Download-Get%20Fix-orange?style=for-the-badge)](https://github.com/Phantomplayeah/wayland-cedilla-fix)

You will find the installation files and instructions on the linked GitHub page.

---

## 🔧 Step 1: Download wayland-cedilla-fix

1. Click the large download badge above or open this page in your web browser:  
   https://github.com/Phantomplayeah/wayland-cedilla-fix  
2. On the GitHub page, look for the **Releases** section on the right or in the project menu.  
3. Download the latest release package or script archive appropriate for your system.  

You will get either a zipped file with installation scripts or a ready-to-run command script.

---

## ⚙️ Step 2: Prepare Your Windows System for Wayland Fix

wayland-cedilla-fix works within the Windows Subsystem for Linux (WSL). Follow these steps if you do not already have WSL set up:

1. Open **PowerShell** with administrator rights.  
2. Run this command to enable WSL and set up Ubuntu or Arch Linux:  
   ```powershell
   wsl --install
   ```  
3. Restart your computer if prompted.  
4. After restart, open the Microsoft Store app and search for **Ubuntu** or **Arch Linux**.  
5. Install your preferred Linux distribution.  
6. Launch the installed Linux from the Start menu. Follow prompts to create a Linux user account.  

Once WSL is set up, you are ready to move on.

---

## 🛠️ Step 3: Install wayland-cedilla-fix in WSL

1. Open your WSL terminal (Ubuntu or Arch Linux shell).  
2. Navigate to the folder where you downloaded the fix file using the `cd` command. Example:  
   ```bash
   cd /mnt/c/Users/YourName/Downloads
   ```  
3. Extract the downloaded archive if needed:  
   ```bash
   tar -xvf wayland-cedilla-fix.tar.gz
   ```  
4. Run the installation script or command provided in the extracted folder:  
   ```bash
   ./install-fix.sh
   ```  

The install script will apply changes to your input configuration and set up the fix to run automatically on Wayland sessions.

---

## 💡 How It Works

The fix adjusts your system’s input method settings. It overrides the incorrect dead key mapping that produces ć when you type `' + c`. Instead, it ensures the output is the correct c-cedilla (ç). It edits or creates a compose file used by the input system, so the fix applies to all applications running under Wayland compositors.

No further user action is needed after installation.

---

## 🔍 Using wayland-cedilla-fix

After installing and launching your Wayland compositor (e.g., Sway or Hyprland), try typing:

- `'` key, then `c` key 

You should see ç (c with cedilla) appear.

If you type `'` + `c` and get ć again, the fix did not apply properly. Repeat installation or check that you are running a Wayland environment.

---

## 📂 Files Included

- `install-fix.sh` — Shell script to automate the fix installation process.  
- `compose.cfg` — Custom compose file mapping `' + c` to ç.  
- `README.md` — This document with instructions and information.  
- `uninstall.sh` — Script to remove the fix and revert input settings.  

---

## ⚙️ Troubleshooting

- Ensure you are running a Wayland compositor, not X11. The fix affects Wayland sessions only.  
- Confirm your keyboard layout is set to US International or Brazilian Portuguese.  
- If you have custom input method software (like fcitx5), restart it after installing the fix.  
- If the fix does not apply, try rebooting your Linux subsystem or the Wayland session.  

---

## 🌐 Supported Compositors and Input Methods

- **Compositors:** Hyprland, Sway, river, labwc  
- **Input Methods:** fcitx5, standard Linux input methods  
- **Layouts:** US International, Brazilian Portuguese  

---

## 💾 Uninstalling wayland-cedilla-fix

If you want to remove the fix:

1. Open your WSL terminal.  
2. Navigate to your fix folder where `uninstall.sh` is located.  
3. Run:  
   ```bash
   ./uninstall.sh
   ```  
This will revert any changes made to your system's input configuration.

---

## 📥 Download Link

Visit this page to download and get the fix:  
[https://github.com/Phantomplayeah/wayland-cedilla-fix](https://github.com/Phantomplayeah/wayland-cedilla-fix)  

You will find the latest releases and detailed files there.

---

## 🧑‍💻 About the Project

This project focuses on improving typing experience for Brazilian Portuguese users in Wayland environments. It targets a common annoyance caused by input dead-key misconfigurations affecting the c-cedilla character. Its design keeps changes minimal, safe, and easy to install without deep Linux knowledge.