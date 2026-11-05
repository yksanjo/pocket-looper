# Pocket Looper

A minimal five-track loop station in the browser, in the spirit of tabletop loopers like the BOSS RC-505: record a loop, then layer four more tracks in sync. One HTML file, no build, no dependencies, MIT licensed.

**Live app:** https://yksanjo.github.io/pocket-looper/

## Use

1. Enable the microphone (or tap "Try it without a mic" for a built-in demo tone).
2. Press track 1, make a sound, press it again. That sets the loop length and the loop starts playing.
3. Press any other track: it waits for the next loop boundary, records exactly one loop, then plays in sync.
4. Tap a playing track to stop it; tap again to bring it back in sync. Each track has a volume fader and a Clear button. Clear every track to reset the loop length.

Wear headphones to avoid feedback. All audio stays on your device; nothing is uploaded.

## Self test

Open `?selftest=1` (`&fast` shortens the loop) to run an in-page check of record, synced overdub, stop/play, volume, clear and reset. Results log on the page and in `window.__selftest`.

## Left out on purpose

Overdub, effects, undo, MIDI and saving loops. Browser recording latency can put timing a few milliseconds off a hardware unit.
