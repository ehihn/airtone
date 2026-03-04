<div align="center">

# ✋ AirTone

**Shape sound with your hands.**

A camera-controlled synthesizer that uses real-time hand tracking to turn your gestures into music. No MIDI controller, no keyboard — just your hands and a webcam.

[**Try it live →**](https://ehihn.github.io/airtone)

</div>

---

## How It Works

AirTone uses **MediaPipe Hand Landmarks** to track both hands via your webcam, and maps your gestures to a **Web Audio API** synthesizer in real time.

| Hand | Gesture | Controls |
|------|---------|----------|
| ✊ Left | Fist open/close | Filter cutoff (20 Hz → 12,000 Hz) |
| ✊ Left | ~30% open sweet spot | Resonance peak (squelchy acid sound) |
| 👋 Right | Move left/right | Legato note selection (chromatic) |
| ✊ Right | Fist close | Vibrato intensity & speed |

## Features

- **Two-hand control** — left hand shapes the filter, right hand plays notes
- **Legato mode** — smooth 150ms glide between notes
- **Vibrato** — close your right fist for expressive pitch wobble
- **4 waveforms** — Sawtooth, Square, Sine, Triangle
- **Multi-oscillator** — stack 1–3 oscillators with detune spread for fat unison sounds
- **Reverb & Delay** — toggle on/off for atmospheric textures
- **5 octave range** — from deep sub bass to piercing leads
- **Dual-ring visualizer** — inner ring (purple) reacts to filter, outer ring (green) reacts to pitch
- **Zero dependencies** — single HTML file, no build step, no install

## Quick Start

1. Open [**ehihn.github.io/airtone**](https://ehihn.github.io/airtone) in Chrome
2. Allow camera access
3. Wait for the hand model to load
4. Click **Start Synth**
5. Raise both hands and play!

## Tips

- **Sawtooth + filter sweep** = the most dramatic sound. Slowly open your left fist.
- **Octave 1–2 + Sawtooth** = acid bass. Keep your left fist around 20–40% open where resonance peaks.
- **3 Osc mode** = instant supersaw. Try it with reverb + delay for huge ambient pads.
- **Good lighting** helps tracking. Avoid backlighting.
- **Smooth, deliberate movements** sound more musical than jerky ones.

## Tech Stack

- [MediaPipe Hand Landmarker](https://developers.google.com/mediapipe/solutions/vision/hand_landmarker) — real-time hand tracking
- [Web Audio API](https://developer.mozilla.org/en-US/docs/Web/API/Web_Audio_API) — synthesizer engine
- Vanilla HTML/CSS/JS — no frameworks, no build tools

## Roadmap

- [ ] Scale lock — snap to major, minor, pentatonic, blues scales
- [ ] Multi-oscillator independent waveforms — different waveform per oscillator
- [ ] Formant filter — vowel-shaping texture control
- [ ] MIDI output — control DAW plugins with your hands

## Requirements

- Google Chrome (recommended)
- Webcam
- Speakers or headphones

---

<div align="center">

Built with 🤚 by [ehihn](https://github.com/ehihn)

</div>
