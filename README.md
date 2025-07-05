# Atmo Cursors

[<img src="svg/hand2.svg" width="100" alt="Atmo Cursors">](https://syndromatic.com)

**The SynOS defacto cursor library**

Inspired by classic Mac OS X cursors and thoughtfully reimagined with the classy elegance of the **Atmo** design language, *Atmo Cursors* offers a refined, high-DPI cursor set tailored exclusively for the SynOS desktop experience.

Tested on **SynOS Canora Beta 1**

---

## Installation

As of now, Atmo Cursors does not have a packaged release, and as such is largely the same as the original Apple_cursor project. You’ll need to build and install it manually:

### 🔧 Prerequisites

- **Python 3.7+**
- [`clickgen`](https://github.com/ful1e5/clickgen) (for cursor generation)
- [`yarn`](https://classic.yarnpkg.com/lang/en/) (for dependency management)
- [`cbmp`](https://github.com/ful1e5/cbmp) (for color customisation)

### 🛠️ Building

```bash
git clone https://github.com/phenom64/Atmo-Cursors.git
cd Atmo-Cursors
yarn install
yarn generate
```

This will build the cursor theme in the themes/ directory.

### 📦 Installing to SynOS

```bash
# Local install (user-only)
mkdir -p ~/.icons
cp -r themes/Atmo* ~/.icons/

# System-wide install (requires sudo)
sudo cp -r themes/Atmo* /usr/share/icons/
```

To apply the cursor theme:

- Open System Preferences → Appearance → Cursors
- Select Atmo Cursors
- Log out and back in for full effect

### Features

- HiDPI support with crisp SVG-to-bitmap rendering
- Mac-inspired cursor forms, reinterpreted in the Atmo visual style
- Seamless integration with KDE Plasma (SynOS default)

### Credits
- Based on apple_cursor by @ful1e5
- Special thanks to the open-source cursor tooling ecosystem: clickgen, cbmp, ctgen

---

TM & © 2025 Syndromatic Ltd — Crafted with ❤️ for SynOS
