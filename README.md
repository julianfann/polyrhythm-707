# PR-707 — Odd Rhythm Composer

A skeuomorphic web-based drum machine built for composing in odd time signatures.

**[▶ Live Demo](https://<your-username>.github.io/polyrhythm-707/)**

![PR-707](https://img.shields.io/badge/time_signatures-5%2F4_to_15%2F16-ff6b3d) ![Kits](https://img.shields.io/badge/drum_kits-8-1aff5c) ![Patterns](https://img.shields.io/badge/presets-24-ffaa00)

## Features

- **9 odd time signatures** — 5/4, 5/8, 7/8, 7/4, 9/8, 10/8, 11/8, 13/8, 15/16
- **8 drum kits** — 808, 909, LinnDrum, Oberheim DMX, CR-78, Acoustic, Industrial, Lo-Fi Tape
- **24 genre presets** — Balkan, prog, jazz, dub, Afrobeat, math rock, gamelan, fusion, and more
- **8 instrument tracks** — Kick, Snare, Hi-Hat, Open HH, Clap, Tom, Rim, Cowbell
- **Swing control** — Add groove feel to any pattern
- **Beat-up 80s aesthetic** — Skeuomorphic UI with worn chassis, rubber pads, phosphor LCD, screw holes
- **Zero dependencies** — Pure HTML/CSS/JS with Web Audio API synthesis
- **Fully self-contained** — Single file, no build step, no external assets

## Controls

| Control | Action |
|---------|--------|
| `Space` | Play / Stop |
| `Click` | Toggle pad on/off |
| `1`–`8` | Switch drum kits |
| Tempo slider | 40–240 BPM |
| Swing slider | 0–80% swing |

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
