# Letrane releases

**The beginning guides the eye.**

Letrane is an experimental Windows reading-assistance app. Its transparent reading
window emphasizes word beginnings or gently fades word tails in other apps,
without changing the original text. Recognition runs locally using Windows OCR.
It is not a medical treatment and does not guarantee improved reading.

## Download and run

Download `Letrane.App.exe` from the [latest release](https://github.com/SimonSkotheimsvik/Letrane-Releases/releases/latest)
and launch it directly.

- Windows 11 x64 with an installed Windows OCR language is required.
- No installer, administrator access or separate .NET runtime is required.
- The EXE is signed and timestamped. SmartScreen may still show a reputation warning.
- The optional `Letrane.App.exe.sha256` asset verifies the downloaded file.
- Local preferences and statistics are saved under `%LOCALAPPDATA%\Letrane`.

Open Help in the app for the quick-start guide. Drag the purple reading frame over
text, resize it, and use Menu to customize the appearance.

## Updates

The app checks this repository for a newer stable release at startup, at most
once per day. About has a manual **Check for updates** button and a saved option
to disable automatic checks. A newer version opens a release page in your
browser; the app does not download or install updates automatically. Update
checks send no usage totals or installation identifier; GitHub receives normal
request metadata and the app version.

Tags follow `vMAJOR.MINOR.PATCH`, matching the executable's app version.
Published assets are not replaced with different builds under the same version.
This repository hosts public downloads only; application source is maintained
separately. WinGet publication requires a separate package submission.

## Usage reporting

Usage sharing is on by default and can be disabled on Statistics. On normal
Exit, the app sends aggregate usage totals, first-use time, app version and a
hashed random installation identifier to the developer's Azure service in North
Europe. No screen content, recognized text, hardware identifiers or account names
are included. The identifier links reports from the same installation; reports
are pseudonymous, not fully anonymous.

Received reports are retained for 12 years (4,383 days). Opting out stops future
reports but does not erase existing reports early. Network services process
transport metadata. Reporting is separate from update checking.

## Freeware

Letrane is free to use. Optional support:
[Buy me a coffee](https://buymeacoffee.com/simonskothn).
