# Knowl

Download the latest release for your platform from the [Releases](https://github.com/Vandra-Ventures/knowl/releases) page.

## Installation (macOS)

1. Download the ZIP file for your Mac:
   - Apple Silicon (M1/M2/M3): `Knowl-*-arm64-mac.zip`
   - Intel: `Knowl-*-mac.zip`

2. Extract the ZIP (double-click it)

3. Open Terminal and run this command:
   ```bash
   xattr -cr ~/Downloads/Knowl.app && codesign --force --deep --sign - ~/Downloads/Knowl.app
   ```

4. Drag Knowl to your Applications folder (optional)

5. Double-click to open!

> **Note:** The app is not yet notarized with Apple, so this manual step is required for now.
