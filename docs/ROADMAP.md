# What’s next

[← TapDeck](../README.md) · [Suggest a feature](https://github.com/wakeupbrk/TapDeck/issues/new?template=feature_request.yml) · [Release notes](CHANGELOG.md)

Our direction: **create on the Mac, control from the phone**. The Mac should be a comfortable workspace for building controls; the phone should stay a simple browser deck with large buttons and fixed pages.

These are planned areas, not promised dates. Priorities can change with feedback and testing. Shipped work is listed in the [changelog](CHANGELOG.md).

## Shipped in 0.3.3

- Click a button to select it. The inspector stays open, and Test runs the action.
- Drop an application onto the deck to add a button. Website drops are not included.
- The Mac app can check for an available or required update and opens only the official TapDeck release page.

## Next focus: a better Mac workspace

- **Direct creation:** drop website links into the workspace the same way applications drop in today.
- **Faster organization:** search, keyboard shortcuts, multi-select and batch moves.
- **Phone preview:** see portrait and landscape layouts while editing on the Mac.

## Reliability and release readiness

- Publish the update catalog from the hosted controller so installed 0.3.3 apps can see a newer release. The Mac check already exists.
- Clear connection troubleshooting and action-readiness feedback.
- Local deck history, safer restore and an import review before replacing data.
- Security reviews of new input paths and continued dependency maintenance.
- Keyboard/VoiceOver and physical Safari/Home Screen acceptance checks.
- Developer ID signing, notarization and a repeatable coordinated release process.

## Later ideas

- Optional workflow templates and a clean blank starting point.
- Better macro step organization, feedback and cancellation guidance.

The generic starter remains available. Pairing approval, authenticated encryption, revocation and the Mac’s control over action definitions remain product requirements. Improvements do not reset existing trial timestamps.

Have a use case we should understand? [Open a feature request](https://github.com/wakeupbrk/TapDeck/issues/new?template=feature_request.yml) with what you want to accomplish and the steps that feel awkward today. We track implementation privately and publish shipped changes in the [changelog](CHANGELOG.md).
