# PR-707 — Odd Rhythm Composer

A skeuomorphic web-based drum machine built for composing in odd time signatures.

**[▶ Live Demo](https://julianfann.github.io/polyrhythm-707/)**

![PR-707](https://img.shields.io/badge/time_signatures-5%2F4_to_15%2F16-ff6b3d) ![Kits](https://img.shields.io/badge/drum_kits-19-1aff5c) ![Patterns](https://img.shields.io/badge/presets-24-ffaa00) ![FX](https://img.shields.io/badge/master_FX-6-1af0ff)

## Features

- **9 odd time signatures** — 5/4, 5/8, 7/8, 7/4, 9/8, 10/8, 11/8, 13/8, 15/16
- **19 drum kits** across three categories:
  - *Classic* — 808, 909, LinnDrum, Oberheim DMX, CR-78, Simmons SDS, SP-1200
  - *Modern* — Modern Analog, Acoustic, Brush Jazz, Industrial, Lo-Fi Tape, Glitch/Digital, Reggaeton, Noise/Ambient
  - *World* — Tabla/Dholak, Middle Eastern, Afro-Latin, Gamelan
- **6-effect master FX chain** — Bitcrusher, Distortion, Filter (LP/HP), Compressor, Delay, Reverb
- **24 genre presets** — Balkan, prog, jazz, dub, Afrobeat, math rock, gamelan, fusion, and more
- **4-state pad system** — Off, on-beat, offbeat (&), or both — doubles rhythmic resolution without visual clutter
- **8 instrument tracks** — Kick, Snare, Hi-Hat, Open HH, Clap, Tom, Rim, Cowbell
- **Swing control** — Add groove feel to any pattern
- **MIDI export** — Standard MIDI file with GM drum mapping, swing timing, and DAW compatibility
- **Beat-up 80s aesthetic** — Skeuomorphic UI with worn chassis, rubber pads, phosphor LCD, screw holes
- **Zero dependencies** — Pure HTML/CSS/JS with Web Audio API synthesis
- **Fully self-contained** — Single file, no build step, no external assets

## Controls

|Control     |Action                               |
|------------|-------------------------------------|
|`Space`     |Play / Stop                          |
|`Click`     |Cycle pad state (off → on → & → both)|
|`[` / `]`   |Previous / Next drum kit             |
|`M`         |Export MIDI file                     |
|Tempo slider|40–240 BPM                           |
|Swing slider|0–80% swing                          |

## FX Chain

Signal path: **Synths → Master Gain → Bitcrusher → Distortion → Filter → Compressor → Delay → Reverb → Output**

Each effect has an on/off toggle and 1–2 parameters. The FX LED on the top panel lights amber when any effect is active.

|Effect|Parameters              |Description                                       |
|------|------------------------|--------------------------------------------------|
|Crush |Bits, Rate              |Sample rate & bit depth reduction                 |
|Dist  |Drive                   |Waveshaper distortion                             |
|Filter|Cutoff, Resonance, LP/HP|Lowpass or highpass with resonance                |
|Comp  |Threshold, Ratio        |Dynamics compressor for punch and glue            |
|Delay |Time, Feedback          |Delay line with feedback loop                     |
|Reverb|Size, Mix               |Algorithmic reverb with generated impulse response|

## Deploy

This is a single `index.html` file. Deploy anywhere:

```bash
# GitHub Pages — just push and enable Pages in repo settings
git init && git add . && git commit -m "init"
git remote add origin git@github.com:<you>/polyrhythm-707.git
git push -u origin main
```

Then go to **Settings → Pages → Source: main branch** → Save.

## License

MIT