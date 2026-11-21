# Loop Gizmo — Owner's Manual

**Version 2.0**

▶ **Live version: [https://droogia.github.io/loop-gizmo/](https://droogia.github.io/loop-gizmo/)**

Loop Gizmo is a 6-track loop station that runs in a web browser. It follows the workflow of a hardware tabletop looper: record a phrase, layer more on top, stack parts on separate tracks, add a drum rhythm, and shape everything with effects in real time.

---

## Contents

1. [Getting started](#1-getting-started)
2. [Tutorial — your first loop session](#2-tutorial--your-first-loop-session)
3. [Panel reference](#3-panel-reference)
4. [Tracks in depth](#4-tracks-in-depth)
5. [Loop sync, quantize and tempo](#5-loop-sync-quantize-and-tempo)
6. [Rhythm machine](#6-rhythm-machine)
7. [Effects](#7-effects)
8. [LCD menus](#8-lcd-menus)
9. [Import and export](#9-import-and-export)
10. [Keyboard shortcuts](#10-keyboard-shortcuts)
11. [Latency and audio setup](#11-latency-and-audio-setup)
12. [Troubleshooting](#12-troubleshooting)
13. [Technical notes](#13-technical-notes)

---

## 1. Getting started

### 1.1 Requirements

a) A desktop browser: Chrome, Edge or Firefox (recent versions). Safari may work but is not tested.

b) An audio input: a built-in or USB microphone, or an audio interface with a guitar, synth or mic plugged in.

c) **Headphones** are strongly recommended when you record from a microphone. Otherwise the speakers feed back into your loops.

### 1.2 Opening the looper

a) **Online:** open the [live version](https://droogia.github.io/loop-gizmo/).

b) **Offline:** download `index.html` from the repository and double-click it. Everything is in that one file, with no installation and no internet connection needed.

### 1.3 Powering on

When the page opens, it shows the **⏻ POWER ON** screen. Browsers only allow audio after you click something, and this is that click.

a) Click **POWER ON**.

b) The browser asks for microphone access. Allow it. If you have several inputs (for example an audio interface), the browser uses its default input. Pick a different one in the browser's site settings (the icon next to the address bar), then use **MENU → MICROPHONE** to reconnect.

c) The LCD shows `MIC: <device name>` when the input works, or `MIC N/A` if access was refused. Without a mic you can still use the rhythm machine and load audio files onto tracks.

### 1.4 Checking the input level

a) Make a sound. The **IN** meter on the LCD moves.

b) Adjust the third middle knob, **IN.LV**, so loud notes fill most of the meter without staying pinned at the end.

c) To hear your live input through the looper, turn on **MENU → INPUT MONITOR**. Leave it off if your interface already provides direct monitoring.

---

## 2. Tutorial — your first loop session

This walk-through builds a short piece with drums, a bass line, chords, a melody and an effect sweep. It uses keyboard shortcuts, but each one has an on-screen button (see section 10).

### Lesson 1 — Free loop, no drums

a) Press **`1`** (or click the big pad on track 1). The ring around the pad turns **red** and blinks: you are recording.

b) Play a phrase of a few seconds — a chord progression, a beat on the table, anything.

c) Press **`1`** again exactly where the phrase should loop. The ring turns **yellow**: track 1 now loops what you recorded and you are **overdubbing** (adding on top).

d) Play a second layer on top of the loop.

e) Press **`1`** once more. The ring turns **green**: plain playback, nothing is recorded.

f) Press **`Q`** (or track 1's ■ STOP button) to stop the track. Press **`1`** to start it again.

> The length of this first loop is now the **master loop**. The tempo on the LCD has been calculated from it, and every later track lines up with it.

### Lesson 2 — Undo and redo

a) With track 1 playing, press **`1`** to overdub and add something you don't like.

b) Press **`Z`** (UNDO/REDO). The last overdub pass disappears.

c) Press **`Z`** again to bring it back (redo). Press it a third time to remove it again.

Undo works on the **last track you recorded or overdubbed**, and it remembers one pass. The UNDO/REDO button lights up when there is something to undo or redo.

