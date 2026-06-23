# Pearl Wallet Android — Public Release Artifacts

Signed APKs, AABs, and native debug symbols for [Pearl Wallet Android](https://pearl-wallet-showcase.netlify.app).

## Download

Browse the [Releases](https://github.com/rebots-online/pearl-wallet-releases/releases) page and download the `release-signed.apk` file from the latest release.

## Install

1. Download the `.apk` file on your Android device
2. Allow "Install from unknown sources" if prompted
3. Open the file and install
4. If upgrading from a debug/dev build, uninstall first — release builds use a different signing key

## Verify

Each release includes a SHA-256 hash. Verify before installing:

```bash
sha256sum pearl-wallet-android-v*.*.*-release-signed.apk
# Compare with the hash shown on the release page
```

## Signing key

All release builds are signed with:
```
CN=PRL Wallet Upload, O=Robin L M Cheung MBA, C=CA
```

## Current status

**Tester builds** — not yet confirmed as the first fully working wallet release. Do not use for meaningful funds.

## Links

- **Landing page**: https://pearl-wallet-showcase.netlify.app
- **Vercel mirror**: https://pearl-wallet-showcase.vercel.app
- **Explorer**: https://explorer.pearlchain.org
- **OTC Market**: https://lordofpearls.xyz

## FAQ

**What is Pearl Wallet?**
A noncustodial Android wallet for the Pearl blockchain. Monitor mining rigs, send/receive PRL, and check live OTC rates.

**Why is the source code not public?**
The source repo is private during development. This public repo hosts only the signed release binaries.

**Is it safe?**
Tester builds are signed but not yet confirmed working. Always verify the SHA-256 hash before installing. Do not use with meaningful funds until a release is marked production-ready.

**What permissions does the app request?**
- Internet (network access)
- Camera (QR code scanning)
- Biometric (fingerprint unlock)
- Vibrate (notifications)
- Battery optimization exemption (keeps sync alive in background)
- Foreground service (sync notification)
- Boot completed (resume sync on restart)

**How do I import my wallet?**
Use the 12-word recovery phrase. The app supports camera OCR for seed import — point your camera at the words, no typing needed.

**How do home screen widgets work?**
Long-press your home screen → Add widget → Pearl Wallet. Two sizes available: a compact wallet widget (balance + price) and a full miner stats widget. Tap the widget to open the Receive/QR screen.
