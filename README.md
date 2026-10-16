# Komic Desktop

A modern desktop manga & comic reader for Windows.

Read, organize and download your library, install content extensions, and keep everything in sync with AniList and MyAnimeList - all in one app.

[![Download Latest Release](https://img.shields.io/badge/Download-Latest%20Release-8b5cf6?style=flat&logo=github)](https://github.com/xNightStar0/Komic/releases/latest)
[![Windows Only](https://custom-icon-badges.demolab.com/badge/Windows%20Only-0078D6?logo=windows11&logoColor=white)](#)
[![Total Downloads](https://img.shields.io/github/downloads/xNightStar0/Komic/total?style=flat&logo=github&label=Total%20Downloads&labelColor=27303D&color=0D1117)](#)
</div>

---

## Screenshots

| Home | Library |
| :---: | :---: |
| ![Home](docs/screenshots/home.png) | ![Library](docs/screenshots/library.png) |

| Reader | Discover |
| :---: | :---: |
| ![Reader](docs/screenshots/reader.png) | ![Discover](docs/screenshots/discover.png) |

| Extensions | Settings |
| :---: | :---: |
| ![Extensions](docs/screenshots/extensions.png) | ![Settings](docs/screenshots/settings.png) |


---

## Getting started

1. Install extensions: open the Extensions page and install the sources you want (the app ships with the Keiyoushi extension catalog; more stores can be added).
2. Find a series: use Discover to search across every installed source at once, then add titles to your library.
3. Read: open any title and choose a chapter. The reader supports long-strip, single-page and double-page modes, with right-to-left as the default direction.
4. Download for offline: download chapters from the title page and find them later under Downloads.
5. sync: connect AniList or MyAnimeList in Settings → Tracking to sync your library and reading progress in both directions.

---

## Features
### Library & dashboard
- Dashboard with Continue reading and a preview of your library
- Full library with tracker-aware tabs: Reading, Planning, Completed, Paused, Dropped, Rereading
- Custom categories with create/delete and quick "move to category"
- Powerful filters & sorting: status, reading progress, source, title, chapter count, unread chapters, recently updated
- Display modes: compact grid, comfortable grid and list
- Unread and download badges, optional tab counters
- Bulk tools: Bulk match sources, Migrate titles and Refresh chapters
- Reading history of every chapter you opened

### Discover
- One search across all installed sources in parallel
- Per-source language preferences for multi-language extensions
- Add any result straight to your library with one click

### Extensions
- Powered by the bundled Komic Engine — a local, headless extension runtime (based on Suwayomi) that starts automatically with the app
- One-click Install / Update / Remove from the built-in extension catalog
- Add custom extension stores
- Filter and browse by language, content warnings and A–Z order
- Runs fully on 127.0.0.1 — nothing is exposed to the network

### Reader
- Page modes: Long strip (webtoon-style), Single page and Double page
- Reading direction: Right-to-left (default) or left-to-right — ideal for manga
- Image fit (width / height / original), page width and gap controls
- Reader backgrounds (black / charcoal / white), grayscale and dim options
- Auto-scroll, smooth scrolling, preload and configurable progress-bar position
- Zen mode, fullscreen, chapter list, change source, next/previous chapter
- Chapter actions: mark as read, mark as unread, mark this and below as read
- Full keyboard support (see below)

### Offline reading
- Download chapters and read them without a connection
- Downloads manager with Downloading, Failed and Completed sections
- Downloaded chapters are marked in your library and history

### Tracking
- AniList: built-in sign-in, two-way library sync, status updates, reading-progress sync and custom categories that appear on your AniList list
- MyAnimeList: secure OAuth sign-in, two-way sync and title matching
- Source matching for unlinked titles, including bulk matching for your entire library

### Data, privacy & backups
- Your library, reading progress and downloads are stored locally on your machine
- No account needed and no telemetry
- Automatic backups plus manual Backup & restore (export/import as a .zip, includes library, covers, downloads, extensions and settings)

### Network
- Built-in network proxy support (SOCKS5 / HTTP) — for example V2RayN on 127.0.0.1:10808
- Optional Cloudflare solver helper for sources protected by Cloudflare
- Diagnostics log for troubleshooting

---

## Keyboard shortcuts (Reader)

| Key | Action |
| --- | --- |
| F | Toggle fullscreen |
| P | Toggle auto-scroll (switches to long-strip mode) |
| H | Hide / show controls (zen mode) |
| Esc | Close settings, exit zen mode, or close the reader |
| Space / ↓ / S | Scroll down (long-strip mode) |
| ↑ / W | Scroll up (long-strip mode) |
| ← / → | Previous / next page (page modes, follows reading direction) |

A full help panel is also available in the reader via the ? button.

---

## FAQ & Troubleshooting

Windows/antivirus says the app or installer is unsafe.
The installer is not code-signed, so SmartScreen and some antivirus products flag it. If you downloaded the file from this repository's Releases page, click More info → Run anyway, or whitelist the file (and the installed folder) in your antivirus.

The Extensions page shows "Engine Offline".
The local engine usually starts automatically within a few seconds. If it stays offline, restart Komic Desktop, and make sure your antivirus or firewall is not blocking the app. Diagnostic logs are written to logs\desktop.log inside the app's data folder (see below).
A source returns no results or shows Cloudflare errors.
Some sources are protected by Cloudflare. Enable the Cloudflare solver in Settings → Connection, or try again later — sources can also be temporarily down on their side.

Where is my data stored?
Everything is stored locally in the app's data folder inside %APPDATA% (library database, cover cache, downloads, extensions, logs). You can export everything at any time from Settings → Backup & restore.

How do I move my library to another computer?
Use Settings → Backup & restore to export a backup .zip, then import it on the new machine.

Do I need an account?
No. Accounts are only needed if you want AniList or MyAnimeList sync; everything else works entirely offline.

How do I uninstall?
Uninstall via Settings → Apps → Komic Desktop, like any other Windows application. Your library data is kept so a reinstall restores your setup — export a backup first if you want to remove it manually.

---

## Feedback & support

- Found a bug? Open an [issue](https://github.com/xNightStar0/komic/issues) and include your version and a short description — attaching logs\desktop.log helps a lot.
- Have a feature request or feedback? Open an issue or start a discussion.

---

## Planned

- Local file reading (CBZ / ZIP / PDF and image folders)
- Additional community trackers

---

## License

Komic Desktop is proprietary software. Copyright (c) Komic Desktop. All rights reserved.

This repository does not contain source code. Redistribution, resale or modification of the application binaries is not permitted without prior written permission.

The bundled Komic Engine is based on [Suwayomi-Server](https://github.com/Suwayomi/Suwayomi-Server), licensed under the Mozilla Public License 2.0 (MPL-2.0). The engine's source and license files are available in the app under Settings → Komic Engine → "Engine licenses & source". Extension catalogs are provided by their respective communities (for example [Keiyoushi](https://github.com/keiyoushi/extensions)).

---

## Legal disclaimer

- Komic Desktop does not host, provide or distribute any manga or comic content.
- Extensions are third-party components that retrieve content from publicly available websites. The app is a reader and organizer only.
- You are responsible for how you use the app and for complying with your local laws and the terms of any website you access.
Notes before you publish:
