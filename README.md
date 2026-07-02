# Single‑Key Piano

A minimal web‑based piano that plays notes using only one key (the spacebar).
Each press of the spacebar (or click on the virtual key) plays the next note in the C major scale, cycling through C4,
D4, E4, F4, G4, A4, B4, C5 and then back to C4.

## How to use

1. Open `piano.html` in any modern browser (Chrome, Edge, Firefox, Safari).
2. Press the **spacebar** or **click** the white key on the screen.
3. A different note will play each time, and the name of the note is shown below the key.

## Features

- Uses the Web Audio API to generate sine‑wave tones.
- No external libraries or dependencies.
- Works offline (just the HTML file).
- Visual feedback: the key lights up briefly when pressed.

## Technical details

- The scale is hard‑coded as an array of note names and frequencies.
- The audio context is created on the first user interaction to comply with browser autoplay policies.
- The oscillator type is `sine`; you can change it to `triangle`, `sawtooth`, or `square` by editing the `osc.type` line
in the script.
