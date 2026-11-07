# GTA V Lite 🎮

A lightweight, borderless desktop application wrapper for playing GTA 5 in your browser, packaged into a single Windows installer.

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Platform](https://img.shields.io/badge/platform-Windows%20x64-lightgrey.svg)

> **⚠️ Disclaimer:** This project is an unofficial third-party web wrapper and is not affiliated with, endorsed by, or connected to Rockstar Games or Take-Two Interactive.

---

## ✨ Features

- **Only 360MB:** Everything comes from [Play GTA V.com](https://playgta5.com/) so nothing is stored on your PC except for your save files and the 360MB needed to run the game.
- **Instant startup:** Starts up in under a second without needing a launcher, the game itself does take 1-2 minutes to load.
- **FPS counter:** Press = to view your fps in the top left corner.

---

## 🚀 Installation

1. Go to the [Releases](https://github.com/matsdepe-rgb/gta5-lite/releases) page.
2. Download the latest installer (`gtavlite-setup-64x.exe`).
3. Run the installer and follow the setup wizard.
4. Launch **GTA V Lite** from your Desktop or Start Menu!

---

## 🛠️ Building from Source

If you want to package the application yourself from scratch:

### Prerequisites

- [Node.js](https://nodejs.org/) (v16 or higher)
- [Inno Setup 7](https://jrsoftware.org/isdl.php)

### 1. Build the Desktop App Bundle

Open PowerShell or your terminal and run Nativefier to create the standalone Electron wrapper:

```bash
npx nativefier --name "GTA 5 Lite" --full-screen "https://playgta5.com"
```

This generates a folder named `GTA 5 Lite-win32-x64` on your Desktop.

### 2. Build the Windows Installer

1. Clone this repository:
   ```bash
   git clone https://github.com/matsdepe-rgb/gta5-lite.git
   cd gta5-lite
   ```
2. Open `gtavlite.iss` in **Inno Setup Compiler**.
3. Press `Ctrl + F9` to compile the setup script.
4. The final installer `.exe` will be saved to your `Downloads\Output` directory.

---

## 📄 License

This repository contains setup scripts and build configurations released under the [MIT License](LICENSE). All game media and web assets belong to their respective copyright holders.
