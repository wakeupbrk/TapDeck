# Changelog

[← TapDeck](../README.md) · [Download releases](https://github.com/wakeupbrk/TapDeck/releases) · [Roadmap](ROADMAP.md)

## 0.3.2 — security preview

[Download and release details](https://github.com/wakeupbrk/TapDeck/releases/tag/v0.3.2-security.1)

- Deleted controls no longer authorize their old remote action IDs. Relevant configuration changes cancel affected queued or running work.
- The relay verifies credentials before allocating a connection, using short-lived, single-use admission tickets.
- Bounded request handling prevents incomplete request bodies from blocking an active room’s processing.
- Added action-authorization, cancellation and relay regressions. Local and synthetic live encrypted connection checks passed.

**Upgrade:** install the matching 0.3.2 Mac preview and refresh browser/Home Screen tabs. Older Mac builds cannot reconnect to the updated relay. Saved pairing and original seven-day trial timestamps remain compatible.

## 0.3.1 — trial packaging

- Updated current preview packaging to the proprietary seven-day trial notice.
- Preserved earlier license grants and third-party licenses.
- Trial behavior remained unchanged.

## 0.3.0 — seven-day trial preview

- Added explicit activation and one server-backed seven-day trial per Mac.
- Reinstalling retains the original expiry.
- Online verification locks controls when access cannot be confirmed; saved decks remain exportable after expiry.

## 0.2.0 — consumer preview

- Native Mac app with browser-only phone control and a generic starter deck.
- Mac customization, large phone buttons, fixed pages and a compact browser menu.
- Scan-and-approve pairing, remembered reconnect and revocation.

## Current release status

The latest download remains a **preview**: ad hoc signed and unnotarized, with paid licenses unavailable. Developer ID signing, notarization, clean-Mac installation, physical Safari/Home Screen acceptance and independent security review remain before wider production distribution.

Passing automated checks and a point-in-time dependency audit do not establish that the app is vulnerability-free. Releases preserve permanent trial records and applicable earlier/third-party license grants.