### Lesson 3 — Clearing

Hold **`Q`** (or track 1's ■ button) for one second. The LCD shows `TRACK 1 CLEARED`. Once every track is empty, the master loop resets and the next recording sets a new length.

### Lesson 4 — Starting with the drums

a) Press **RHYTHM EDIT** a few times to choose a pattern. Its name shows at the top right of the LCD.

b) Set the tempo: turn the first middle knob (**TEMPO**), or tap **`G`** (TAP TEMPO) four times in time. The TAP TEMPO button blinks on every beat.

c) Press **`B`** (RHYTHM START/STOP). The drums play and the LCD counts `MEAS` and `BEAT`.

d) Balance the drums with the second middle knob (**RHY.LV**).

While the rhythm runs, **one bar of the rhythm is the master loop**, and every recording becomes a whole number of bars.

### Lesson 5 — Building a song in layers

With the rhythm running:

a) **Bass on track 1:** press **`1`** just before a bar starts. With **REC QUANTIZE** set to MEASURE (the default), the ring blinks **orange (WAIT)**, and recording starts exactly on the next downbeat. Play two bars of bass.

b) Press **`1`** near the end of bar two. Recording continues to the bar line and then switches to overdub/play. Whether you press a little early or a little late, the loop snaps to whole bars.

c) Press **`1`** again if you want plain playback.

d) **Chords on track 2:** press **`2`** and play four bars. Track 2 can be longer than track 1: the tracks stay in phase, and track 1 simply repeats twice under track 2.

e) **Melody on track 3:** press **`3`**, play, and press **`3`** to close it.

f) **Mix:** use each track's **fader** for level, and click **TRACK** on a strip then turn the fourth middle knob (**PAN**) to place it in the stereo field.

### Lesson 6 — Performing with effects

a) Click track 2's **FX** button so it lights up. Track 2 now goes through the Track FX.

b) Choose bank **A** on the right side (TRACK FX). By default it is **FILTER**.

c) Turn the big **TRACK FX** knob down and up slowly: the chords sweep from muffled to open.

d) Press **EDIT** above it to change bank A's type. Try **FLANGER**, then **WAH-WAH**. With WAH-WAH, the big knob works like the pedal: rock it back and forth.

e) Now an **input effect**: click **C** on the left side (INPUT FX), and press the left **EDIT** until it reads **TRANSPOSE**. Set the left big knob to **−12 st**. Anything you play is now an octave lower, so you can record an octave bass line with a guitar. Click **C** again to turn the input effect off.

### Lesson 7 — Arrangement and ending

a) **Breakdown:** press **`W`** and **`E`** to stop tracks 2 and 3, leaving drums and bass.

b) **Build-up:** press **`2`** and **`3`** to bring them back in. They come back in phase.

c) **Reverse trick:** click **TRACK** on track 3, select **REVERSE** with ◀ ▶ and press **ENTER**. The melody plays backwards. Press **EXIT** to leave the page.

d) **Ending:** press **Space** (ALL START/STOP). Every track and the rhythm stop together. Press **Space** again to restart everything from the top of the loop.

e) **Keep your work:** for each track, click **TRACK → EXPORT WAV** to save a `.wav` file.

You have now used all the main features. The sections below cover each control in detail.

---

## 3. Panel reference

### 3.1 Top section

| Control | Function |
|---|---|
| **INPUT FX big knob** (left) | Amount (or semitones / pedal position) of the selected input FX bank |
| **INPUT FX EDIT** | Cycles the effect type of the selected input bank |
| **MENU** | Opens/closes the SYSTEM MENU page on the LCD |
| **LOOP** | Opens/closes the LOOP SETTINGS page |
| **LCD** | Status display and menus (section 8) |
| **EXIT ✕** | Back to the main LCD page |
| **ENTER ●** | Changes the selected menu item; on the main page it opens the selected track's page |
| **◀ ▶** | On the main page: select the previous/next track. In menus: move the cursor |
| **OUTPUT LEVEL** | Master volume |
| **RHYTHM EDIT** | Next rhythm pattern |
| **TRACK FX EDIT** | Cycles the effect type of the selected track FX bank |
| **TRACK FX big knob** (right) | Amount of the selected track FX bank |

