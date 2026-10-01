# TapDeck

**Your Mac. One tap away.**

A native Mac app with a large control deck in your phone's browser. Scan the Mac's QR, approve the browser once, then return to the same saved controller to reconnect.

[Download the Mac preview](https://github.com/wakeupbrk/TapDeck-Downloads/releases/tag/v0.2.0-preview.1) · [Browser controller](https://tapdeck-connect.pages.dev)

![TapDeck on Mac](images/mac-deck.png)

## Install the preview

1. Download **TapDeck-0.2.0-Mac.dmg** from Releases.
2. Open it and drag TapDeck to Applications. Keep one installed copy.
3. Open TapDeck, choose the phone button and scan its QR with your phone's Camera.
4. Open the link and approve the browser on your Mac. Optionally add the page to your Home Screen.

Both devices need internet access. The Mac must be awake with TapDeck running. macOS 14 or newer is required; Apple silicon and Intel are supported. No phone app, account registration or domain purchase is needed. Opening the bare controller address explains pairing; use the Mac's QR to connect.

**Preview status:** this build is ad hoc signed and is not Apple Developer ID signed or notarized. Gatekeeper may block it. It is offered for testing, not as a finished paid product. Physical iPhone Safari/Home Screen acceptance testing also remains before production launch.

## Make it yours

The starter deck includes Finder, Safari, Notes, Calendar, Mail, Music, Reminders and Settings. Customize apps, websites, keyboard commands, Shortcuts, icons, colors and pages from the Mac. The phone shows fixed pages of large icon buttons with a compact side menu. Keyboard actions need Accessibility permission on the Mac.

![Phone browser in landscape](images/browser-landscape.png)

## Security and privacy

A new browser requires an expiring invitation and local Mac approval. Messages use authenticated encryption. Revoke browsers in Mac settings when needed. Do not share pairing QR codes or invitation URLs. No analytics SDK is included; the Cloudflare hosting provider processes connection metadata. No claim of zero vulnerabilities is made.

Use [private vulnerability reporting](https://github.com/wakeupbrk/TapDeck-Downloads/security/advisories/new) for security issues. Never include active pairing credentials or private deck data in public issues.

## Downloads and licensing

This repository contains only downloads, screenshots and instructions. App development source is private and is not uploaded here. GitHub's automatic source ZIP contains only this repository's documentation and images.

The already-published 0.2.0 preview retains its [original MIT license](LICENSE-MIT-preview.txt). Future paid versions may have different terms, supplied with those versions. Payment and activation have not been implemented yet. Restricting source access does not withdraw prior MIT permissions or prevent every form of reverse engineering.

Verify the DMG with the SHA256SUMS.txt asset in the release. Do not substitute an unofficial download.
