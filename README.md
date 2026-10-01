# TapDeck

**Your Mac. One tap away.**

A native Mac app with a large control deck in your phone's browser. Scan the Mac's QR, approve the browser once, then return to the same saved controller to reconnect.

[Download the 7-day Mac trial](https://github.com/wakeupbrk/TapDeck/releases/tag/v0.3.2-security.1) · [Browser controller](https://tapdeck-connect.pages.dev)

![TapDeck on Mac](images/mac-deck.png)

## Install the preview

1. Download **TapDeck-0.3.2-Mac.dmg** from Releases.
2. Open it and drag TapDeck to Applications. Keep one installed copy.
3. Open TapDeck and choose **Start or resume 7-day trial**.
4. Choose the phone button and scan its QR with your phone's Camera.
5. Open the link and approve the browser on your Mac. Optionally add the page to your Home Screen.

Both devices need internet access. The Mac must be awake with TapDeck running. macOS 14 or newer is required; Apple silicon and Intel are supported. No phone app, account registration or domain purchase is needed. Opening the bare controller address explains pairing; use the Mac's QR to connect.

**Preview status:** this build is ad hoc signed and is not Apple Developer ID signed or notarized. Gatekeeper may block it. It is offered for testing, not as a finished paid product. Physical iPhone Safari/Home Screen acceptance testing also remains before production launch.

## Upgrade to 0.3.2

Install the 0.3.2 Mac preview and refresh your phone browser or Home Screen controller. Older Mac builds cannot reconnect to the updated relay. Saved pairing credentials and the original seven-day trial expiry are preserved. This security update prevents deleted controls from authorizing remote actions and verifies relay credentials before allocating connections.

## Seven days, one Mac

The trial starts when you first activate it, not when you download it. It lasts seven consecutive days. Deleting the app, redownloading, reinstalling or clearing local data on the same Mac does not restart it. After expiry, pairing and controls lock; your saved deck remains available to export. A paid version is not available yet.

Before activation, TapDeck asks permission to send an app-specific hash derived from your Mac’s hardware UUID. The raw hardware UUID is never sent. Our service retains that hash and the original activation/expiry timestamps indefinitely to prevent trial resets. Internet access is required throughout the trial; verification failures lock controls. See [Privacy](PRIVACY.md).

![Seven-day trial activation](images/mac-trial.png)

## Make it yours

The starter deck includes Finder, Safari, Notes, Calendar, Mail, Music, Reminders and Settings. Customize apps, websites, keyboard commands, Shortcuts, icons, colors and pages from the Mac. The phone shows fixed pages of large icon buttons with a compact side menu. Keyboard actions need Accessibility permission on the Mac.

![Phone browser in landscape](images/browser-landscape.png)

## Security and privacy

A new browser requires an expiring invitation and local Mac approval. Messages use authenticated encryption. Revoke browsers in Mac settings when needed. Do not share pairing QR codes or invitation URLs. No analytics SDK is included; the Cloudflare hosting provider processes connection metadata. No claim of zero vulnerabilities is made.

Use [private vulnerability reporting](https://github.com/wakeupbrk/TapDeck/security/advisories/new) for security issues. Never include active pairing credentials or private deck data in public issues.

## Downloads and licensing

This repository contains only downloads, screenshots and instructions. App development source is private and is not uploaded here. GitHub's automatic source ZIP contains only this repository's documentation and images.

The 0.3.2 preview is supplied under the [proprietary seven-day trial notice](LICENSE-TRIAL.txt). Earlier license grants and third-party licenses are unaffected. The old unrestricted preview is no longer offered in public Releases. Previously downloaded copies cannot be recalled or retroactively restricted. Payment and paid licensing are future work. Compiled software is not immune to reverse engineering or deliberate tampering.

Verify the DMG with the SHA256SUMS.txt asset in the release. Do not substitute an unofficial download.
