# VisiCue 1.0.22 validation

Both platforms now ship an offline interface translation catalog with 25 language choices and 525 source keys. English is listed once; speech-recognition regions remain independent. Native-language names make the first-run picker usable without navigating an English settings page.

A missing installation preference triggers setup once on new installs and upgrades. Continue/Apply persists completion. Settings allows later changes. Preferences stay outside show files. Windows requires restart after a settings language change. Urdu and Kashmiri use right-to-left layout. Translations are machine-assisted with targeted editorial corrections; native-speaker review is still welcome. System dialogs and updater panels use their own supported translations.

## Verified

- Universal Intel/Apple Silicon Mac Release archive (version 1.0.22, build 22) compiled in Xcode.
- The packaged Mac app launches. The first-run language selector, German preview, native language names, one English entry, language Settings from the main window and Command-comma, Urdu right-to-left preview, preference persistence, and relaunch without repeated setup were exercised.
- 26,261 checks on the actual Swift localization code passed: language resolution, coverage and placeholders.
- Windows x64 self-contained publish and Velopack setup, portable and full update package creation completed.
- 26,362 Windows core/localization checks passed: installation preference migration/persistence, regional language resolution, catalog coverage/placeholders, preservation of user placeholder text, show file compatibility, trigger confirmation/deduplication, atomic saving, remote authentication, PCM backpressure, and MIDI ownership/timing.
- Mac app signature passes deep/strict verification; archive contains both CPU architectures and the Sparkle license.
- Sparkle ZIP Ed25519 signature was independently verified with the embedded public key.
- DMG checksum verified. Mounted image contains the same signed app and catalog and a working /Applications shortcut.
- Release staging validates versions, ZIP/DMG structure, update-feed package sizes/checksums, and stable download filenames.
- Technical URLs, API paths, and Companion variable names in the catalog retain their exact literal values.

## Limits

Windows hardware/UI, installation/uninstallation, and a full two-version installation/update cycle have not been tested on this Mac host. Existing live speech/audio behavior is preserved; these checks do not establish new audio hardware performance results. The Mac app remains locally signed and not Apple-notarized; Windows remains without Authenticode publisher signing.
