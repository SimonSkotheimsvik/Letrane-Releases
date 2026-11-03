# Letrane releases

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/branding/letrane-wordmark-dark.svg">
  <img src="assets/branding/letrane-logo-horizontal.svg" alt="Letrane — a purple L icon and a wordmark with an emphasized beginning" width="317">
</picture>

**The beginning guides the eye.**

Letrane is an experimental Windows reading-assistance app. Its transparent reading
window emphasizes word beginnings or gently fades word tails in other apps,
without changing the original text. Recognition runs locally using Windows OCR.
It is not a medical treatment and does not guarantee improved reading.

**[Download the latest signed Windows EXE](https://github.com/SimonSkotheimsvik/Letrane-Releases/releases/latest)**

## A calmer place for the eyes to land

Letrane began with a simple observation: my daughter, Ane, found text easier to
follow when the beginnings of words were emphasized. I wanted to explore a small,
practical tool that could bring those visual anchors to the text already on her
screen, rather than asking her to copy everything into a separate reading app.

The result is a movable reading frame for webpages, documents and emails. Place
it over the text, choose an appearance that feels comfortable, and keep using
the app underneath as usual. The original document stays unchanged.

Different people prefer different visual cues. Letrane lets you try highlighted
word beginnings, softer word tails, or both, and adjust their strength. It is an
experiment in making text more comfortable to follow, not a promise that one
reading style works for everyone.

### Reading support and ADHD

Some people with ADHD find visual reading aids, such as a line guide or clearer
word beginnings, helpful for keeping their place and making reading feel more
manageable. Letrane offers these as optional supports to try, not as a solution
that works for everyone.

**Letrane has not been clinically validated, and its reading benefits for people
with ADHD have not been medically proven.** It does not diagnose, treat or cure
ADHD, and it is not a replacement for professional advice or care. Personal
experiences are not clinical evidence; choose what feels comfortable for you.

## Why “Letrane”?

The name brings together **letters**, **Ane**, and a little bit of **rain**.
We live on Norway's rainy west coast, but the rain has another meaning too:
a busy page can feel like letters raining down, with nowhere for the eyes to
settle.

Letrane aims to add calmer places to land—small visual anchors at the beginnings
of words.

**Letters. Ane. Rain. Letrane.**

## What you can do

- **Read in other apps:** move and resize the transparent, always-on-top frame
  over the text you want to follow.
- **Make the emphasis comfortable:** choose colors, emphasize the first 1–5
  characters, and adjust highlight strength or word-tail fading.
- **Guide your place:** optionally follow the mouse with a thin reading-line
  frame and one, three or five line-sized slots.
- **Keep changes smooth:** tune how the markings respond to small webpage changes.
- **Match your desktop:** use System, Light or Dark appearance.
- **Start simply:** the Help tab opens first, with three quick steps and a
  built-in reading-style preview.
- **Keep recognition local:** Windows OCR processes the text on your device.
  Optional aggregate usage reporting and update checking are explained below.

## Screenshots

These are views of Letrane's latest development interface, rendered in a clean
preview. No personal documents or desktop content are shown. The screenshots
show the new defaults for the next release; the currently published v0.1.0
download may look different.

The new defaults are **Smooth changes: 3%**, **Lead emphasis: 2** and
**Tail fade strength: 75%**. **Highlight color** starts off, with **Yellow**
selected; **Fade word tails** starts on. **Follow mouse** starts on with
**3 lines**, **Middle** placement and **gradient fill**. **Color theme** is
**System** (shown here on a dark Windows desktop).

### Follow your reading line

The yellow follow-mouse frame keeps the active middle line clear, with a soft
gradient above and below it. Word tails are gently faded while the first two
characters stay unchanged.

This clean demonstration uses sample text recognized by Windows OCR and
Letrane's actual reading-frame and overlay rendering. The pointer position is
fixed for the image; no private desktop content is captured.

![Letrane reading frame over sample text, with faded word tails and a yellow three-line follow-mouse gradient around the clear middle line](assets/screenshots/follow-mouse.png)

### Start with three simple steps

The Help tab explains how to position the frame, read at your own pace and make
the appearance comfortable.

![Letrane Help tab with the quick-start guide in dark appearance](assets/screenshots/help.png)

### Try the reading style

The **Reading style** checkbox applies Letrane's emphasis directly to the Help
text. This shows the built-in preview—not a screenshot of OCR over another app.

The preview uses the new default tail fading; the mouse-following frame is
demonstrated separately above, not inside the Help text.

![Letrane Help text with the first two characters unchanged and word tails gently faded](assets/screenshots/reading-style.png)

### Make it your own

Reading assistance, word appearance and mouse-following controls are grouped
into compact cards, with explanations available from the small information icons.

![Letrane Settings tab showing smoothing, word emphasis and mouse-following options](assets/screenshots/settings.png)

![Letrane Follow mouse controls with tracking enabled, three lines, Middle placement and gradient enabled, followed by System color theme](assets/screenshots/follow-mouse-settings.png)

## The visual identity

<img src="assets/branding/letrane-256.png" alt="Letrane purple rounded-square app icon with a white weighted L" width="96">

The purple icon contains a geometric **L** with a heavier leading stem and a
lighter trailing foot. The **Let**rane wordmark follows the same idea: an
emphasized beginning, followed by a quieter ending.

The brand purple is `#6558E8`, supported by deep `#25223A` and light `#F7F7FC`.
The branding echoes the app's visual-anchor idea; your reading-highlight color
is yours to choose.

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

The next release also includes current reading-setting choices in these reports,
so the developer can see which options people prefer. These are exit-time
preferences, not a record of what you read or how long you used each setting.
Sharing the settings follows the same Statistics opt-out.

Received reports are retained for 12 years (4,383 days). Opting out stops future
reports but does not erase existing reports early. Network services process
transport metadata. Reporting is separate from update checking.

## Freeware

Letrane is free to use. Optional support:
[Buy me a coffee](https://buymeacoffee.com/simonskothn).
