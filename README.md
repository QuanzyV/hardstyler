# ⚡ HARDSTYLER ⚡

Turn **any song** into a hardstyle remix, right in your browser. Drop a track in, it finds the beat, and lays a pumping hardstyle kick on top.

### 👉 [**Use it live here**](https://quanzyv.github.io/hardstyler/)

No install, no sign-up, no upload. **100% offline** — your audio never leaves your machine; all the processing happens locally in your browser.

---

## How to use

1. Open the [live link](https://quanzyv.github.io/hardstyler/) (works best in **Chrome** or **Edge**).
2. **Drag a song** onto the drop zone (`mp3`, `wav`, `m4a`, `ogg`, `flac`).
3. It analyzes the track and shows the detected **BPM** + a waveform with the **beats marked** in magenta.
4. Tweak the sliders — or just smash **🚀 FULL SEND** for the cranked preset.
5. Hit **⚡ HARDSTYLE IT ⚡**, A/B the result against the original, and **download the `.wav`**.

## What it actually does

Hardstyle is a famously formulaic genre, so this applies the recipe with real DSP (no AI, no training):

- **Beat detection** — spectral-flux onset detection → autocorrelation tempo estimation → an Ellis-style dynamic-programming beat tracker, so the kick lands **on the beat**, not on a dumb metronome grid.
- **Speed / pitch lift** — the euphoric pitched-up "edit" sound.
- **Synthesized distorted kick** — a punchy 170→45 Hz kick placed on every detected beat (with smart density: it auto-doubles to 8th-notes on slower songs).
- **Saturation, sidechain pump, and reverb** — the gritty, breathing, euphoric character.

## Controls

| Control | What it does |
|---|---|
| 🔥 Intensity | Overall hardness / distortion / pump depth |
| 🎤 Pitch / Speed | How far the track is pitched + sped up |
| 💥 Kick Volume | Loudness of the added kick |
| 🌌 Reverb | Euphoric space / tail |
| 🥁 Kick pattern | Auto / every beat / double-time / half-time |

## Honest expectations

It's a fun, real **edit** — not a studio master or an AI cover. On tracks with a weird intro or a tempo change, glance at the magenta beat-lines on the waveform; if they drift, nudge the **Kick pattern** or trim the song. Most four-on-the-floor tracks lock in great.

## Run it locally

Just download `index.html` and double-click it. That's the whole app — one file.

## License

MIT — see [LICENSE](LICENSE). Go nuts.
