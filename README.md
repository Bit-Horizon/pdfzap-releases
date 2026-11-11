# PDFZap releases

Signed installers for [PDFZap](https://pdfzap.com), the desktop app that reads receipts, invoices and bank
statements into spreadsheets, entirely on your computer.

**Download from [pdfzap.com/download](https://pdfzap.com/download)**, or pick a version under
[Releases](https://github.com/Bit-Horizon/pdfzap-releases/releases). Each release has:

| File | What |
|---|---|
| `PDFZap_<version>_aarch64.dmg` | macOS (Apple Silicon, macOS 13 or later). Signed with Developer ID and notarised by Apple. |
| `PDFZap_<version>_x64-setup.exe`, `.msi` | Windows 10 (22H2) or 11, 64-bit, when available |
| `SHA256SUMS.txt` | Checksums for the files above |
| `latest.json` | The update information the app reads from pdfzap.com/updates/latest.json |
| `THIRD-PARTY-NOTICES.txt` | Licences of the open-source components inside the app |

The app's source code isn't public. This repository only hosts the published builds.

## Check a download

```bash
shasum -a 256 PDFZap_*.dmg            # compare with SHA256SUMS.txt
spctl -a -vvv -t install PDFZap_*.dmg  # "source=Notarized Developer ID", BIT HORIZON - FZCO (H9299XVMSN)
```

## Help

Email [hi@pdfzap.com](mailto:hi@pdfzap.com). PDFZap is made by Bit Horizon FZCO.
