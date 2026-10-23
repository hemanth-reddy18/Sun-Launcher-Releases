<div align="center">

# ☀️ Sun Launcher

**A focused, ambient desktop operating space for Windows, macOS, and Linux.**

[![Version](https://img.shields.io/badge/version-0.21.0-amber.svg?style=flat-square)](https://github.com/hemanth-reddy18/Sun-Launcher-Releases/releases)
[![SafeBuild](https://img.shields.io/badge/SafeBuild-verified-10b981.svg?style=flat-square)](https://github.com/hemanth-reddy18/safebuild-skill)
[![Platform](https://img.shields.io/badge/platform-macOS%20%7C%20Windows%20%7C%20Linux-blue.svg?style=flat-square)](https://github.com/hemanth-reddy18/Sun-Launcher-Releases/releases)
[![License](https://img.shields.io/badge/license-Proprietary-red.svg?style=flat-square)](#license)
[![Security](https://img.shields.io/badge/security-Sun%20Shield%204--Layer-emerald.svg?style=flat-square)](#-sun-shield--security-hardening)
[![Electron](https://img.shields.io/badge/electron-44.9.1-teal.svg?style=flat-square)](https://www.electronjs.org/)

<p align="center">
  Sun consolidates your favorite AI assistants, corporate communication suites, and media workflows into clean, dedicated Modes.<br>
  Built with sandboxed WebContentsView stages, native macOS notch awareness, and hardware-accelerated Liquid Glass aesthetics.
</p>

</div>

---

## 📥 Downloads (Latest v0.21.0)

All official binary releases in this repository are packaged and distributed following the [SafeBuild Specification](https://github.com/hemanth-reddy18/safebuild-skill) to guarantee tamper-evident delivery, cryptographic hash verification, and zero bundled telemetry.

| Platform | Type | Architecture | SafeBuild Direct Download | Checksum / Digest |
| :--- | :--- | :--- | :--- | :--- |
| **macOS** | Universal DMG (`.dmg`) | Apple Silicon (M1/M2/M3/M4) & Intel | [**Download for macOS (.dmg)**](https://github.com/hemanth-reddy18/Sun-Launcher-Releases/releases/latest/download/Sun-TV-Mac-universal.dmg) | [View SHA-256](https://github.com/hemanth-reddy18/Sun-Launcher-Releases/releases) |
| **Windows** | Portable Executable (`.exe`) | 64-bit Windows 10 / 11 | [**Download for Windows (.exe)**](https://github.com/hemanth-reddy18/Sun-Launcher-Releases/releases/latest/download/Sun-TV-Windows.exe) | [View SHA-256](https://github.com/hemanth-reddy18/Sun-Launcher-Releases/releases) |
| **Linux** | Standalone AppImage (`.AppImage`) | 64-bit Linux (Ubuntu, Fedora, Arch) | [**Download for Linux (.AppImage)**](https://github.com/hemanth-reddy18/Sun-Launcher-Releases/releases/latest/download/Sun-TV-Linux.AppImage) | [View SHA-256](https://github.com/hemanth-reddy18/Sun-Launcher-Releases/releases) |
| **Linux** | Debian Package (`.deb`) | Ubuntu / Debian x64 | [**Download for Linux (.deb)**](https://github.com/hemanth-reddy18/Sun-Launcher-Releases/releases/latest/download/Sun-TV-Linux.deb) | [View SHA-256](https://github.com/hemanth-reddy18/Sun-Launcher-Releases/releases) |

> 📦 **All Releases & Checksums**: View all release tags, changelogs, and SHA-256 verification digests at [GitHub Releases](https://github.com/hemanth-reddy18/Sun-Launcher-Releases/releases).

---

## 🛡️ SafeBuild Release Integrity & Verification

Following [SafeBuild standards](https://github.com/hemanth-reddy18/safebuild-skill), we provide transparent SHA-256 checksums for every build so you can verify binary integrity before executing:

### 1. macOS Verification (`.dmg`)
Verify the SHA-256 checksum in Terminal:
```bash
shasum -a 256 Sun-TV-Mac-universal.dmg
```
*Installation & Gatekeeper*: Open the DMG and drag Sun Launcher to your `Applications` folder. Because community preview builds are ad-hoc signed, macOS may prompt an unidentified developer notice on first run. Permit launch via **System Settings ➔ Privacy & Security ➔ Open Anyway**.

### 2. Windows Verification (`.exe`)
Verify the SHA-256 checksum in PowerShell:
```powershell
Get-FileHash .\Sun-TV-Windows.exe -Algorithm SHA256
```
*Installation & SmartScreen*: Sun Launcher is a portable executable — no intrusive registry installation or root services required. Simply run the `.exe`. As fresh releases build reputation with Microsoft SmartScreen, click **More info ➔ Run anyway** if prompted.

### 3. Linux Verification (`.AppImage` / `.deb`)
Verify the SHA-256 checksum in bash:
```bash
sha256sum Sun-TV-Linux.AppImage
# Or for Debian package:
sha256sum Sun-TV-Linux.deb
```
Make the AppImage executable:
```bash
chmod +x Sun-TV-Linux.AppImage
./Sun-TV-Linux.AppImage
```

---

## ✨ What's New in v0.21.0

### 🍎 MacBook Display Notch Optimization
- **Dynamic Display Safe-Area Handling**: Automatically calculates top insets on 14" & 16" MacBook Pro and 13.6" & 15" MacBook Air displays.
- **Zero Content Clipping**: Top navigation, stage rail, embedded browser views, and top switcher dynamically avoid the camera housing.
- **Native Traffic-Light Alignment**: 80px left clearance in windowed mode keeps interactive content clear of macOS window controls.
- **Windows & Linux Invariance**: Scoped strictly to macOS displays with zero layout regressions on Windows or Linux.

### 🛍️ Liquid Glass Apps Store
- **1-Click In-App Installer**: Browse top AI and corporate apps, watch real-time in-app installation progress ($0\% \rightarrow 100\%$), and pin apps directly to your preferred Mode.
- **OS Auto-Detection**: Dynamically detects macOS (`.dmg`), Windows (`.exe`), or Linux (`.AppImage`) and presents platform-tailored packages with interactive manual override.
- **Unified Catalog**:
  - **AI Suites**: Anthropic Claude, OpenAI ChatGPT, Cursor, Perplexity, Google Gemini, Google DeepMind Antigravity, Notion AI, Codex.
  - **Corporate & Work**: Slack, Microsoft Teams, Zoom Workplace, Google Chrome, VS Code, Figma, Linear, Asana, Jira, GitHub, Google Docs.
  - **Media & Entertainment**: YouTube, Spotify, Netflix, JioHotstar, Amazon Prime Video.
  - **Games**: Steam, Epic Games Store, Xbox Cloud Gaming.
- **Clean Starting Slate**: Starts completely clean with zero forced pre-pinned bloat; configure only what you need.

### 🛡️ Sun Shield & Security Hardening
- **4-Layer Protection**: Loopback DNS engine, Chromium network request filter, Brave-style cosmetic ad block, and domain allowlists.
- **Resilient Fallback**: Automatic failover to public secure DoH resolvers (Cloudflare, Quad9, AdGuard) if the primary resolver is unreachable.
- **Hardened YouTube Experience**: Zero-interruption video streaming with ad domain blocking and clean Stage routing.
- **Security Advisor**: Audits system hygiene, tracks tamper-chained logs, and enforces strict payload limits.

### 🌐 Direct In-App Chrome Integration
- Google Chrome opens directly within the in-app Stage (`WebContentsView`) with zero lag on macOS, Windows, and Linux.

### 🖥️ Sun OS Overlay Mode
- **Trapped Keyboard Navigation**: `Ctrl+Tab` and `Alt+Tab` cycle through Sun Launcher stages instead of switching to host OS windows.
- **Session Control**: Includes a dedicated **"Log out / Exit Sun OS"** button in Settings to cleanly return to your host desktop.

---

## 🎯 Core Experience & Modes

Sun organizes your desktop experience into focused, purposeful mindsets:

- **⌘ Productivity**: Deep work, code editors, writing tools, and conversational AI agents.
- **◉ Entertainment**: Movies, video streaming, podcasts, and personal media.
- **✧ Games**: Cloud gaming and digital game stores.
- **⌥ Tools**: System utilities, Spaces, and Clipboard manager.

### Sandboxed Stage Workspace
- **Side Stage Rail & Overview**: Quickly switch between active stages (`Ctrl/Cmd + E`).
- **Memory Optimization**: Automatically unloads inactive background views after 30 seconds or when the two-view budget is reached.
- **Isolated Sandboxing**: Every embedded web application runs inside isolated `WebContentsView` instances with sandboxed permissions.

---

## 🔒 Security & Privacy Boundary

- **SafeBuild Compliance**: Packaged following [hemanth-reddy18/safebuild-skill](https://github.com/hemanth-reddy18/safebuild-skill) recommendations.
- **Zero Telemetry**: Sun contains no user surveillance, telemetry beacons, background analytics, or third-party tracking scripts.
- **Sandboxed Execution**: Third-party websites run within sandboxed Chromium views without Node.js integration or private context exposure.
- **Verified Updates**: Downloaded updates are checked against SHA-256 metadata published on GitHub releases.
- **Source Disclosure**: The application source code is proprietary and privately hosted. This public repository hosts official binary distributions, verification metadata, and [component notices](THIRD-PARTY).

---

## 📄 License & Notices

Proprietary — All rights reserved. Maintained by [hemanth-reddy18](https://github.com/hemanth-reddy18).
For third-party dependencies, open-source licenses, and notices, see [THIRD-PARTY](THIRD-PARTY).
