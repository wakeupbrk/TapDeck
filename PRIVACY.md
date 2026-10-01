# TapDeck preview privacy

Trial activation is optional: declining keeps controls locked. Starting sends an app-specific SHA-256 hash derived from your Mac’s hardware UUID to the TapDeck service over HTTPS. The raw hardware UUID is never transmitted. The service retains the hash, activation timestamp and fixed seven-day expiry indefinitely to recognize the same Mac after reinstalling. No email, account or payment information is collected by this preview. Trial verification continues while the app runs and requires internet access.

The phone browser stores its pairing credential locally to reconnect. Clearing browser data requires pairing again; it does not reset the Mac trial. QR invitations require local Mac approval. Messages between approved devices use authenticated encryption. The relay does not persist deck messages or intentionally log their contents. Cloudflare processes connection metadata, including IP addresses, to deliver and protect the service. No analytics SDK is included.

A Mac or browser you unlock, software running on that device, and the hosting/deployment account are trusted parts of the system. Revoke browsers in Mac settings when needed. Never share a pairing QR or active invitation.

For privacy questions, use the repository’s discussions/issues without posting device identifiers, credentials or personal deck data. Security reports belong in private vulnerability reporting. This is an experimental preview; future paid products will provide their own terms.
