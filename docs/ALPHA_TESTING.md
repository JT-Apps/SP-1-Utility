# SP-1 Utility Alpha Testing

This checklist is for early testers running SP-1 Utility on a real SP-1.

## Before Testing

- Install the latest signed DMG build.
- Plug the SP-1 into USB-C and put it in transfer mode.
- Keep the Mac awake for long transfers.
- Use short test albums first, then move to larger albums.
- If anything feels stuck, take a screenshot before restarting.

## What To Test

### Prepare

- Drag in one song and confirm it appears in the queue.
- Drag in multiple songs and confirm all are queued.
- Run Prepare all and confirm every completed song appears in Library.
- Confirm unsupported files show a visible import message instead of silently
  doing nothing.

### Library

- Confirm prepared songs appear without needing a manual refresh.
- Play the master preview.
- Play each stem preview.
- Confirm the compatibility label says SP-1 ready only for 24-bit, 48 kHz,
  eight-channel PCM WAVs.

### Upload

- Import ready WAVs or drag them into Upload.
- Confirm rows show clean song titles, duration, BPM, and size.
- Confirm the Transfer Album button sends every ready song in the list.
- Use Edit Selected Song only for title, artist, BPM, and one-song actions.
- During transfer, confirm the panel shows current song, confirmed sectors,
  current write speed, retry count, and stop/recovery status.

## Transfer Expectations

Large albums can take hours. The app should stay truthful while it works:

- Done means the SP-1 confirmed the song sectors.
- Needs resend means the local plan has not been fully confirmed on the device.
- Recovering means the app is reconnecting and preparing to resume.
- Album complete means every ready song in the current album plan was confirmed.

## Report Format

When reporting an issue, include:

- macOS version.
- App version or build date.
- SP-1 connection state shown in the toolbar.
- Song title and row status.
- Transfer panel text if a transfer was running.
- Whether the SP-1 itself appeared to keep writing.
- Any Console or trace file the app produced.

## Good Screenshots To Attach

- The toolbar connection chip.
- The Upload transfer panel.
- The song row that says Done, Ready, Needs resend, Failed, or Missing file.
- The Library detail panel if the issue is about playback or stems.

## Known Alpha Limits

- Stem separation quality depends on the source material.
- Finder and Quick Look may not play upload WAVs normally because they are
  eight-channel files.
- Full-device transfers are slow by design; a reliable confirmed transfer is
  more important than a fast-looking progress bar.