### 3.2 Middle row

| Control | Function |
|---|---|
| **INPUT FX A B C D** | Select and switch on an input FX bank. Click the lit bank again to switch input FX off |
| **ALL START/STOP** | Stops all tracks and the rhythm; pressed again, restarts every track that has content (and the rhythm, if it was running) from the top |
| **UNDO/REDO** | Undoes the last recording/overdub pass; pressed again, redoes it |
| **TEMPO knob** | Rhythm tempo (40–250 BPM). Locked once a loop exists |
| **RHY.LV knob** | Rhythm volume |
| **IN.LV knob** | Input gain (before the input FX) |
| **PAN knob** | Pan of the selected track (shown as `PAN n`) |
| **TAP TEMPO** | Tap at least twice to set the tempo; blinks on every beat |
| **RHYTHM START/STOP** | Starts/stops the drums |
| **TRACK FX A B C D** | Selects which track FX bank is active for every track whose FX button is on |

### 3.3 Track strips (1–6)

| Control | Function |
|---|---|
| **FX** | Routes this track through the active Track FX bank |
| **TRACK** | Selects the track and opens its settings page on the LCD |
| **■ STOP** | Stops the track. **Hold 1 s to clear it** |
| **Fader** | Track playback level |
| **Length readout** | Loop length in seconds and in bars |
| **Big pad** | Record / overdub / play (see 4.1) |
| **Ring** | Shows state and loop position (see 4.2) |

All knobs and faders respond to **vertical drag** or the **mouse wheel**. Hold **Shift** while dragging a knob for fine adjustment. **Double-click** resets a knob or fader to its default.

---

## 4. Tracks in depth

### 4.1 What the big pad does

The result of a press depends on the track's current state and on **REC ACTION** (LOOP page).

| Current state | REC→DUB→PLAY (default) | REC→PLAY→DUB |
|---|---|---|
| Empty | Start recording | Start recording |
| Recording | Close the loop → **overdub** | Close the loop → **play** |
| Overdubbing | → Play | → Play |
| Playing | → Overdub | → Overdub |
| Stopped | → Play | → Play |

A **one-shot** track (see 4.4) is different: each press restarts it from the beginning, and it does not overdub.

### 4.2 Ring colours

| Ring | Meaning |
|---|---|
| Dark | Empty |
| **Red**, blinking | Recording the first loop (free length) |
| **Red**, filling up | Recording synced to the master loop |
| **Orange**, blinking | WAIT: recording starts on the next bar line |
| **Yellow**, filling up | Overdubbing |
| **Green**, filling up | Playing; the filled arc is the position in the loop |
| Grey | Stopped (it still holds audio) |

The text under the pad repeats the state. During a synced recording that you have already closed, it shows what comes next (for example `REC → DUB`).

### 4.3 Overdubbing

Overdub adds new audio on top of the existing loop. The loop length never changes during an overdub. Every overdub pass (from entering DUB until you leave it) is one undo step.

### 4.4 Track settings (TRACK page)

| Item | Values | Effect |
|---|---|---|
| REVERSE | ON / OFF | Plays the loop backwards. Overdubs on a reversed track are written backwards too, so they line up with what you hear |
| ONE SHOT | ON / OFF | The track plays once from the start each time you press its pad, then stops. Good for samples and stings |
| TRACK FX | ON / OFF | Same as the strip's FX button |
| PAN | L50 … C … R50 | Same as the PAN knob. ENTER / click steps through values |
| IMPORT AUDIO… | — | Loads an audio file onto this track (section 9) |
| EXPORT WAV | — | Saves this track as a 16-bit stereo WAV (section 9) |

### 4.5 Stopping and clearing

a) **Stop:** short press on ■ (or `Q` `W` `E` `R` `T` `Y`). If the track is recording, the loop closes first and then stops.

