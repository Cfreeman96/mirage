# Distortion & Character — Roar, Overdrive, Vocoder, Saturator

_Source: Ableton Live 12 manual / release notes. Synced 2026-07-23. See `principles.md` for Dry/Wet, Filter types, LFO, Sidechain, Mid/Side._

---

## Roar
**What it is:** A dynamic saturation device (Live 12 Suite). Ranges from subtle mastering warmth to wild sound-mangling. Because it has so many sections, it's best learned one section at a time.

### 1) Input & Drive/Tone
Before anything, **Drive** and **Tone** shape the incoming signal on its way into the gain stages. Drive pushes level into saturation; Tone tilts the pre-saturation brightness.

### 2) Routing modes (the big structural choice)
Roar routes the signal into one of these topologies:
- **Single** — one shaper/gain stage.
- **Serial** — two shapers in series; **Blend** mixes Stage 1 vs Stages 1+2 combined.
- **Parallel** — two independent shapers; **Blend** crossfades between them (try two very different shaper curves and modulate Blend).
- **Multi Band** — splits into **Low / Mid / High** with two **crossover filters**; saturate each band independently (great for drums and whole mixes).
- **Mid Side** — process the mono (mid) and stereo (side) content independently.
- **Feedback** / **Delay** — feed output back for resonant tails or distorted repetitions/slapbacks.

### 3) Gain Stage tabs (the shaper controls)
Each stage has three controls plus two dropdowns:
- **Shaper Amount** — how much saturation (distortion happens where the signal hits the curve's non-linear parts). You can also drag the waveform display.
- **Shaper Bias** — offsets the signal for *asymmetrical* distortion; higher = "broken circuit" character; extreme = signal goes quiet.
- **Filter Frequency** — a per-stage filter, applied **before or after** the shaper.
- **Shaper Type** dropdown — **12 curves** from subtle to destroyed (e.g. *Soft Sine* = smooth warm saturation, up through harder/noisier/fractal curves).
- **Filter Type** dropdown — the per-stage filter shape.

### 4) Modulation & output
Two **LFOs**, an **Envelope Follower** (with external sidechain), and a **Noise** generator feed an expansive **Modulation Matrix**. Output stage has **Width**, **Compress**, and **Dry/Wet / Output** to fit it into the mix.

**In your track:** you ran Roar in **Multi Band** on your **drum group** (Low/Mid/High). *Listen for:* per-band saturation adds harmonic "grit"/loudness where you dial it — solo the drum group, bypass Roar, and the drums sound cleaner but smaller/flatter; enable it and they get denser and more aggressive, band by band.

**Sources:** [manual](https://www.ableton.com/en/manual/live-audio-effect-reference/) · [Roar video](https://www.youtube.com/watch?v=ETzf6O9-6us) · [Roar Multiband](https://www.youtube.com/watch?v=_ZwzIkmo9Eg)

---

## Overdrive
**What it is:** A distortion effect modeled on classic guitar pedals; can be driven hard without losing dynamic range.

**Key controls:**
- **Band-pass filter (X-Y pad)** — *before* the distortion. Horizontal = band position (frequency), vertical = bandwidth. This decides *which* frequencies get distorted.
- **Drive** — amount of distortion (note: 0% is *not* zero distortion).
- **Tone** — post-distortion EQ; higher = brighter.
- **Dynamics** — how much internal compression rides with the distortion. Low = more compression/makeup as you drive harder; high = less.
- **Dry/Wet** — blend (100% on a return track).

**In your track:** Overdrive is on the bass, synth pluck, and lead (you flagged it as unfamiliar). *Listen for:* the X-Y band decides where the grit lives — park it on the mids and the sound gets a focused "growl"; bypass and the tone gets cleaner but less present/edgy.

**Sources:** [manual](https://www.ableton.com/en/manual/live-audio-effect-reference/)

---

## Vocoder
**What it is:** Combines the **frequency content of a carrier** (a harmonically rich synth/pad) with the **amplitude contour of a modulator** (something rhythmic — speech, drums). Both run through banks of band-pass filters; the modulator's level in each band controls the carrier's level in that band. Classic use: "talking synth"/robot voice. Insert it on the **modulator** track, then pick a carrier.

**Key controls:**
- **Carrier chooser** — *Noise* (with an X-Y for downsampling/density), *External* (route another track — the classic robot-voice option), *Modulator* (resynthesize itself), *Pitch Tracking* (a monophonic osc tuned to the modulator).
- **Bands** — number of filters; more = more accurate spectral analysis (more CPU).
- **Range** sliders + **BW** — the frequency span and bandwidth of the filter bank.
- **Unvoiced** + **Sens.** + **Fast/Slow** — a noise generator that reproduces pitchless sounds ("f", "s"); sensitivity/speed of voiced-vs-unvoiced detection.
- **Enhance** — normalizes the carrier's spectrum/dynamics for a brighter result.
- **Central display** — shows/edits per-band levels.

**Reality check on your note:** you thought Vocoder "boosts mids." It *felt* that way because speech/percussion energy concentrates in the mids, so the carrier gets stamped with mid-focused movement — but the real job is "make the carrier take on the modulator's spectral shape/rhythm."

**In your track:** you used it on the **snare** to lift mids. *Listen for:* the carrier starts "moving" with the modulator's rhythm; bypass and that talking/pulsing spectral motion flattens back to a static tone.

**Sources:** [manual](https://www.ableton.com/en/manual/live-audio-effect-reference/)

---

## Saturator
**What it is:** A **waveshaping** effect that adds dirt, punch, or warmth — from subtle "analog" color to intense coloration. It maps each signal value to a new one along a shaping curve, so it reshapes dynamically based on level. Think of it as the clean, controllable warmth device (vs. Overdrive's pedal grit or Roar's wild saturation).

**Key controls:**
- **Drive** — gain into the shaper; more Drive = more saturation/harmonics (watch it in the Shaper Curve display).
- **Curve Type** (8 choices) — *Analog Clip* (smooth transition around the clip point), *Soft Sine*, *Bass Shaper*, *Medium Curve*, *Hard Curve*, *Sinoid Fold*, *Digital Clip* (immediate hard clipping), *Waveshaper* (unlocks 6 extra controls: Curve, Depth, Linear, Damp, Period…).
- **Color** (toggle) — two "color filters": an EQ applied *before* the shaper and again *inverted after* it. Lets you, e.g., **remove bass before shaping** so only mids/highs saturate while the low-end energy is preserved. **Amt Lo** sets how much the lows get saturated (negative = less).
- **Output** — attenuates the final level (handy to tame boosts from Color).
- **DC** filter + **Dry/Wet**.

**Common uses:** warmth/harmonics on synths, bass, drums, or a whole bus; "analog glue"; pushed harder it becomes outright distortion.

**In your track:** Guido introduced this in Part 2. It's the cousin of your Overdrive and Roar (all add harmonics), but Saturator is the go-to for **clean warmth/color** with precise control. *Listen for:* Drive thickens and adds harmonic richness/loudness; the **Color** trick keeps your sub clean while saturating the mids/highs — bypass and the sound gets thinner and more sterile.

**Sources:** [manual](https://www.ableton.com/en/manual/live-audio-effect-reference/)
