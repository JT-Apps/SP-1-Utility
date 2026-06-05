# Release Copy

## Title

SP-1 Utility Alpha for Mac

## Body

### SP-1 Utility Alpha

SP-1 Utility is a Mac app from JT Apps for preparing stem-based songs,
previewing the result, and transferring an album plan to an SP-1 over USB-C.

No terminal, Homebrew, Python setup, or coding tools are required. The app
ships with its local processing engine bundled inside the download.

Download the DMG, open it, and drag **SP-1 Utility** into **Applications**.

### What it does

- Prepares regular songs into SP-1-ready stem files.
- Accepts existing four-stem folders when you already have separated stems.
- Creates 24-bit, 48 kHz, eight-channel WAV files for SP-1 upload.
- Adds prepared songs to a Library view with master and stem previews.
- Transfers ready songs to the SP-1 over USB-C.
- Shows transfer progress based on SP-1 confirmations, not just files being
  read on the Mac.
- Resumes from confirmed progress when a recoverable transfer stall happens.
- Shows a live SP-1 panel for faders, buttons, power, and mode while connected.

### Built for non-technical use

The app is packaged as a normal Mac download. You do not need to install
developer tools, Homebrew, Python, command-line packages, or audio utilities.
Everything needed for normal app use is included in the app bundle.

### Important alpha notes

- This is an alpha build, so please test with a small album first.
- Large transfers can take hours. Keep the SP-1 plugged in and keep the Mac
  awake until the app says the album is complete.
- A song is marked Done only after the SP-1 confirms the write sectors.
- If a song says Needs resend, run Transfer Album again and the app will retry
  the unfinished work.
- Finder and Quick Look may not play the upload WAVs normally because they are
  eight-channel device files. Use the app's Library preview for normal stereo
  listening.

### Mac requirements

- macOS 14 or newer.
- Apple silicon Mac recommended.
- USB-C connection to SP-1.
- Enough free disk space for prepared songs and stems.

### Download

- `SP-1 Utility.dmg`
- `SP-1 Utility.dmg.sha256`

Checksum:

```text
fe6b2d34e922a921dbbac45e08d40e03d847520cdcf5fea77bec4c991473a368
```

### Reporting issues

When reporting an issue, include:

- macOS version.
- App build/date.
- What the toolbar connection status said.
- The song title involved.
- Whether the song row said Done, Ready, Needs resend, or Failed.
- A screenshot of the transfer panel if the issue happened during upload.

### Publisher

SP-1 Utility is published by [JT Apps](https://jtapps.xyz).
