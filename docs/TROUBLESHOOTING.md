# Troubleshooting

[← TapDeck](../README.md) · [Getting started](GETTING-STARTED.md) · [Report a bug](https://github.com/wakeupbrk/TapDeck/issues/new?template=bug_report.yml)

## Start here

| Symptom | First check |
| --- | --- |
| Phone keeps reconnecting | Install Mac 0.3.2, refresh the phone page, keep the Mac awake and check internet access |
| QR will not pair | Generate a fresh invitation and approve the browser on the Mac |
| Keyboard control does nothing | Check the target app and Mac Accessibility permission |
| Controls are locked | Check trial status and internet access; original expiry survives reinstalling |
| Download opens as a text file | Choose the `.dmg` asset rather than `SHA256SUMS.txt` |

## macOS blocks the app

The preview is ad hoc signed and **not notarized**. macOS may block it. Confirm that you downloaded it from the [official release](https://github.com/wakeupbrk/TapDeck/releases/tag/v0.3.2-security.1) and verify the checksum below. A checksum confirms the file matches the published build; it does not make an app notarized or prove that it is safe.

Keep macOS security protections enabled. If you cannot install the preview comfortably, wait for a Developer ID signed, notarized release. Include the exact macOS message in a bug report, with personal information removed.

## Verify the download

Download `SHA256SUMS.txt` and the DMG from the same release. Put them in the same folder and run this in Terminal from that folder:

```sh
shasum -a 256 -c SHA256SUMS.txt
```

The expected result is `TapDeck-0.3.2-Mac.dmg: OK`. If the files were renamed by your browser, restore the names used in the checksum file first. A mismatch means the file does not match; download a fresh copy from the official release before installing.

## The phone stays disconnected

1. Check that your Mac is awake, TapDeck is running and remote control is not paused.
2. Check internet access on both devices and your Mac trial status.
3. Make sure the Mac app is **0.3.2**. Refresh the browser or Home Screen controller after upgrading.
4. Reopen the same saved controller. Switching browsers, private browsing and cleared browser storage may require a new pairing.
5. If the pairing was revoked or the invitation expired, generate a fresh QR and approve it on the Mac.

Avoid clearing pairing as the first troubleshooting step. Saved pairing and original trial expiry are retained when upgrading normally.

## A QR expires or the bare website shows instructions

Invitations expire after two minutes. Generate another from TapDeck on your Mac and open it with your phone. The plain controller address contains no invitation, so it cannot connect by itself.

## Keyboard commands fail

Choose the correct target application. Grant Accessibility permission to the installed TapDeck copy when you use keyboard controls, and check whether the target is ready to receive the command. Opening ordinary apps or websites does not need Accessibility.

For Apple Shortcuts, check the exact shortcut name and whether it waits for an interactive prompt. A delay in a macro waits a fixed time; it does not confirm another app finished its work. Cancelling a macro cannot undo already completed steps.

## The trial is unavailable or expired

Trial verification needs internet access. A verification failure locks controls. After the original seven-day expiry, controls stay locked; reinstalling does not restart the trial. Your deck remains available to export. Paid activation is not available yet.

## Still stuck?

[Report a bug](https://github.com/wakeupbrk/TapDeck/issues/new?template=bug_report.yml) with the Mac app version, macOS version, phone/browser versions and steps to reproduce. Remove pairing URLs, QR codes, device identifiers and personal data from screenshots or diagnostics. Security concerns belong in [private reporting](../SECURITY.md).