b) **Clear:** keep ■ held for 1 second. This also discards the track's undo/redo memory.

c) When every track is cleared (and the rhythm is off), the master loop resets.

---

## 5. Loop sync, quantize and tempo

### 5.1 The master loop

All tracks share one timeline, the **master loop**. It is set in one of two ways:

a) **By the first recording**, if the rhythm is not running. The phrase you record defines the master length, and the tempo is worked out by assuming the loop holds a whole number of 4/4 bars. The looper picks the number of bars that puts the tempo at 75 BPM or above, so a 2-second loop becomes 1 bar at 120 BPM, and a 6-second loop becomes 2 bars at 80 BPM.

b) **By the rhythm**, if you start the drums before recording anything. The master is then one bar at the current tempo.

The LOOP page shows the master length in seconds and bars (`LOOP LENGTH`).

### 5.2 Synced recording

Once a master loop exists, every new recording:

a) **Starts** on a bar line (the start of the master loop), if REC QUANTIZE is MEASURE. If you press during roughly the first 12 % of the loop, recording starts immediately from that loop's start, so a slightly late press still catches the downbeat. Otherwise the track waits (orange) for the next loop start.

b) **Ends** on a whole multiple of the master length. A press in roughly the first 12 % of a new cycle rounds down; any later press rounds up and keeps recording to the next boundary.

With REC QUANTIZE **OFF**, recording starts at once. The part of the loop before your press is silent, and the end is still rounded to a whole multiple.

### 5.3 Phase

Tracks never drift apart: each one always plays the part of its loop that matches the shared timeline. A track that is twice the master length plays its first half and then its second half while a one-master-length track repeats twice.

### 5.4 Restarting from the top

When nothing is playing (all tracks stopped, rhythm off), the next start (a single track, ALL START, or the rhythm) **resets the timeline**, so playback begins at the top of the loop.

### 5.5 Tempo

a) Tempo can only change while **no loop exists**. After that, the LCD shows `TEMPO LOCKED`, because changing the tempo would change the loop lengths.

b) TAP TEMPO takes the average of the taps made within 2.5 seconds of each other.

c) The DELAY and FLANGER effects follow the tempo: the delay repeats on a dotted eighth note, and the flanger sweeps over two bars.

---

## 6. Rhythm machine

### 6.1 Patterns

| Pattern | Description |
|---|---|
| ROCK | Straight 8th hi-hats, kick on 1, 3 and the "and" of 3 |
| POP | 16th hi-hats, syncopated kick |
| FUNK | Busy kick and ghost snares, open hat |
| SHUFFLE | Swung 8ths (triplet feel) |
| HIPHOP | Laid-back kick with a light swing |
| 4 FLOOR | Kick on every beat, open hats on the off-beats |
| METRO | Metronome click, accented on the first beat of each loop |

Press **RHYTHM EDIT**, or use **MENU → RHYTHM PATTERN**, to change the pattern. The change takes effect immediately, even while the rhythm is playing.

### 6.2 How the rhythm follows the loops

The rhythm is locked to the master loop. If you start it while tracks are playing, it joins in time. If the first loop was recorded freely, the drums use the tempo and bar count worked out from it (5.1).

The drum sounds are synthesized live (kick, snare, closed and open hi-hat, click), so there are no samples to load.

---

## 7. Effects

### 7.1 Input FX vs Track FX

a) **Input FX** process what you play **before it is recorded**. The effect becomes part of the loop. Example: record a bass line through TRANSPOSE −12.

b) **Track FX** process a track's **playback**. The recording itself stays clean, and you can change or remove the effect at any time. Each track opts in with its **FX** button. All opted-in tracks use the active bank (A–D).

Each section has four banks. Every bank holds an effect type, which you change with **EDIT**, and its own knob setting.

Default banks:

| Bank | Input FX | Track FX |
|---|---|---|
| A | REVERB | FILTER |
| B | DELAY | DELAY |
| C | RING MOD | REVERB |
| D | LO-FI | LO-FI |

