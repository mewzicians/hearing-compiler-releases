# Judiciary Hearing Compiler: Mac downloads

This repository publishes built copies of the Judiciary Hearing Compiler
prototype for Apple Silicon Macs (M1 or later). It contains app builds only. No
hearing recordings, transcripts or notes are stored here.

## First install

1. Open the [latest release](../../releases/latest) and download
   `HearingCompilerPrototype-Mac-AppleSilicon.zip`.
2. Unzip it if your browser didn't, then drag **Hearing Compiler** into your
   **Applications** folder.
3. Double-click it. The first time, your Mac will say **"Apple could not verify
   'Hearing Compiler' is free of malware…"**. That's expected, because the app
   isn't notarized by Apple. Then:
   1. Click **Done**, not Move to Trash.
   2. Open **System Settings → Privacy & Security** and scroll down to
      **"Hearing Compiler" was blocked**.
   3. Click **Open Anyway**. When asked again, click **Open Anyway** and enter
      your Mac password.
4. Your browser opens the local workspace. Use **Stop app** when you're done.

Never turn off Gatekeeper. If your Mac says the app **is damaged and can't be
opened**, don't open it. Report it instead.

## Updates

After the first install, the app updates itself. When it opens, it checks for a
newer build. If nothing is processing, it downloads the build, checks its
fingerprint and signature, swaps it in and reopens. The window's top-right
corner shows the version and build number.

- **Saved work stays put.** Hearings and corrections live in
  `~/Library/Application Support/HearingCompilerPrototype/`, and updates don't
  change them. The previous version is kept in `updates/previous/` inside that
  folder.
- **Pre-releases are tests.** Builds marked **Pre-release** are being tested
  and are never installed automatically.

Every build has passed the project's automated tests and Mac package checks.
Drafts it produces still need human review against the source.
