# Loop Gizmo

**Version 1.0**

A 5-track loop station in a single HTML file, modelled on the workflow of a hardware tabletop looper (RC-505mkII style): five synced stereo tracks, overdub, undo/redo, a built-in rhythm machine, and input/track effects.

No install and no dependencies: open `index.html` in Chrome, Edge or Firefox, or use it through GitHub Pages.

## Features

- **5 stereo tracks**, each with a REC/DUB/PLAY pad (with a progress ring), STOP (hold 1 s to clear), a level fader, an FX on/off switch and a TRACK settings button.
- **Loop sync**: the first loop (or the rhythm, if it is running) sets the master length. Later tracks become whole multiples of it, with measure-quantized start and end.
- **Rec action**: REC→DUB→PLAY (default) or REC→PLAY→DUB.
- **Undo/Redo**: one level per track, applied to the last recorded or overdubbed track.
- **Rhythm**: synthesized drums with 7 patterns (Rock, Pop, Funk, Shuffle, Hip-Hop, 4-Floor, Metronome), tap tempo, and phase lock to the loops. The tempo is derived automatically from a free-recorded first loop.
- **Input FX** (A–D) and **Track FX** (A–D): Filter, Delay, Reverb, Lo-Fi and Ring Mod. EDIT changes the type of the selected bank; the big knob sets the amount.
- **Track settings**: reverse, one-shot, pan, import of an audio file, and export of the track as a WAV file.
- **Latency compensation** for overdubs (AUTO or a fixed value in ms).
- Sample-accurate audio engine running in an AudioWorklet.

## Controls

| Control | Action |
|---|---|
| Track pad / `1`–`5` | Record → overdub → play (empty track: start recording; stopped track: play) |
| STOP / `Q` `W` `E` `R` `T` | Stop track; hold 1 s to clear it |
| ALL START/STOP / `Space` | Stop everything, or restart all tracks from the top |
| UNDO/REDO / `Z` | Undo the last pass; press again to redo |
| RHYTHM START/STOP / `B` | Rhythm on/off |
| TAP TEMPO / `G` | Tap tempo (only while no loop exists) |
| RHYTHM EDIT | Next rhythm pattern |
| MENU | System page: input monitor, microphone, pattern, tempo |
| LOOP | Loop page: rec action, rec quantize, latency compensation |
| TRACK | Track page for that track |
| ◀ ▶ / arrow keys | Move the LCD cursor (main page: select track) |
| ENTER / `Enter`, EXIT / `Esc` | Change the item / back to the main page |
| Middle knobs | Tempo, rhythm level, input level, pan of the selected track |

Knobs and faders respond to vertical dragging or the mouse wheel; double-click resets them. You can also click LCD menu items directly: click = next value, right-click or Shift-click = previous value. Drop an audio file on a track strip to load it.

## Notes

- Use **headphones** when recording from a microphone. With INPUT MONITOR off (default), you only hear the input once it has been recorded.
- The browser asks for microphone or audio-interface access when you press POWER ON. Auto gain, noise suppression and echo cancellation are turned off for a clean signal.
- If overdubs land late, set LATENCY COMP on the LOOP page to a fixed value.
- Loops live in memory only and are lost when you reload the page. Export a track as WAV to keep it.

## Version history

- **1.0** — First release.
