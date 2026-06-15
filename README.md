# Sonix — Releases

Downloadable macOS (Apple Silicon) builds of **Sonix**, a desktop audio toolkit
for stem separation, BPM/key analysis, tagging, format conversion, and Serato
cue export.

This repository hosts the compiled `.app` builds only — the source code lives
in a separate private repository.

## Download

Grab the latest build from the [**Releases**](https://github.com/elDoof/sonix-releases/releases/latest)
page. Each release attaches `Sonix.app.zip`.

## First run on a new Mac

Sonix is signed but **not notarized** by Apple, so the first time you open it
macOS may say *"Sonix is damaged and can't be opened."* It is **not** damaged —
that is just Gatekeeper blocking an app it did not download itself.

1. Unzip `Sonix.app.zip` (it expands to a `Sonix/` folder).
2. Drag `Sonix.app` wherever you want it (e.g. your Applications folder).
3. Double-click **"Open Sonix (first run).command"** in that folder.
   If macOS blocks the `.command` too, right-click it → Open → Open.
4. From then on, just double-click `Sonix.app` normally.

Manual alternative (Terminal):

```bash
xattr -cr /path/to/Sonix.app
```

## Updating

Sonix checks for updates automatically (once a day, on launch) and via
**Help → Check for Updates…** inside the app. When a newer build is published
here, the app offers to download it for you.
