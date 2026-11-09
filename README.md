<p align="center">
  <img src="assets/hero-en.svg" width="100%" alt="Dynamic Audio: an island for the MacBook notch">
</p>

<p align="center">
  <b>English</b> · <a href="README.ru.md">Русский</a>
</p>

<p align="center">
  <a href="https://github.com/5DHelLD5/dynamic-audio-releases/releases/latest"><img src="https://img.shields.io/github/v/release/5DHelLD5/dynamic-audio-releases?style=for-the-badge&label=release&labelColor=1f1b2e&color=a855f7" alt="Latest release"></a>
  <img src="https://img.shields.io/badge/macOS-27%2B-111111?style=for-the-badge&logo=apple&logoColor=white&labelColor=1f1b2e" alt="macOS 27 or later">
  <img src="https://img.shields.io/badge/price-free-1fc27a?style=for-the-badge&labelColor=1f1b2e" alt="Free">
  <a href="https://github.com/5DHelLD5/dynamic-audio-releases/releases"><img src="https://img.shields.io/github/downloads/5DHelLD5/dynamic-audio-releases/total?style=for-the-badge&label=downloads&labelColor=1f1b2e&color=ec4899" alt="Downloads"></a>
</p>

<p align="center">
  Your MacBook's notch, alive. Music with a spectrum measured from the real sound,<br>
  volume and brightness, battery and headphones, a file shelf, timers,<br>
  and what Claude Code and Codex are doing right now.
</p>

<p align="center">
  <a href="https://github.com/5DHelLD5/dynamic-audio-releases/releases/latest"><img src="assets/download-en.svg" width="300" alt="Download for macOS"></a>
</p>

<p align="center">
  <a href="https://web.tribute.tg/d/TQG"><img src="https://img.shields.io/badge/Support_the_author-Tribute-229ED9?style=for-the-badge&labelColor=1f1b2e" alt="Support the author via Tribute"></a>
</p>

<p align="center">
  <a href="#what-it-does">Features</a> ·
  <a href="#install">Install</a> ·
  <a href="#if-it-does-not-open">Won't open?</a> ·
  <a href="#uninstall">Uninstall</a> ·
  <a href="#privacy">Privacy</a> ·
  <a href="#help">Help</a> ·
  <a href="#support-the-author">Support</a>
</p>

---

## What it does

### Music
- The cover and a **live spectrum** right at the notch, in 23 styles. The spectrum comes from your Mac's actual audio, measured as it plays and never recorded.
- An expanded player with seeking, volume, likes, AirPlay and a sleep timer that fades out.
- **Lyrics** that fill with color as they are sung, under the notch or in the player.
- **Stage**: when your Mac sits idle while music plays, the screen turns into a stage with the cover, the lyrics and the visualizer.
- **Music stats**: how much you listened this week, your top tracks and artists.
- Works with any player macOS shows in Control Center.

### Claude Code and Codex
While an agent works, the island shows what it is doing, how long it has been at it and how much of your limits is left. When Claude asks for permission, you can allow or deny it right from the island. When it finishes, you see it.

<p align="center">
  <img src="assets/agents-en.png" width="588" alt="Three Claude Code sessions with their current steps, and the Claude and Codex limits">
</p>

<p align="center">
  <img src="assets/done-en.png" width="457" alt="Claude finished in weather-app, last step: an edit to ContentView.swift">
</p>

### HUDs worth looking at
Volume and brightness with a scale, headphones with the battery of each bud, meetings with a Join button, a mouse or keyboard running low, external drives, timers, Caps Lock and the keyboard layout. They appear in the island and stay out of your way.

<p align="center">
  <img src="assets/volume-en.png" width="415" alt="Volume at 62">
  <img src="assets/brightness-en.png" width="415" alt="Brightness at 80">
</p>

<p align="center">
  <img src="assets/headphones-en.png" width="436" alt="AirPods Pro connected, with the battery of each bud and the case">
  <img src="assets/event-en.png" width="457" alt="A team call in 5 minutes, with a Join button">
</p>

<p align="center">
  <img src="assets/mouse-en.png" width="366" alt="Magic Mouse battery almost empty">
  <img src="assets/timer-en.png" width="383" alt="A 25-minute timer at the notch">
</p>

### When nothing is playing
The time and date, the weather in your city, CPU and memory load and the battery, one glance away.

### And more
| | |
|---|---|
| **Clipboard history** | Everything you copied, one shortcut away |
| **Shelf and AirDrop** | Drop files on the island to keep them handy or send them on |
| **Downloads and scripts** | Browser downloads and any command's progress at the notch |
| **External drives** | A card when a drive connects, and eject from the island |
| **Timer and Pomodoro** | The countdown lives at the notch |
| **Keep awake** | Your Mac stays awake for as long as you need |
| **Microphone** | Mute with one shortcut, with a red dot while you are muted on a call |
| **Mirror** | A quick camera check before a call |
| **English and Russian** | Follows your system language, or pick one in Settings |

### Settings that explain themselves
Every feature has its own switch, and the Overview page shows them all at once.

<p align="center">
  <img src="assets/settings-en.png" width="700" alt="Dynamic Audio settings, the Overview page">
</p>

---

## Install

You need macOS 27 or later on an Apple silicon Mac. The island is made for MacBooks with a notch; on other displays it becomes a glass capsule at the top edge of the screen.

1. Download `Dynamic-Audio-X.Y.zip` from the [latest release](https://github.com/5DHelLD5/dynamic-audio-releases/releases/latest).
2. Unzip it and drag **Dynamic Audio.app** into **Applications**.
3. Open it. A short setup asks which features you want and only for the permissions they need.

Updates install themselves after a check of the developer's signature.

---

## If it does not open

Dynamic Audio is signed but not yet notarized by Apple, so macOS may block the first launch.

- **"Dynamic Audio is damaged and can't be opened."** It is not damaged. Run this in Terminal, then open the app again:
  ```bash
  xattr -cr "/Applications/Dynamic Audio.app"
  ```
- **"Apple could not verify it is free of malware."** Open **System Settings → Privacy & Security**, scroll down to Dynamic Audio and click **Open Anyway**.

---

## Uninstall

If you connected Claude Code, first open **Settings → Claude and Codex** and click **Disconnect…**. This removes the app's hooks from `~/.claude/settings.json`.

Then click **Settings → General → Reset all settings…**. This deletes your settings, the Yandex Music sign-in, pinned clipboard items, shelf copies, listening stats and caches. Dynamic Audio restarts clean: quit it from its menu bar menu and move it from Applications to the Trash.

---

## Permissions

Each permission is asked for only when you turn on the feature that needs it.

| Permission | What for |
|---|---|
| System audio recording | The live spectrum |
| Accessibility | "Copied" and "Pasted", pasting from the history |
| Calendar | Meeting reminders |
| Camera | The mirror |
| Automation of Music | The like button for Apple Music |

---

## Privacy

No account, no analytics, no ads. Audio, camera, calendar and clipboard are handled on your Mac only. The app goes online only for lyrics (track title and artist), update checks on GitHub and, once you set them up, the weather (the city name goes to Open-Meteo) and Yandex Music. Each can be switched off in Settings. Details: [PRIVACY.md](PRIVACY.md).

---

## Help

- **Something is broken:** check [If it does not open](#if-it-does-not-open), then open a [bug report](https://github.com/5DHelLD5/dynamic-audio-releases/issues/new?template=bug_report.yml) with your Dynamic Audio version (Settings → About) and macOS version.
- **An idea:** open a [feature request](https://github.com/5DHelLD5/dynamic-audio-releases/issues/new?template=feature_request.yml).
- **A security issue:** report it privately, see [SECURITY.md](SECURITY.md).
- **Documents:** [LICENSE.md](LICENSE.md), [PRIVACY.md](PRIVACY.md), [TRADEMARKS.md](TRADEMARKS.md), [SUPPORT.md](SUPPORT.md).

---

## Support the author

Dynamic Audio is free, with no trial, ads or sign-up. If it earned its place at your notch, you can support the author with any amount. It is voluntary and unlocks nothing.

Donations go through [Tribute](https://web.tribute.tg/d/TQG). Pay by card in your browser with just an email address, or right in Telegram.

A star on this repository helps other people find the app too.

---

<p align="center">
  <sub>© 2026 5DHelLD5. Free to use, see the <a href="LICENSE.md">license</a>. This repository holds releases only; the source code is closed.</sub><br>
  <sub>Apple, Mac, MacBook and macOS are trademarks of Apple Inc. Claude belongs to Anthropic and Codex to OpenAI. Dynamic Audio is not affiliated with them.</sub>
</p>
