# VisiCue

Official VisiCue downloads for macOS and Windows. Current versions: **Mac 1.0.21**, **Windows 1.0.20**.

## Downloads

- [Download for Mac](https://github.com/josephcaudill293/visicue-releases/releases/latest/download/VisiCue-macOS.dmg) — universal app for Apple Silicon and Intel; macOS 14 or later. Open the DMG, drag VisiCue onto the Applications shortcut, then eject the disk image and open VisiCue from Applications.
- [Download Windows installer](https://github.com/josephcaudill293/visicue-releases/releases/latest/download/VisiCue-Windows-Setup.exe) — Windows x64; runtime and offline English model included.
- [Download Windows portable ZIP](https://github.com/josephcaudill293/visicue-releases/releases/latest/download/VisiCue-Windows-Portable.zip) — extract the entire folder before opening the app.

Both platforms support multilingual speech triggers, with up to two active speech languages. Windows can use downloaded Vosk models or installed Windows speech languages.

Mac 1.0.21 also includes **Check for Updates…** in the top-right VisiCue icon menu.

## Automatic updates

Check for Updates is configured in these builds. Mac uses Sparkle with Ed25519-signed ZIP archives; the DMG is the website installation download. Windows uses Velopack with HTTPS hosting and package checksums. Existing builds without a configured feed need one manual installation of 1.0.20. Portable Windows copies require installation before in-app updating.

## Validation and publisher signing

The universal Mac archive, app launch, signature verification, live update-feed check, DMG checksums, and mounted DMG contents passed verification. The Windows x64 build and 75 core checks passed. [Read the validation details](VALIDATION.md). Windows hardware/UI and installation tests, and a two-version installation/update cycle, remain unverified.

The Mac app is locally signed and not Apple-notarized. Windows binaries are not Authenticode-signed. OS unidentified-publisher warnings may appear; publisher signing requires certificates not present on the build host.

[Release notes and checksums](https://github.com/josephcaudill293/visicue-releases/releases/latest). The DMG has its own accompanying SHA256 checksum file.

This repository contains downloads and public release information. Application source code and private signing keys are not published here. GitHub's generated source archives contain repository documentation, not app installers.

## Feedback

Report problems through [Issues](https://github.com/josephcaudill293/visicue-releases/issues). Include app version, operating system, and reproduction steps. Issues are public; omit private information.
