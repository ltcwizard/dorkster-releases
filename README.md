# Dorkster: downloads

Dorkster sends files between our own computers. This page only has the
ready-to-run downloads. Get the newest one from
**[Releases](https://github.com/ltcwizard/dorkster-releases/releases/latest)**.

## Windows 10 / 11
1. Download `Dorkster-vX.Y.Z-windows-x64-setup.exe`.
2. Double-click it and click through the installer. It doesn't need an admin
   password. Dorkster then shows up in the Start menu (and on the desktop if
   you ticked that box).
3. **"Windows protected your PC"?** The app isn't signed by a big company, so
   Windows warns about it. Click **More info** → **Run anyway**.
4. When Windows Firewall asks, allow **Private networks**.

To remove it: **Settings → Apps → Installed apps → Dorkster → Uninstall**.

<details>
<summary>No-install option (zip)</summary>

1. Download `Dorkster-vX.Y.Z-windows-x64.zip`.
2. Right-click it → **Extract All…** (put it somewhere like `Documents\Dorkster`).
3. Open the extracted `Dorkster` folder and double-click **`Dorkster.exe`**.
   Keep the whole folder together; the `.exe` needs the `_internal` folder next to it.
</details>

## Linux Mint 22 / Ubuntu 24.04
One-time setup (installs the web view Dorkster's window uses):
```bash
sudo apt install gir1.2-webkit2-4.1
```
Then:
1. Download `Dorkster-vX.Y.Z-linux-x86_64.tar.gz`.
2. Right-click it → **Extract Here**.
3. Open the `Dorkster` folder and double-click **`Dorkster`** (or run `./Dorkster`
   in a terminal from that folder).

## Updating
Windows: run the new `…-setup.exe`. It replaces the old version (and closes
Dorkster first if it's open). Zip/Linux: replace the old `Dorkster` folder.
Your settings, paired laptops and shared folders are stored separately, so they stay.

## Checking a download (optional)
Each release has `SHA256SUMS.txt`. To confirm a file downloaded correctly:
- Windows (PowerShell): `Get-FileHash .\Dorkster-vX.Y.Z-windows-x64-setup.exe`
- Linux: `sha256sum Dorkster-vX.Y.Z-linux-x86_64.tar.gz`

The value should match the line for that file.