### 7.2 Effect types

| Type | What the big knob controls | Notes |
|---|---|---|
| **FILTER** | Cutoff of a resonant low-pass: fully left = open, fully right = closed | Classic DJ-style sweep |
| **DELAY** | Wet level and number of repeats | Tempo-synced dotted 8th, darkened repeats |
| **REVERB** | Reverb amount | About a 2.4 s hall |
| **LO-FI** | Bit depth (16 → 3 bits) and bandwidth | From slightly gritty to heavily crushed |
| **RING MOD** | Carrier frequency (30–930 Hz) | Metallic or robotic tones |
| **FLANGER** | Intensity (depth, feedback, mix) | Jet-plane sweep over 2 bars |
| **WAH-WAH** | **Pedal position**: left = heel (dark), right = toe (bright) | Rock the knob like a pedal |
| **TRANSPOSE** | Pitch in semitones, −12 … +12 (centre = 0) | Pitch shift that keeps the length; double-click the knob for 0 |

The value under each big knob shows the setting in the effect's own units: `%`, `PEDAL %`, or `±n st`.

### 7.3 Tips

a) **Octave layers:** record a part, then overdub it again with input TRANSPOSE +12 for a 12-string or organ feel.

b) **Wah sweeps:** set a track FX bank to WAH-WAH and move the knob in time with the beat.

c) **Breakdowns:** put FILTER on every track (FX on), then sweep the cutoff down over four bars and snap it back open on the drop.

d) **Reverse + reverb:** set REVERSE on a track and add REVERB from the track FX for ghostly swells.

---

## 8. LCD menus

### 8.1 Main page

```
MEMORY 01          ♩=120.0          ROCK ▶
[1 P][2 D][3  ][4  ][5  ][6 S]          ← track states (R/D/P/S/W)
[■■■■■■■■■■■■·········]                 ← master loop position
MEAS 01/02  BEAT 3            IFX:REVERB
IN ▮▮▮   OUT ▮▮▮▮▮           MIC: ...
TEMPO   RHY.LV 60   IN.LV 80   PAN1 C   ← middle knob labels
```

Highlighted track boxes are active. When the selected track is empty, its box is highlighted too.

### 8.2 Navigating

a) **◀ ▶** or the **arrow keys** move the cursor.

b) **ENTER** changes the selected item to the next value.

c) **Click** an item for the next value; **right-click** or **Shift-click** for the previous value. The **mouse wheel** over an item also changes it.

d) **EXIT** or **Esc** returns to the main page.

### 8.3 LOOP SETTINGS (LOOP button)

| Item | Values |
|---|---|
| REC ACTION | REC→DUB→PLAY / REC→PLAY→DUB |
| REC QUANTIZE | MEASURE / OFF |
| LATENCY COMP | AUTO, or 0 … 100 ms |
| LOOP LENGTH | Master length (display only) |

### 8.4 SYSTEM MENU (MENU button)

| Item | Values |
|---|---|
| INPUT MONITOR | ON / OFF: hear the live input |
| MICROPHONE | Shows the device; ENTER disconnects or reconnects |
| RHYTHM PATTERN | Pattern list |
| RHYTHM TEMPO | ENTER / click adds 1 BPM, right-click subtracts |

### 8.5 TRACK page (TRACK button)

See 4.4.

---

## 9. Import and export

### 9.1 Importing audio

Drop an audio file (WAV, MP3, OGG, FLAC, M4A — anything your browser can decode) **onto a track strip**, or use **TRACK → IMPORT AUDIO…**.

a) If no master loop exists, the file's length becomes the master loop.

b) If a master loop exists, the file is padded or trimmed to the nearest whole multiple of it.

c) The track is left **stopped**. Press its pad to play it.

d) Importing can be undone with UNDO.

### 9.2 Exporting

