# Frequently asked questions

[← TapDeck](../README.md) · [Get started](GETTING-STARTED.md) · [Get help](../SUPPORT.md)

## Which release file should I download?

| File | Purpose |
| --- | --- |
| **TapDeck-0.3.7-Mac.dmg** | The Mac app installer. Download this to use TapDeck. |
| **SHA256SUMS.txt** | The installer’s SHA-256 fingerprint. Use it to check your downloaded file matches the published build. |
| **LICENSE-TRIAL.txt** | The preview’s usage terms, in plain text. |
| **THIRD-PARTY-NOTICES.txt** | Applicable browser-library notices. |
| **Source code (zip / tar.gz)** | GitHub’s automatic archives of this public repository. They contain documentation and images, not the private app development source. Both formats contain the same repository files. |

A `.txt` file is a text document; it does not install the app. [How to verify the checksum](TROUBLESHOOTING.md#verify-the-download).

## Do I install anything on my phone?

No. Scan the Mac’s QR and use your phone browser. You can optionally add the controller to your Home Screen. There is no native phone app in this edition.

## Must both devices use the same Wi-Fi?

No. Both need internet access. The Mac must be awake with TapDeck running and an active verified trial.

## Do I need an account?

No TapDeck account or email registration is required. The preview asks for trial-activation consent and retains an app-specific hardware hash. [Privacy details](../PRIVACY.md).

## Does reinstalling reset the trial?

No. The trial starts at first activation and lasts seven consecutive days. The service retains the original activation and expiry for the same Mac. Downloading again, clearing local data or changing macOS users does not restart it. Your saved deck remains exportable after expiry.

## Can I purchase a license?

Not yet. Pricing, payments and paid activation remain future work. The current download is a preview under its [trial-use notice](../LICENSE-TRIAL.txt).

## Why do older Mac versions fail to reconnect?

The 0.3.2 security update authenticates a connection before allocating a WebSocket. Builds older than 0.3.2 use the retired handshake. Install the current Mac preview and refresh the phone controller; your original trial expiry is retained. The current 0.3.7 preview adds application window controls and connection fixes without retiring 0.3.2 compatibility. Preview signing changes may require re-pairing and refreshing Accessibility permission.

## Can I drag apps straight into the Mac app?

Yes. Drop an application from Finder onto the deck. That adds a button and does not run it. Websites are added with **Add**. Click a button to edit it, and use **Test** to run it. Website drops and other workspace ideas remain [on the roadmap](ROADMAP.md).

## Is TapDeck open source?

The app development repository is private. This public repository hosts compiled previews, documentation, images and support. Current previews use proprietary trial terms; earlier license grants and third-party licenses remain unaffected.

## Is this ready for a finished production release?

The preview is ad hoc signed and unnotarized. Developer ID signing, notarization, clean-Mac installation, physical Safari/Home Screen acceptance and independent security review remain on the release checklist. See [release status](CHANGELOG.md#current-release-status).

## How do I revoke a phone?

Revoke its browser in Mac settings. **Forget this Mac** on the phone clears its local pairing and artwork; revoke on the Mac as well to invalidate its access. Never share a pairing QR or invitation URL.
