# In Dialogue for Android

A native Android voice recorder with offline transcripts, reviewable on-device cleanup, reusable vocabulary and optional NStack delivery.

[Install through Zapstore](https://zapstore.dev/apps/com.wingmanbefree.indialogue) or download the APK from [Releases](https://github.com/OtherStuffAI/in-dialogue/releases). This repository is the public APK and release-metadata catalog.

Record audio with a visible foreground microphone service, browse and play your local library, share audio and transcripts, correct individual words or edit the full transcript, and optionally deliver complete audio and reviewed text to your existing NStack workspace and channel. Automatic delivery and local retention are opt-in. Recording files and failed delivery snapshots are retained for recovery and explicit retry.

## Requirements and models

Android 9 or newer, with a 64-bit arm64 or x86_64 device. The initial speech model is English (US), an explicit approximately 40 MiB download. Optional cleanup uses an explicit approximately 469 MiB model download and needs roughly 1.5 GiB available RAM. Installed-model transcription and cleanup run on the device, with no cloud inference fallback. Cleanup drafts require review and acceptance; original transcripts remain separate.

## Privacy and updates

The app keeps recordings and its PIN-protected Nostr vault in app-private storage excluded from Android backup. Import your own Nostr identity only if you want NStack delivery. Model downloads and configured delivery require network access; recording and installed-model inference work offline.

Update in place with the same package and release certificate. Uninstalling deletes the library and vault. Export important recordings and keep your own Nostr-key backup. Android can stop capture after interruptions, force stop, reboot or storage exhaustion; previously saved segments are recovered where readable.

Package: `com.wingmanbefree.indialogue`.

Zapstore publisher: `npub1llwrq3rtah3rg3r2dyfyht55ek7aa0ey7z47ujju407pzfp38shqa7zcvr`.
