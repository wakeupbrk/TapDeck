# Changelog

[← TapDeck](../README.md) · [Download releases](https://github.com/wakeupbrk/TapDeck/releases) · [Roadmap](ROADMAP.md)

## 0.3.7 — application windows and connection stability

[Download and release details](https://github.com/wakeupbrk/TapDeck/releases/tag/v0.3.7)

- Phone application buttons track Mac windows: gray when closed, red when minimized, green when visible. Tap to open, minimize or restore; manual Mac changes synchronize.
- Stable tiles during presses and color changes; Finder opens a window when only its Desktop exists and falls back to opening if window controls are unavailable.
- Delayed failures from old connections no longer stop their replacements. Repeated available-network notifications no longer restart healthy sessions; returning to a stale phone connection starts recovery promptly.
- Automated coverage includes connection races, sustained encrypted heartbeats, network recovery, restart, revocation and rejected keys. Further physical phone/Finder acceptance remains.

**Upgrade:** quit TapDeck, replace the app in Applications, refresh the phone controller, and pair again if requested. Confirm Accessibility permission for keyboard/window controls. Your deck and original trial expiry remain. This is an ad hoc signed, unnotarized preview.

## 0.3.4 — smoother editor and deck recovery

[Download and release details](https://github.com/wakeupbrk/TapDeck/releases/tag/v0.3.4)

- Drag the actual button while neighbours adjust, with no leftover drag copy. Release saves one reorder and one Undo step.
- Review imports before replacement; back up the current deck and referenced artwork before import or restore. Deck History offers local recovery after restart.
- Clearer editor hierarchy, selection marker, action inspector and accessibility controls; separate label settings for the Mac and phone.
- Phone navigation opens the configured destination page, including overflow layouts. Phone labels and icon-picker choices now render correctly.
- The live controller publishes update notices for available Mac downloads.
- Local verification passed 43 core tests, 23 Web/Worker tests, native builds and isolated trial, action, recovery, reorder and encrypted relay checks. The user confirmed pairing, navigation, smooth dragging/rotation, refresh/reconnect and immediate phone updates after Mac reordering.
- Hosted private-source CI was unavailable at packaging time. This requested preview was built from the locally verified review branch; the source PR remains open.

**Upgrade:** quit TapDeck, install 0.3.4 and replace the app in Applications. Refresh Safari/Home Screen tabs. Existing pairing and original trial expiry are retained; 0.3.2 and newer Mac builds remain compatible.

## 0.3.3 — Mac editor

[Download and release details](https://github.com/wakeupbrk/TapDeck/releases/tag/v0.3.3)

- The Mac app edits directly. Click a button to select it, keep the inspector beside the deck, and use Test to run it.
- Drop an application onto the deck to add a button. A website drop does not add a button. Websites stay on Add.
- Right-click a deck to modify or delete it. The last deck cannot be deleted.
- Check for Updates is in the app menu and Settings. The download button opens only this repository’s releases. The hosted controller does not publish that catalog yet, so a check does not mark this preview out of date.

**Upgrade:** install the 0.3.3 Mac preview. A 0.3.2 app still connects. Builds older than 0.3.2 cannot reconnect. Saved pairing and original seven-day trial timestamps remain compatible.

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