**TRACK → EXPORT WAV** saves the selected track as `loop-gizmo-trackN.wav` (16-bit stereo, at the browser's sample rate). If REVERSE is on, the exported file is reversed too. Track FX, fader and pan are **not** included in the export.

> Loops are kept only in the browser's memory. **Reloading or closing the page erases them.** Export anything you want to keep.

---

## 10. Keyboard shortcuts

| Key | Action | On-screen equivalent |
|---|---|---|
| `1` … `6` | Record / overdub / play track 1–6 | Big pad |
| `Q` `W` `E` `R` `T` `Y` | Stop track 1–6; hold 1 s to clear | ■ button |
| `Space` | All start/stop | ALL START/STOP |
| `Z` | Undo / redo | UNDO/REDO |
| `B` | Rhythm start/stop | RHYTHM START/STOP |
| `G` | Tap tempo | TAP TEMPO |
| `←` `→` `↑` `↓` | Track select / menu cursor | ◀ ▶ |
| `Enter` | Enter | ENTER |
| `Esc` | Exit to main page | EXIT |

Shortcuts are ignored while Ctrl, Alt or Cmd is held, so browser shortcuts keep working.

---

## 11. Latency and audio setup

### 11.1 Why overdubs can land late

Sound takes time to travel from the looper to your ears (output latency) and from your instrument into the looper (input latency). When you play along with a loop, what you record therefore arrives slightly late. **LATENCY COMP** moves overdubs and synced recordings earlier by that amount.

a) **AUTO** uses the latency the browser reports, plus a small margin. The value in use is shown next to it.

b) If overdubs still sound late (flammy), choose a larger fixed value. If they sound early, choose a smaller one.

c) **Calibration tip:** start the METRO pattern, record a track of hand claps exactly on the clicks, and play it back with the rhythm. Adjust LATENCY COMP until the claps and the clicks sound like one sound.

### 11.2 Lower latency

a) **Windows:** use Chrome or Edge with your audio interface set as the default device, at a low buffer size in its control panel. Close other audio-heavy applications.

b) Bluetooth headphones add a lot of latency (often 150 ms or more). Use wired headphones for recording.

### 11.3 Clean input

The looper asks the browser to turn off echo cancellation, noise suppression and automatic gain. These features are built for voice calls and degrade music.

---

## 12. Troubleshooting

| Problem | Solution |
|---|---|
| `MIC N/A` on the LCD | Allow microphone access for the page (the icon next to the address bar), then **MENU → MICROPHONE → ENTER** |
| Wrong input device | Change the site's microphone in the browser settings, then reconnect via **MENU → MICROPHONE** |
| Howling feedback | Use headphones, or turn **INPUT MONITOR** off |
| Hear the input twice | Turn INPUT MONITOR off when your interface already monitors directly |
| Overdubs out of time | Adjust **LATENCY COMP** (11.1) |
| `TEMPO LOCKED` | Tempo only changes while no loop exists. Clear all tracks (and stop the rhythm, if the master came from a recorded loop) |
| Recording didn't start | The ring is probably blinking orange (WAIT): it starts at the next bar line. Turn off REC QUANTIZE for an instant start |
| Glitch when starting an overdub on a very long loop | The undo copy of a long loop is made at that moment. Keep loops under about a minute, or overdub less often |
| No sound at all | Check OUTPUT LEVEL and the track faders, and make sure you clicked POWER ON |
| "Audio engine failed" | Use an up-to-date Chrome, Edge or Firefox |

---

## 13. Technical notes

a) **Engine:** a custom AudioWorklet processor runs all six tracks with sample-accurate timing. Recording, overdubbing, quantized starts and ends, and undo snapshots all happen on the audio thread. Every track has its own stereo output, routed through its FX insert, fader, panner and the master limiter.

b) **TRANSPOSE:** a second AudioWorklet processor that does granular pitch shifting with two overlapping read heads crossfaded by power-complementary windows (60 ms grains).

c) **Memory:** each second of stereo audio takes about 0.4 MB per track at 48 kHz, plus one undo copy per track.

d) **Single file:** all code, styles and sounds are inside `index.html`. Nothing is loaded from the network.

---

*Loop Gizmo is an independent project and is not affiliated with any hardware manufacturer.*
