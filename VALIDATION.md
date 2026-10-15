# VisiCue 1.0.20 validation

## macOS

- Full Release archive compiled in Xcode 27 for Intel x86_64 and Apple Silicon arm64.
- Bundle identifier remains com.JosephCaudillMusic.VisiCue; build number 20.
- App launched and rendered its main interface, both speech-language selectors, input controls, cues, MIDI controls, and Companion controls.
- Check for Updates contacted the published Sparkle feed and reported the installed build was current.
- The final app passes codesign --verify --deep --strict. It is locally signed, not Apple Developer ID signed or notarized.
- The distributed ZIP includes Sparkle's license notice. Its Ed25519 update signature was independently verified against the public key embedded in the app.
- Existing Mac updater interlock regression checks cover running shows and pending audio startup.

## Windows

- .NET 10 self-contained Windows x64 publish and Velopack 1.0.20 packaging completed.
- 75 core regression checks pass, covering trigger confirmations/deduplication, show round trips, atomic saving, request authentication, PCM backpressure, invalid audio samples, MIDI ownership/timing, and schedules.
- The update package contains the production HTTPS feed configuration and bundled offline English model.
- Every package's byte length and SHA256 match releases.win.json.
- Previous native Vosk replay and production Mac show-file round-trip tests passed. Those validate the model/format, not Windows hardware drivers.

## Remaining checks and signing

Windows hardware/UI testing is deferred at the owner's request. Windows installation/uninstallation and a two-version download/install/restart cycle have not been verified. Mac speech/audio hardware testing and an actual two-version Sparkle installation are also not established by the checks above.

Apple Developer ID signing/notarization and Windows Authenticode publisher signing require certificates not present on this build host. OS unidentified-publisher warnings may appear. Cryptographic Sparkle update signing is configured independently of Apple notarization.
