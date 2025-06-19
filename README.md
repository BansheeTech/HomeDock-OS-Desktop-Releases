# HomeDock OS Desktop

![HomeDock OS Desktop Running on macOS ARM64](https://raw.githubusercontent.com/BansheeTech/Logo/refs/heads/main/homedock-os/desktop-screen-mac.webp "HomeDock OS Desktop Running on macOS ARM64")

This repository contains the official **installers** for [HomeDock OS Desktop](https://www.homedock.cloud), the universal self-hosted Cloud OS built for professionals.

> 💡 HomeDock OS Desktop transforms your computer into a private cloud environment with encrypted storage and secure app deployment.

---

## 🔽 Download Latest Version

You can download the latest version for your platform from the [Releases](https://github.com/BansheeTech/HomeDock-OS-Desktop-Releases/releases) page or [our official website](https://www.homedock.cloud/install/).

| Platform                         | Installer / Command                                  |
| -------------------------------- | ---------------------------------------------------- |
| 🖥️ macOS (Intel & Apple Silicon) | `.dmg` file                                          |
| 🪟 Windows 10/11 (x64)           | `.exe` file                                          |
| 🐧 Linux (Headless setup)        | `curl -fsSL https://get.homedock.cloud \| sudo bash` |

---

## 📌 How to Install

### macOS

1. Download the `.dmg` file.
2. Open it and drag **HomeDock OS Desktop** into your Applications folder.
3. If macOS blocks it, [read this quick guide](https://support.apple.com/en-us/HT202491) to allow unsigned apps.
4. Alternatively, you can run the following command on the Terminal until we sign the app:

```bash
sudo xattr -rd com.apple.quarantine "/Applications/HomeDock OS Desktop.app"
```

### Windows

1. Download the `.exe` installer.
2. Run it and follow the setup wizard.
3. Shortcut will appear on your desktop and start menu.

---

## 📣 About HomeDock OS Desktop

**HomeDock OS Desktop** is part of the [HomeDock OS ecosystem](https://www.homedock.cloud), a secure self-hosted cloud platform built for:

- Freelancers & professionals
- Developers & tech-savvy users
- Startups & small businesses
- You!

Installed apps behave just like native ones while the HomeDock OS Desktop is running, delivering a seamless user experience, you can also link all your **Cloud Instances** from [HomeDock Cloud](https://dashboard.homedock.cloud/plans) for the exact same experience, fully managed and accessible from anywhere.

> 💡 With **HomeDock OS Desktop**, you can finally self-host HomeDock OS natively on **Windows and macOS**, platforms that have traditionally been off-limits for serious self-hosting.

---

## 🛠️ Troubleshooting and Error Reporting

If you encounter any issues while using **HomeDock OS Desktop**, we’ll be happy to help.

Please attach the `hdos_desktop.log` file in your email to **support@homedock.cloud**. This log contains technical information that is **incredibly helpful for us to improve the app and move it out of Beta**.

🔍 You can find the log file here:

- **macOS**:  
  `/Users/your_username/Library/Application Support/cloud.homedock.app/homedock/hdos_desktop.log`

- **Windows**:  
  `%APPDATA%\cloud.homedock.app\homedock\hdos_desktop.log`

Thanks for your support and for being part of the future of self-hosting.

---

## 🚨 Source Code

This repository **does not contain the source code**. It is exclusively used to distribute signed installers and official binaries for **HomeDock OS Desktop**, our Electron-based project that brings HomeDock OS to Windows and macOS.

The source code of **HomeDock OS Desktop** is private and will not be released in the short term due to strategic reasons and to prevent potential misuse or replication of critical desktop infrastructure components.

For more information, visit:

➡️ https://www.homedock.cloud
