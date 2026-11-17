# Contributing to Nijatva

Short version: send a patch, sign it off, and it stays Apache-2.0. No CLA, no
paperwork, no email thread.

## What gets accepted

- Bug fixes, especially on de-Googled devices, BharOS and Android 7 to 15.
- Accessibility fixes and translations.
- Anything that makes an app smaller, faster or more private.

## What gets rejected without discussion

- Any dependency on Google Play Services, Firebase, Crashlytics or an ad SDK.
  The build guard `no-gms-check` exists to catch this; a pull request that adds
  one will fail CI before anyone reads it.
- Analytics, telemetry, crash reporting that phones home, or "anonymous usage
  statistics".
- A network call that is not the app's stated job.

If a feature needs any of the above to work, it does not belong in this suite.

## How to send a change

1. Open an issue first if the change is bigger than a bug fix.
2. Fork, branch, commit.
3. Sign off every commit: `git commit -s`. This is the Developer Certificate of
   Origin — it says you wrote the patch, or have the right to submit it.
4. Open the pull request and say what you tested on. A device model and an
   Android version are more useful than a screenshot.

## Licence of contributions

Contributions are accepted under the **Apache License 2.0**, the same licence as
the project: inbound equals outbound. You keep the copyright in your work; you
are not assigning it to anyone.

Because the licence is already permissive, the project can ship a build that
includes your patch under any terms Apache-2.0 allows. What nobody can do is
take your patch and relicense it to something else — that would need your
permission, and it would need everyone else's too.

## Style

- Kotlin, no Java. Compose for UI.
- Keep the shared skeleton: top bar, permission banner, main surface, three
  bottom actions. A user who learns one app should know all of them.
- No new dependency without a reason in the pull request. Every dependency is a
  promise to every user.

## Contact

Vasudev.work@rediffmail.com
