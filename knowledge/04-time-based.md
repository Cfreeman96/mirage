# Time-Based — Delay, Echo, Reverb

_Source: Ableton Live 12 manual. Synced 2026-07-23. See `principles.md` for Dry/Wet, Sync divisions, Feedback, Filter types._

---

## Delay
**What it is:** A clean, straightforward digital delay with two channels, sync, filtering, and modulation. (Live also has the deeper **Echo** — see below — when you want character.)

**Key controls:**
- **Left / Right delay time** — set in **beat divisions** (when Sync is on) or **milliseconds** (Sync off).
- **Link** — tie both channels together.
- **Feedback** — number of repeats (see principles).
- **Filter** — a band-pass in the feedback path so repeats get darker/thinner as they trail (keeps delays from cluttering the mix).
- **Modulation** (Rate/Amount) — subtle pitch/time wobble for analog-ish movement.
- **Ping Pong** — bounce repeats L↔R.
- **Freeze** — hold the current buffer and loop it.
- **Dry/Wet**.

**In your track:** Delay appears across many tracks (bass, synth pluck with L3/R6 re-pitch dry/wet 17% fb 30%, pad, lead, vocals). *Listen for:* short offsets between L and R widen/thicken; higher feedback leaves a rhythmic trail — bypass and the sound gets drier, narrower, more "point-source."

**Sources:** [manual](https://www.ableton.com/en/manual/live-audio-effect-reference/) · [Delay video](https://www.youtube.com/watch?v=Ss5yOq8nQK4)

---

## Echo
**What it is:** A **modulation delay** with two independent delay lines *plus* envelope/filter modulation and vintage "character" — the characterful cousin of Delay.

**Key sections:**
- **Channel Mode** — Stereo, Ping Pong, or Mid/Side (in M/S the Left/Right knobs become Mid/Side).
- **Left / Right time** — beat divisions or ms (**Sync** switch). **Sync Modes:** Notes, Triplet, Dotted, 16th.
- **Stereo Link** — apply changes to both sides at once.
- **Delay Offset** — shorten/extend by fractions for a **swing** feel.
- **Feedback** — repeats.
- **Filter / Modulation** — shape and move the repeats.
- **Character tab** — **Gate** (mute repeats below a threshold), **Ducking** (reduce the wet while there's input, so echoes fill the gaps), **Noise** (vintage hiss, with Morph), **Wobble** (irregular tape-style time modulation), plus a built-in **Reverb** amount.

**In your track:** you used Echo on the **lead vocals** — double sync (L 1/8, R 1/4), dry/wet 30%, decay 50%, stereo. *Listen for:* the two different note values create a bouncing L/R rhythmic tail; Ducking keeps it out of the way while you're singing and lets it bloom in the gaps — bypass and the vocal loses its space/movement.

**Sources:** [manual](https://www.ableton.com/en/manual/live-audio-effect-reference/) · [Echo Character](https://www.youtube.com/watch?v=WJ16d_FpvEg) · [Echo Modulation](https://www.youtube.com/watch?v=inMwdangbA0)

---

## Reverb
**What it is:** Simulates a space — the wash of reflections that follows a sound. Signal flow: **early reflections** → **diffused tail**.

**Key controls:**
- **Predelay** (ms) — gap before the first reflection; conveys room size (natural: ~1–25 ms). Larger predelay keeps the dry source clear before the wash arrives.
- **Size** — room volume: large = shifting, diffuse; small = colored, metallic.
- **Decay** — time for the tail to fall −60 dB (how long the reverb rings).
- **Smooth** — how Size changes are handled (None/Slow/Fast) to avoid artifacts.
- **Freeze** — sustain the reverb almost endlessly.
- **Early Reflections: Spin** (modulation Amount/Rate — less-colored tail) and **Shape** (how sharply early reflections give way to the tail; affects intelligibility).
- **Diffusion Network: high & low shelving filters** — frequency-dependent decay (high shelf models air/material absorption; low shelf thins the decay). **Diffusion / Scale** set the tail's density/coarseness. Filters can be switched off to save CPU.
- **In/Out filters + Dry/Wet** — high-cut/low-cut on the input tames what feeds the reverb.

**In your track:** several reverbs — e.g., the **main pad** used a low+high-cut reverb, then a high-cut reverb; and reverbs sit on lead, vocals, FX, ambience. *Listen for:* the **filters on the reverb** are why you stack two — the first carves the wash (no boomy lows, no fizzy highs), the second sets the final tail tone. Bypass and the sound snaps forward, dry and roomless.

**Sources:** [manual](https://www.ableton.com/en/manual/live-audio-effect-reference/) · [Hybrid Reverb video](https://www.youtube.com/watch?v=yLBIOiM97Vs)
