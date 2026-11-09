# 📥 Downloads & Installation — Amar Bangla Kotha (আমার বাংলা কথা)

Welcome to the official download page for **Amar Bangla Kotha** (v1.0.0).  
Select your operating system below to download the latest production release package.

---

## 🚀 Quick Download Matrix (Version 1.0.0)

| Operating System | Package Type | Architecture | Download Link | File Size | SHA256 Checksum |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **Linux (Ubuntu / Debian / Mint)** | `.deb` package | `x86_64 / amd64` | [📥 Download .deb](https://github.com/MehediHasanSumon/amar-bangla-kotha-docs/releases/download/v1.0.0/amar-bangla-kotha_1.0.0_amd64.deb) | ~451 KB | `2706a8d30933acf48bc84881571baac597102b5da43053eefe7eaedb9bf22966` |
| **Linux (Generic / Portable)** | `.tar.gz` archive | `x86_64` | [📥 Download .tar.gz](https://github.com/MehediHasanSumon/amar-bangla-kotha-docs/releases/download/v1.0.0/amar-bangla-kotha_1.0.0_linux_x86_64.tar.gz) | ~1.55 MB | `0a38588f3a31823a0c52aa71e29ea3fb61cccb1357abc8265b8b8bfe3629d662` |
| **Windows 10 / 11** | Inno Setup `.exe` | `x64` | [📥 Download .exe](https://github.com/MehediHasanSumon/amar-bangla-kotha-docs/releases/download/v1.0.0/AmarBanglaKotha-Setup-1.0.0.exe) | 2.24 MB | `deec554918f201cdc049d8d7b6a022ac00869dba0ad0d89ccdc72a83e51f0f4f` |
| **macOS (Sonoma / Ventura / Monterey)** | Native `.pkg` | `Universal / arm64 / x86_64` | [📥 Download .pkg](https://github.com/MehediHasanSumon/amar-bangla-kotha-docs/releases/download/v1.0.0/AmarBanglaKotha-1.0.0.pkg) | Package | 29 KB |

> 🔗 **All Releases on GitHub**: [github.com/MehediHasanSumon/amar-bangla-kotha-docs/releases](https://github.com/MehediHasanSumon/amar-bangla-kotha-docs/releases)

---

## 🐧 Linux Installation Guide

### Option 1: Debian/Ubuntu `.deb` Package (Recommended for Ubuntu/Debian/Pop!_OS/Mint)

1. **Download the `.deb` file**:
   ```bash
   wget https://github.com/MehediHasanSumon/amar-bangla-kotha-docs/releases/download/v1.0.0/amar-bangla-kotha_1.0.0_amd64.deb
   ```

2. **Install using `apt` or `dpkg`**:
   ```bash
   sudo apt install ./amar-bangla-kotha_1.0.0_amd64.deb
   ```
   *Note: `apt install` will automatically resolve dependencies (such as `python3-gi`, `python3-gi-cairo`, `gir1.2-gtk-3.0`).*

3. **Launch the Application**:
   - Search for **"Amar Bangla Kotha"** in your application launcher / desktop app grid.
   - Or run from terminal:
     ```bash
     amar-bangla-kotha
     ```
   - For IBus system integration:
     - Open **Settings** → **Keyboard** → **Input Sources**.
     - Click **+** and select **Bangla** → **Amar Bangla Kotha (আমার বাংলা কথা)**.

---

### Option 2: Portable Linux Archive (`.tar.gz`) — No Root Required

Ideal for users without sudo/root access or users on Arch Linux, Fedora, openSUSE, etc.

1. **Download and Extract**:
   ```bash
   wget https://github.com/MehediHasanSumon/amar-bangla-kotha-docs/releases/download/v1.0.0/amar-bangla-kotha_1.0.0_linux_x86_64.tar.gz
   tar -xzf amar-bangla-kotha_1.0.0_linux_x86_64.tar.gz
   cd amar-bangla-kotha_1.0.0_linux_x86_64
   ```

2. **Run Immediately without Installation**:
   - **Launch Avro-style GUI Bar**:
     ```bash
     ./run_gui.sh
     ```
   - **Launch CLI Interactive Translator**:
     ```bash
     ./run_cli.sh
     ```

3. **Install to Local User (`~/.local`)**:
   ```bash
   ./install_user.sh
   ```

---

## 🪟 Windows Installation Guide

### Windows 10 & Windows 11 (64-bit)

1. **Download `AmarBanglaKotha-Setup-1.0.0.exe`**.
2. **Run the Installer**:
   - Double click the `.exe` file.
   - Follow the wizard instructions. The installer will automatically register the native Text Services Framework (TSF) Input Method COM DLL (`abk_tsf.dll`).
3. **Switch Input Language**:
   - Press <kbd>Win</kbd> + <kbd>Space</kbd> to switch between English and **Amar Bangla Kotha**.
   - Or click on the language bar on the taskbar.
   - Press <kbd>F12</kbd> anytime to toggle Bengali phonetic mode on/off.

---

## 🍏 macOS Installation Guide

### macOS Ventura, Sonoma & Monterey

1. **Download `AmarBanglaKotha-1.0.0.pkg`**.
2. **Run the Installer**:
   - Double click the `.pkg` package.
   - Complete the installation steps. The input method engine will be installed into `/Library/Input Methods/AmarBanglaKotha.app`.
3. **Enable Input Source**:
   - Open **System Settings** → **Keyboard** → **Text Input** → **Input Sources** → **Edit...**.
   - Click **+** (Add), scroll to **Bengali**, and select **Amar Bangla Kotha**.
4. **Switch Keyboard**:
   - Press <kbd>Ctrl</kbd> + <kbd>Space</kbd> or click the input switcher icon in the menu bar.

---

## 🔒 Verification & Security

To verify the integrity of downloaded Linux packages, run:
```bash
sha256sum -c <<EOF
2706a8d30933acf48bc84881571baac597102b5da43053eefe7eaedb9bf22966  amar-bangla-kotha_1.0.0_amd64.deb
0a38588f3a31823a0c52aa71e29ea3fb61cccb1357abc8265b8b8bfe3629d662  amar-bangla-kotha_1.0.0_linux_x86_64.tar.gz
EOF
```

---

## ❓ Need Help?
- Check our [Phonetic Keymap Guide](docs/KEYMAP.md) for how to type in Bengali.
- Check [Architecture & Core Engine](docs/ARCHITECTURE.md) to understand how it works.
- Report any issues or feature requests on the [GitHub Issues tracker](https://github.com/MehediHasanSumon/amar-bangla-kotha-docs/issues).
