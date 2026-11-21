# Dorkster: downloads

Dorkster sends files between our own computers. This page only has the
ready-to-run downloads. Get the newest one from
**[Releases](https://github.com/ltcwizard/dorkster-releases/releases/latest)**.

## Windows 10 / 11
1. Download `Dorkster-vX.Y.Z-windows-x64.zip`.
2. Right-click it → **Extract All…** (put it somewhere like `Documents\Dorkster`).
3. Open the extracted `Dorkster` folder and double-click **`Dorkster.exe`**.
   Keep the whole folder together; the `.exe` needs the `_internal` folder next to it.
4. **"Windows protected your PC"?** The app isn't signed by a big company, so
   Windows warns about it. Click **More info** → **Run anyway**.
5. When Windows Firewall asks, allow **Private networks**.

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
Download the new version and replace the old `Dorkster` folder.
Your settings, paired laptops and shared folders are stored separately, so they stay.

## Checking a download (optional)
Each release has `SHA256SUMS.txt`. To confirm a file downloaded correctly:
- Windows (PowerShell): `Get-FileHash .\Dorkster-vX.Y.Z-windows-x64.zip`
- Linux: `sha256sum Dorkster-vX.Y.Z-linux-x86_64.tar.gz`

The value should match the line for that file.
