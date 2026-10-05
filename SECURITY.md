# Security and responsible reporting

[← TapDeck](README.md) · [Privacy](PRIVACY.md) · [Ordinary support](SUPPORT.md)

## Report a vulnerability privately

Use [GitHub private vulnerability reporting](https://github.com/wakeupbrk/TapDeck/security/advisories/new). Include the affected preview version, a clear description and reproduction steps using test-only data.

Do not post active QR invitations, pairing secrets, personal decks, hardware identifiers or provider credentials in public issues. Report ordinary setup problems through [Support](SUPPORT.md).

## Current preview

Use the **0.3.7** Mac preview with the hosted controller. A 0.3.2 Mac app still connects. Builds earlier than 0.3.2 cannot reconnect after the security handshake update. The [changelog](docs/CHANGELOG.md) describes the fixes and upgrade steps.

New browsers require local Mac approval; approved messages use authenticated encryption, replay rejection and revocation. The Mac owns executable definitions and the phone requests configured action IDs. These controls have limitations: endpoint devices and the hosting/deployment account remain trusted.

The download is ad hoc signed and unnotarized and has not received an independent security audit. Automated checks are not proof that no vulnerabilities exist. An independent review and remaining release acceptance checks are planned before wider production distribution.

## If a device is lost or no longer trusted

Revoke its browser in Mac settings. Never share a pairing invitation. Clearing browser storage alone is not a replacement for revocation on the Mac.
