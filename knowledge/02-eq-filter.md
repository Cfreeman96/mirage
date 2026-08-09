# EQ & Filter — EQ Eight, Auto Filter, Utility

_Source: Ableton Live 12 manual. Synced 2026-07-23. See `principles.md` for Cutoff/Resonance, Filter types, Q, Mid/Side, Width/mono._

---

## EQ Eight
**What it is:** An equalizer with up to eight parametric bands per channel, for reshaping a sound's timbre. Your most-used device.

**Key controls:**
- **8 bands**, each with a **filter shape** chooser (bell, low/high shelf, low/high-pass, notch), **Frequency**, **Gain**, and **Q** (width).
- **Processing modes:**
  - **Stereo** — one curve on both channels.
  - **L/R** — independent curves for left and right.
  - **M/S** — independent curves for **Mid** (center/mono) and **Side** (stereo/width). Same tool, different target.
- **Edit switch** — in L/R and M/S, both curves show for reference but only the active one is editable; Edit toggles which.
- **Analyze** — overlays a live spectrum behind the curves.
- **Oversampling** (title-bar menu) — cleaner high-frequency behavior.

**Why two EQ Eights on one track:** they usually do different jobs. **First EQ = subtractive/corrective** (cut rumble, boxiness, harsh resonances) placed *before* compression so the compressor isn't reacting to junk. **Second EQ = additive/tonal** (air, presence) placed *after* dynamics. Fix first, flavor last. Tip: name them "CUT" and "TONE."

**In your track:** EQ Eight is on nearly everything. On the **drum group** you used **M/S** (cut mud from the center while shaping the sides) plus a multiband move. On the bass you "cut sub-100 and above ~1k." On the lead vocals you used "really high Q around 4–5k and 8–10k." *Listen for:* the high-Q cuts remove a specific harshness/resonance without dulling the whole sound — bypass to hear the one nasty frequency return.

**Sources:** [manual](https://www.ableton.com/en/manual/live-audio-effect-reference/)

---

## Auto Filter
**What it is:** A filter that can **move its own cutoff** via an LFO and/or an envelope follower — that's what separates it from a static EQ/filter.

**Key controls:**
- **Filter type** — Low-pass, High-pass, Band-pass, Notch, Morph.
- **Filter circuit** — analog-modeled characters: **SVF** (clean), **DFM** (feeds back distortion — warm drive), **MS2** (Sallen-Key soft-clip, tames resonance), **PRD** (ladder, no resonance limiting). (Circuits apply to LP/HP/BP/Notch/Morph.)
- **Cutoff / Resonance** — the frequency and its emphasis.
- **Drive** — adds distortion/saturation before the filter (0% = clean).
- **LFO** — modulates cutoff rhythmically (rate, waveform, can sync).
- **Envelope follower** — cutoff reacts to the signal's own loudness, or to an **external sidechain**.
- **"Legacy"** — the older filter model from earlier Live versions, kept for compatibility with imported sets (why your course files show it).

**In your track:** you have several automated Auto Filters (a grouped pair on Kick 1, plus on bass and synth), and Auto Filter Legacy twice (carried in from the course project files). *Listen for:* an automated cutoff sweep "opens up" the sound over a build, then releases into the drop — bypass and the movement/tension disappears.

**Sources:** [manual](https://www.ableton.com/en/manual/live-audio-effect-reference/) · [Auto Filter video](https://www.youtube.com/watch?v=7CHuX_V0pD0)

---

## Utility
**What it is:** A humble but essential toolkit device — level, stereo, and mono management.

**Key controls:**
- **Gain** (−∞ to +35 dB) — great for automating volume moves without touching the fader/Volume.
- **Balance** — pan across the stereo field.
- **Width** — stereo spread: 0% = fully mono, >100% = wider.
- **Mid/Side Mode** (Width's right-click menu) — toggles Width for a continuous mono↔stereo control; at 100M sums to mono, at 100S only the side is heard.
- **Bass Mono** — folds low frequencies below a set frequency to mono (solid, phase-safe low end).
- **Mono** — collapse to mono (great mix-check).
- **Channel Mode** — process only L or only R.
- **Phase** (per channel) — invert phase.
- **Mute** — silences input; placed mid-chain it can cut the feed *into* a reverb/delay without killing its tail.
- **DC** — filters sub-audible DC offset (matters before nonlinear effects like compressors/waveshapers).

**In your track:** you used Utility a lot, often with **Gain automation** (a clean way to write fades/level moves), and as part of the **Shaper + 2× Utility** pseudo-sidechain on the bass. *Listen for:* automating Utility Gain creates smooth swells/dips; using Width/Bass-Mono on a wide synth tightens the low end so kick and bass stop fighting.

**Sources:** [manual](https://www.ableton.com/en/manual/live-audio-effect-reference/)

---

## EQ Three
**What it is:** A **DJ-mixer-style** three-band EQ (Low / Mid / High) built for broad moves and full-band **kills** — the opposite of EQ Eight's surgical precision.

**Key controls:**
- **Low / Mid / High gain** — each from **−∞ to +6 dB**. The huge cut range (to silence) with a tiny boost range makes it a *remove/kill* tool, not a boost tool.
- **On/Off (kill) buttons** — per band; instantly cut a band. Great mapped to computer keys or MIDI for live transitions.
- **3 LEDs** — show signal present in each band (threshold −24 dB), even when a band is off.
- **FreqLo / FreqHi crossovers** — set the band boundaries (e.g. Lo 500 Hz, Hi 2 kHz → low 0–500, mid 500–2k, high 2k+).
- **24 dB / 48 dB switch** — slope steepness of the band separation; 48 dB = tighter, cleaner kills with less bleed into neighboring bands.

**Common uses:** DJ-style transitions and drops (kill the bass in a breakdown, slam it back), quick broad tonal sculpting, live performance (map kills to keys), fast removal of a whole frequency range.

**EQ Three vs EQ Eight:** EQ Eight = surgical, 8 parametric bands for detailed mixing/tone. EQ Three = broad 3-band DJ tool for big performance moves and full kills.

**Sources:** [manual (EQ Three)](https://www.ableton.com/en/manual/live-audio-effect-reference/)
