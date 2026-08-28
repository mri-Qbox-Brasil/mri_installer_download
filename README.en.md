# MRI Installer - Official Distribution 🚀

Read this in: [🇧🇷 Português](README.md) | [🇪🇸 Español](README.es.md)

The **MRI Installer** is the gateway to the **MRI Qbox Brasil** ecosystem. A professional, resilient, and secure tool to automate your FiveM server installation.

[![GitHub release (latest by date)](https://img.shields.io/github/v/release/mri-Qbox-Brasil/mri_installer_download?style=for-the-badge&color=7289da)](https://github.com/mri-Qbox-Brasil/mri_installer_download/releases/latest)
[![Security - VirusTotal Verified](https://img.shields.io/badge/Security-VirusTotal%20Scan-blue?style=for-the-badge&logo=virustotal)](https://github.com/mri-Qbox-Brasil/mri_installer_download/releases/latest)

---

## ✨ Why use MRI Installer?

Unlike common installers, MRI was built with a focus on **stability** and **security**:

- 🛡️ **Verified Security**: Every version uploaded to this repository is automatically scanned by **VirusTotal**. The report link is available in each release.
- 💾 **Resilient Installation (Resume)**: Did the internet drop or the PC shut down? The installer detects where it left off and resumes progress automatically, without corrupting files.
- 🗄️ **Automatic Database**: Don't have MariaDB installed? The software takes care of it for you in the background, with resilience against Windows blocking (UAC). Already have a database? Point it to any existing host/port and reveal the password while configuring.
- 👑 **Personalized txAdmin**: The installer automatically configures your server name and language in the management panel.
- 🇺🇸 **Multilingual Support**: Intuitive interface and full support for English, Portuguese, and Spanish.
- 🐧 **Linux Support**: Native binary for Linux servers with an interactive terminal installer or fully automated via flags.

## 🚀 How to Get Started

### Windows (graphical interface)

1. Go to the [**Releases**](https://github.com/mri-Qbox-Brasil/mri_installer_download/releases/latest) tab.
2. Download the `mri_installer.exe` file.
3. Run the installer and follow the 7 guided steps (Environment, Engine, Recipe, Summary, Deploy, Configuration, and Dashboard).

### Linux (terminal / headless server)

1. Go to the [**Releases**](https://github.com/mri-Qbox-Brasil/mri_installer_download/releases/latest) tab.
2. Download the `mri_installer_linux` file.
3. Grant execute permission and run:

```bash
chmod +x mri_installer_linux

# Interactive mode (recommended for beginners)
./mri_installer_linux

# Non-interactive mode (full flags)
./mri_installer_linux \
  --install-path /opt/fivem/mri_qbox \
  --server-name "My Server" \
  --license-key "cfxk_..." \
  --db-pass "password" \
  --install-mariadb

# Subcommands, for servers that are already installed
./mri_installer_linux --login
./mri_installer_linux --update-artifacts --install-path /opt/fivem/mri_qbox
./mri_installer_linux --backup --install-path /opt/fivem/mri_qbox
./mri_installer_linux --list-resources --install-path /opt/fivem/mri_qbox
```

> [!NOTE]
> In interactive mode, the installer shows an 8-character **authorization code**. Approve it by running `/liberar <code>` on our Discord **or** by opening the shown link — no browser needed on the server.

> [!TIP]
> **Security Tip**: Always make sure to download the executable from this official repository of the **MRI Qbox Brasil** organization.

## 🛡️ Transparency and Security

We take our community's security seriously. That's why we integrated our publishing pipeline with the **VirusTotal** API.

You can find the security seal and the link to the full technical report in the description of each released version.

The installer also **embeds no credentials**: access validation and recipe downloads happen on our servers, so inspecting the binary reveals no keys or secrets.

---

Developed with ❤️ by the [MRI QBOX BRASIL](https://github.com/mri-qbox-brasil) team
