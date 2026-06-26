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
## FAQ

**What is Pearl Wallet?**
A noncustodial Android wallet for the Pearl blockchain. Monitor mining rigs, send/receive PRL, and check live OTC rates.  Note that the user must accept all  responsibility for use and any potential losses as it is a purely self-custodial wallet and we are not able to retrieve lost or corrupted keys; further, we do not even implement telemetry or analytics of any sort.

**What permissions does the app request?**
- Internet (network access)
- Camera (QR code scanning)
- Biometric (fingerprint unlock)
- Vibrate (notifications)
- Battery optimization exemption (keeps sync alive in background)
- Foreground service (sync notification)
- Boot completed (resume sync on restart)

**How do I import my wallet?**
Use the 12-/24-word recovery phrase. The app supports camera OCR for seed import — point your camera at the words, no typing needed.

**How do home screen widgets work?**
Long-press your home screen → Add widget → Pearl Wallet. Two sizes available: a compact wallet widget (balance + price) and a full miner stats widget. Tap the widget to open the Receive/QR screen.
