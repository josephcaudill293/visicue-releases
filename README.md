# VisiCue downloads

Official release downloads and update information for VisiCue on macOS and Windows.

## Availability

- **Windows:** 1.0.19 Preview 2 has been built. Download publication is in progress; no installer is currently confirmed uploaded here.
- **macOS:** Release packaging and update signing configuration are in progress.

This repository contains finished apps and public release information. Application source code and private signing keys are not published here.

## Windows preview

The x64 installer includes the .NET runtime and an offline English speech model. The portable ZIP must be fully extracted before opening the app. The preview is unsigned. Windows hardware, UI, installation, and upgrade testing remain outstanding.

75 automated core checks passed, alongside native speech replay, Mac show-file compatibility, and updater guard checks. See the validation report accompanying the preview for scope and limitations.

## Automatic updates

Updater integration is implemented, but production update feeds and signing configuration are not yet complete. Preview 2 has no production feed configured and will require a manual installation of the first update-enabled release. Do not treat this repository as an active update service yet.

## Feedback

Report problems through [Issues](https://github.com/josephcaudill293/visicue-releases/issues). Include the app version, operating system, and reproduction steps. Issues are public; omit private logs and personal information.
