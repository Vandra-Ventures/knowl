# Knowl

Download the latest release from the [Releases](https://github.com/Vandra-Ventures/knowl/releases) page.

## Installation (macOS)

The app isn't notarized yet, so you need to run these commands in Terminal after downloading.

### Option 1: One-liner (recommended)

Copy and paste this into Terminal:

```bash
# For Apple Silicon (M1/M2/M3)
cd /tmp && curl -L -o Knowl.zip "https://github.com/Vandra-Ventures/knowl/releases/latest/download/Knowl-0.1.0-arm64-mac.zip" && unzip -o Knowl.zip && xattr -cr Knowl.app && codesign --force --deep --sign - Knowl.app && mv Knowl.app /Applications/ && rm Knowl.zip && open /Applications/Knowl.app
```

```bash
# For Intel Macs
cd /tmp && curl -L -o Knowl.zip "https://github.com/Vandra-Ventures/knowl/releases/latest/download/Knowl-0.1.0-mac.zip" && unzip -o Knowl.zip && xattr -cr Knowl.app && codesign --force --deep --sign - Knowl.app && mv Knowl.app /Applications/ && rm Knowl.zip && open /Applications/Knowl.app
```

### Option 2: If you already downloaded from browser

If you downloaded the ZIP from your browser to Downloads:

```bash
rm -rf /tmp/Knowl.app
unzip -o ~/Downloads/Knowl-*-mac.zip -d /tmp/
xattr -cr /tmp/Knowl.app
codesign --force --deep --sign - /tmp/Knowl.app
mv /tmp/Knowl.app /Applications/
open /Applications/Knowl.app
```

> **Note:** We're working on proper code signing. This manual step will go away in a future release.
