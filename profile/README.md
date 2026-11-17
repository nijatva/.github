# Nijatva

Small, single-purpose Android apps with no Google Play Services, no accounts,
no ads and no analytics. Built in India.

**Seven apps ship releases today.** The rest are being built in the open, one at
a time, and every repository says which state it is in.

## The rules we do not bend

- **No Google Play Services.** Every app is built for AOSP without GMS, so it
  runs on de-Googled Android and on BharOS.
- **No accounts.** There is nothing to sign up for. Everything stays in the
  device's own storage.
- **No ads, no analytics.** No tracking SDK is linked in. Not disabled, not
  opt-out. Absent.
- **Made in India.** Indian languages and Indian networks as the first target.

## Apps with releases

| App | Version | Notes |
|---|---|---|
| Browser | 2.0.3 | Containers, tracker blocking, reader mode, TTS. Desktop builds too |
| Camera | 0.4.10 | Camera2, manual controls, RAW, night stacking |
| Gallery | 0.1.3 | Local albums, EXIF stripped on share |
| Music | 1.1.2 | Folder-based player, equaliser, sleep timer |
| Dialer | 1.4 | T9, dual-SIM, spam blocklist |
| Contacts | 1.1 | vCard import and export, duplicate merge |
| Messages | 1.1 | Threaded SMS and MMS, offline OTP detection |

Some of these are debug builds; the release page for each app says so. Release
signing is being set up.

## The foundation

Four repositories that every app is built on: `nijatva-core` (Compose design
system, storage helpers, backup), `no-gms-check` (fails CI on any Play Services
or Firebase artefact), `nijatva-design` (icons and templates) and
`nijatva-suite` (the app index and self-hosted F-Droid style repository).

## Where to get the apps

- Website and full status: <https://nijatva.github.io>
- APKs: the releases page of each repository
- No Play Store, no F-Droid listing yet. Distribution is an APK.

## The name and the icon

The code is Apache-2.0. You can use it, change it and ship it, including inside a
closed-source app, as long as you keep the licence and say what you changed.

The **name "Nijatva" and the app icons are not covered by that licence.** A fork
must use its own name and its own icon, so that a user can tell which app they
are installing. Nothing stops a fork from existing; it just cannot pretend to be
this one.

## Contact

Vasudev.work@rediffmail.com
