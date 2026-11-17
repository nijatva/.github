# Nijatva

Small, single-purpose Android apps with no Google Play Services, no accounts,
no ads and no analytics. Built in India.

**Seven apps ship releases today.** The rest are being built in the open, one at a
time, and every repository says which state it is in.

## The rules we do not break

- **No Google Play Services.** Every app is built for AOSP without GMS, so it runs
  on de-Googled Android and on BharOS.
- **No accounts.** There is nothing to sign up for. Everything stays in the
  device's own storage.
- **No ads, no analytics.** No tracking SDK is linked in. Not disabled, not
  opt-out. Absent.
- **Made in India.** Indian languages and Indian networks as the first target.

## Apps with releases

| | App | Version | What it does |
|---|---|---|---|
| <img src="https://nijatva.github.io/assets/icons/browser.svg" width="32" height="32" alt=""> | **[Browser](https://github.com/nijatva/nijatva-browser)** | 2.0.3 | Containers, tracker and ad blocking, reader mode, text-to-speech. Desktop builds too |
| <img src="https://nijatva.github.io/assets/icons/camera.svg" width="32" height="32" alt=""> | **[Camera](https://github.com/nijatva/nijatva-camera)** | 0.4.10 | Camera2 with manual controls, RAW, night stacking, panorama |
| <img src="https://nijatva.github.io/assets/icons/gallery.svg" width="32" height="32" alt=""> | **[Gallery](https://github.com/nijatva/nijatva-gallery)** | 0.1.3 | Local albums, EXIF stripped when you share |
| <img src="https://nijatva.github.io/assets/icons/music.svg" width="32" height="32" alt=""> | **[Music](https://github.com/nijatva/nijatva-music-player)** | 1.1.2 | Folder-based player, equaliser, sleep timer |
| <img src="https://nijatva.github.io/assets/icons/dialer.svg" width="32" height="32" alt=""> | **[Dialer](https://github.com/nijatva/nijatva-dialer)** | 1.4 | T9 keypad, dual-SIM picker, spam blocklist |
| <img src="https://nijatva.github.io/assets/icons/contacts.svg" width="32" height="32" alt=""> | **[Contacts](https://github.com/nijatva/nijatva-contacts)** | 1.1 | vCard import and export, duplicate merge |
| <img src="https://nijatva.github.io/assets/icons/sms.svg" width="32" height="32" alt=""> | **[Messages](https://github.com/nijatva/nijatva-messages)** | 1.1 | Threaded SMS and MMS, offline OTP detection |

Some of these are debug builds; the release page for each app says so. Release
signing is being set up.

The other sixteen apps — Calculator, Clock, Notes, QR Scanner, Files, Recorder,
PDF Viewer, Device Info, Weather, Calendar, Expenses, Tasks, RSS Reader, Vault,
Keyboard, Launcher, App Manager — are planned, and the [website](https://nijatva.github.io/apps.html)
says so in a table rather than in adjectives.

## The foundation

Four repositories that every app is built on:

- **[nijatva-core](https://github.com/nijatva/nijatva-core)** — Compose design
  system, storage helpers, backup, encrypted preferences
- **[no-gms-check](https://github.com/nijatva/no-gms-check)** — fails the build on
  any Play Services or Firebase artefact
- **[nijatva-design](https://github.com/nijatva/nijatva-design)** — icons and
  templates that keep the suite looking like one suite
- **[nijatva-suite](https://github.com/nijatva/nijatva-suite)** — the app index and
  the self-hosted F-Droid style repository

## How the apps work together

They do not depend on each other. Every app installs alone and works alone; when a
sibling is installed they hand off to each other over intents. No app links
another app's code. The contract lives in
[nijatva-core/INTEROP.md](https://github.com/nijatva/nijatva-core/blob/main/INTEROP.md).

## Get involved

Bugs, accessibility fixes and translations are welcome. Read
[CONTRIBUTING.md](https://github.com/nijatva/.github/blob/main/CONTRIBUTING.md)
first: contributions stay Apache-2.0, commits need a `-s` sign-off, and any pull
request that adds Play Services, Firebase or an analytics SDK will fail the build
before anyone reads it.

Every repository has Issues switched on. If a report is about several apps at
once, open it on the app where you saw it and say which others are affected.

## Where to get the apps

- Website and full status: <https://nijatva.github.io>
- APKs: the releases page of each repository
- No Play Store, no F-Droid listing yet. Distribution is an APK.

## The name and the icon

The code is Apache-2.0. You can use it, change it and ship it, including inside a
closed-source app, as long as you keep the licence and say what you changed.

The **name "Nijatva" and the app icons are not covered by that licence.** A fork
must use its own name and its own icon, so that a user can tell which app they are
installing. Nothing stops a fork from existing; it just cannot pretend to be this
one.

## Contact

Vasudev.work@rediffmail.com
