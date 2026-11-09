# Amar Bangla Kotha (আমার বাংলা কথা) — Documentation

<p align="center">
  <img src="assets/logo_bangla.svg" alt="Amar Bangla Kotha Logo" width="220" />
  <br>
  <strong>A Next-Generation, High-Performance, Cross-Platform Bengali Typing Engine & GUI</strong>
</p>

<p align="center">
  <a href="https://github.com/MehediHasanSumon/amar-bangla-kotha-docs/releases"><img src="https://img.shields.io/badge/Release-v1.0.0-blue.svg?style=for-the-badge" alt="Release v1.0.0" /></a>
  <a href="DOWNLOADS.md"><img src="https://img.shields.io/badge/Platform-Linux%20%7C%20Windows%20%7C%20macOS-green.svg?style=for-the-badge" alt="Platforms" /></a>
  <a href="docs/BENCHMARK.md"><img src="https://img.shields.io/badge/Accuracy-97.2%25%20Top--1%20%7C%2098.1%25%20Top--3-brightgreen.svg?style=for-the-badge" alt="Accuracy" /></a>
  <a href="https://github.com/MehediHasanSumon/amar-bangla-kotha"><img src="https://img.shields.io/badge/License-MIT-orange.svg?style=for-the-badge" alt="License" /></a>
</p>

---

## ⚡ Direct Downloads (Version 1.0.0)

| OS | Package | Format | Direct Download Link |
| :--- | :--- | :--- | :--- |
| **Linux (Ubuntu / Debian / Mint)** | Debian Package | `.deb` | [⬇️ **Download .deb**](https://github.com/MehediHasanSumon/amar-bangla-kotha-docs/releases/download/v1.0.0/amar-bangla-kotha_1.0.0_amd64.deb) |
| **Linux (Generic / All Distros)** | Portable Archive | `.tar.gz` | [⬇️ **Download .tar.gz**](https://github.com/MehediHasanSumon/amar-bangla-kotha-docs/releases/download/v1.0.0/amar-bangla-kotha_1.0.0_linux_x86_64.tar.gz) |
| **Windows 10 / 11** | Full Installer | `.exe` | [⬇️ **Download Windows Installer**](https://github.com/MehediHasanSumon/amar-bangla-kotha-docs/releases/download/v1.0.0/AmarBanglaKotha-Setup-1.0.0.exe) |
| **macOS** | Installer Package | `.pkg` | [⬇️ **Download macOS Package**](https://github.com/MehediHasanSumon/amar-bangla-kotha-docs/releases/download/v1.0.0/AmarBanglaKotha-1.0.0.pkg) |

👉 *For detailed checksums, dependencies, and step-by-step setup guides, read the [📥 Downloads Guide (DOWNLOADS.md)](DOWNLOADS.md).*

---

## 🌟 Key Features

1. **State-of-the-Art Phonetic Accuracy**:
   - **97.2% Top-1 Accuracy** and **98.1% Top-3 Accuracy** against rigorous standardized Golden Corpora.
   - Handles complex conjuncts (*যুক্তবর্ণ*), phonological edge cases, and natural colloquial spelling variations.
2. **Lightning-Fast Core Engine**:
   - Written in modern **C++17** with zero external runtime dependencies.
   - Sub-microsecond transliteration latency using prefix-tree (Trie) caching and bigram frequency probability ranking.
3. **Cross-Platform Input Architecture**:
   - **Linux**: Avro-style floating topbar GUI (GTK3 / PyGObject), native IBus engine daemon, and Wayland compatibility.
   - **Windows**: Native Text Services Framework (TSF) Input Method COM DLL (`abk_tsf.dll`) and 64-bit installer.
   - **macOS**: Native InputMethodKit Input Method Engine.
4. **Intelligent Typing & Autocorrect**:
   - Dynamic real-time suggestion candidate box with Tab/Number browsing.
   - Autocorrect with typo-recovery and personalized adaptive dictionary.
5. **Bangladesh Localization Helpers**:
   - Built-in shortcuts for Bengali Taka symbol (৳), English-to-Bangla date formatting, number converters, and administrative terms.
6. **Domain-Specific Vocabulary**:
   - Pre-loaded domain packs for **Medical**, **Legal**, **Administrative**, and **Literature/Poetry**.
7. **Legacy ASCII / Bijoy Conversion**:
   - Full bi-directional converter for legacy ANSI (Bijoy) and modern Unicode text, complete with automatic clipboard monitoring.

---

## ⌨️ Phonetic Typing Quick Reference (Avro-Compatible)

| English Input | Bengali Output | Example Input | Example Output |
| :--- | :--- | :--- | :--- |
| `k`, `kh`, `g`, `gh`, `Ng` | ক, খ, গ, ঘ, ঙ | `kotha` | কথা |
| `c`, `ch`, `j`, `jh`, `NG` | চ, ছ, জ, ঝ, ঞ | `amar` | আমার |
| `T`, `Th`, `D`, `Dh`, `N` | ট, ঠ, ড, ঢ, ণ | `bangla` | বাংলা |
| `t`, `th`, `d`, `dh`, `n` | ত, থ, দ, ধ, ন | `dhonnobad` | ধন্যবাদ |
| `p`, `ph`/`f`, `b`, `bh`/`v`, `m` | প, ফ, ব, ভ, ম | `bhalobasha` | ভালোবাসা |
| `z`, `r`, `l`, `sh`, `S`/`Sh`, `s`, `h` | য, র, ল, শ, ষ, স, হ | `shundor` | সুন্দর |
| `R`, `Rh`, `y` | ড়, ঢ়, য় | `gari` | গাড়ি |
| `t`` | ৎ (খণ্ড-ত) | `hot` | হঠাৎ |
| `k+k`, `k+S`, `b+r` | ক্ক, ক্ষ, ব্র | `kkhoma` | ক্ষমা |

---

## 📚 Complete Documentation Index

| Documentation Topic | Description | Link |
| :--- | :--- | :--- |
| **Download & Install** | Cross-platform downloads, hashes, and setup steps | [DOWNLOADS.md](DOWNLOADS.md) |
| **Phonetic Keymap** | Comprehensive key mappings and rules for all Bengali characters | [docs/KEYMAP.md](docs/KEYMAP.md) |
| **Core Architecture** | C++17 engine internals, transliteration pipeline, memory layout | [docs/ARCHITECTURE.md](docs/ARCHITECTURE.md) |
| **Cross-Platform Guide** | Deep-dive into Linux IBus, Windows TSF, and macOS IMK | [docs/CROSS_PLATFORM.md](docs/CROSS_PLATFORM.md) |
| **Packaging & CI/CD** | Specifications for `.deb`, `.tar.gz`, Inno Setup, `.pkg`, and GitHub Actions | [docs/PACKAGING.md](docs/PACKAGING.md) |
| **Benchmark & Accuracy** | Accuracy metrics (97.2%), microsecond timing, test methodology | [docs/BENCHMARK.md](docs/BENCHMARK.md) |
| **Wayland & Linux GUI** | Floating topbar window positioning, Wayland protocol nuances | [docs/WAYLAND.md](docs/WAYLAND.md) |
| **Accessibility** | AT-SPI2 screen reader compliance and keyboard-only navigation | [docs/ACCESSIBILITY.md](docs/ACCESSIBILITY.md) |
| **Bangladesh Helpers** | Taka symbol shortcuts, date converters, and number formatting | [docs/BANGLADESH_HELPERS.md](docs/BANGLADESH_HELPERS.md) |
| **Quality of Life (QoL)** | Autocorrect, suggestion navigation, undo typing, and backspace behavior | [docs/QUALITY_OF_LIFE.md](docs/QUALITY_OF_LIFE.md) |
| **Legacy Bijoy Converter** | Bi-directional ANSI (Bijoy) <-> Unicode converter and clipboard tool | [docs/LEGACY_FONTS.md](docs/LEGACY_FONTS.md) |
| **Personalization** | Dynamic dictionary, learning frequent phrases, user preferences | [docs/PERSONALIZATION.md](docs/PERSONALIZATION.md) |
| **Settings & Config** | Configuration options, TOML file format, and settings GUI | [docs/SETTINGS.md](docs/SETTINGS.md) |
| **Testing & Sanity** | Catch2 unit tests, fuzz testing, AddressSanitizer (ASan/UBSan) | [docs/TESTING.md](docs/TESTING.md) |
| **Backspace & Editing** | Nuances of deleting Bengali compound characters and vowels | [docs/BACKSPACE.md](docs/BACKSPACE.md) |
| **Code Signing** | Security, Authenticode (Windows), and Notarization (macOS) | [docs/CODE_SIGNING.md](docs/CODE_SIGNING.md) |
| **Cleanroom Provenance** | Cleanroom design compliance, licensing, and cleanroom verification | [docs/PROVENANCE.md](docs/PROVENANCE.md) |

---

## 🛠️ Building From Source

### Linux (Debian / Ubuntu / Fedora)

```bash
# Clone the repository
git clone https://github.com/MehediHasanSumon/amar-bangla-kotha.git
cd amar-bangla-kotha

# Build engine, CLI, and run tests
make all
make test

# Build Debian .deb or Portable .tar.gz package
make package-deb
make package-tar

# Run GUI
python3 gui/app.py
```

### Windows (MSVC 2022)

```cmd
cmake -B build -A x64
cmake --build build --config Release
.\build\Release\abk_tests.exe
```

### macOS (Clang / CMake)

```bash
cmake -B build -DCMAKE_BUILD_TYPE=Release
cmake --build build
ctest --test-dir build --output-on-failure
```

---

## 📄 License

This project is licensed under the [MIT License](https://github.com/MehediHasanSumon/amar-bangla-kotha/blob/main/LICENSE).  
Developed with ❤️ for the Bengali computing community.
