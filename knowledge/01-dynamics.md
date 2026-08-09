# Dynamics — Compressor, Glue Compressor, Multiband Dynamics (OTT), Drum Buss, Limiter

_Source: Ableton Live 12 manual. Synced 2026-07-23. See `principles.md` for Threshold, Ratio, Attack/Release, Knee, Makeup, Sidechain, Parallel processing._

---

## Compressor
**What it is:** Live's original, versatile compressor — the surgical, transparent one for controlling a *single* element.

**Key controls:**
- **Threshold / Ratio / Attack / Release** — the core four (see principles).
- **Knee** — soft (gradual, transparent) to hard (sudden, aggressive). This adjustability is a key difference from the Glue.
- **Detection modes** — Peak (reacts to fast transients) vs RMS (reacts to perceived loudness, smoother).
- **Sidechain section** (unfold the device) — trigger from another track, with its own EQ so you can trigger off a specific frequency. A **headphones** button lets you audition the trigger.
- **Dry/Wet** — blend for parallel compression.
- **Makeup** — level match after compressing (can be Auto).

**Common uses:** tame a vocal, tighten a bass, control a snare, or kick-triggered sidechain ducking.

**In your track:** you have Compressors on the bass, synth pluck, main pad (with sidechain), vocals, and several FX. Several were later **bypassed** in Guido's Part 2 — that's normal; Part 2 rebuilds the dynamics more deliberately. *Listen for:* with the right attack, hits stay punchy but the overall level steadies — turn it off and the track feels more uneven/jumpy in volume.

**Sources:** [manual](https://www.ableton.com/en/manual/live-audio-effect-reference/) · [Sidechaining video](https://www.youtube.com/watch?v=rbuTKgcteKo)

---

## Glue Compressor
**What it is:** An analog-modeled bus compressor (built with Cytomic, based on a classic 80s SSL console compressor). Designed to sit on a **Group or Main** track and fuse multiple sources into one cohesive, slightly-colored whole.

**Key controls:**
- **Threshold / Ratio / Attack (ms) / Release (sec, or Auto)** — note Release is in seconds here.
- **No adjustable knee** — the knee sharpens automatically as Ratio increases.
- **Range** — limits how much compression can occur (−60 to −70 dB emulates the original hardware; −40 to −15 useful as an alt to Dry/Wet).
- **Makeup** — match the needle position for level-matched gain.
- **Dry/Wet** — built-in parallel compression.
- **Soft Clip** — tames loud transients (caps output ~−0.5 dB, but distorts — not a transparent limiter).
- **Oversampling** (title-bar menu) — cleaner, less aliasing, slightly more CPU.
- **Sidechain** — same idea as the Compressor.

**Rule of thumb:** Compressor = control one thing; Glue = make many things feel like one thing.

**In your track:** you put a Glue Compressor on your **drum group** (textbook use) and another on the bass with a sidechain filter. *Listen for:* on the drum group, bypass it and the kit sounds like separate pieces; enable it and the drums "breathe together" as one punchy unit — subtle but it's the glue.

**Sources:** [manual](https://www.ableton.com/en/manual/live-audio-effect-reference/) · [Glue Compressor video](https://www.youtube.com/watch?v=7xEZa1IlW5Q)

---

## Multiband Dynamics (a.k.a. where OTT lives)
**What it is:** A flexible, mastering-grade dynamics processor. It splits sound into up to **three bands** (adjustable crossovers) and can do **both compression and expansion, upward and downward**, per band. **OTT** is just an aggressive preset of this device.

**Concept — four ways to move dynamics:**
- **Downward compression** — turn loud signals *down* (the usual kind).
- **Upward compression** — turn quiet signals *up* (less common; makes things "bigger/denser").
- **Downward expansion** — turn quiet signals further down (like a gate).
- **Upward expansion** — turn loud signals up.
Each band has an **upper** threshold (downward comp) and a **lower** threshold (upward comp), so two things happen per band at once.

**Why OTT sounds so "modern":** it applies heavy upward + downward compression across all three bands — quiet detail gets lifted, loud peaks pulled down, per band — so synths sound instantly bigger, brighter, and more in-your-face. Easy to overdo.

**In your track:** you ran OTT on the **bass** and **synth pluck** (later bypassed on bass in Part 2). *Listen for:* at 100% it flattens and brightens aggressively (that EDM sheen); pulling the Amount to ~25–35% keeps polish without the pumping/lifeless flatten.

**Sources:** [manual](https://www.ableton.com/en/manual/live-audio-effect-reference/)

---

## Drum Buss
**What it is:** An analog-style, one-stop drum processor — compression, distortion, transient shaping, and low-end enhancement in a single device, made to add body/character and glue a kit.

**Key controls:**
- **Trim** — reduce input level before processing.
- **Comp** (toggle) — a fixed compressor (fast attack, medium release, moderate ratio, ample makeup) optimized for gluing drums.
- **Drive** — pushes the signal harder into the distortion.
- **Distortion type** — *Soft* (waveshaping), *Medium* (limiting), *Hard* (clipping + bass boost).
- **Transients** — emphasizes/de-emphasizes attack above 100 Hz. Positive = punchy, fuller; negative = tighter, crisper, less room/rattle.
- **Crunch** — sine-shaped distortion on the mid-highs (clarity/presence on snares, hats).
- **Damp** — low-pass that removes harsh highs created by the distortion.
- **Boom** — a tuned resonant low-end boost (with Freq and Amount) to fatten the kick.

**In your track:** you ran a **Drum Buss on Kick 1** — which is why that one device seems to "do a lot" (it's comp + distortion + transient + low-end at once). *Listen for:* nudging **Transients** up adds attack/click; **Boom** adds sub-weight; the **Comp** toggle glues — A/B each control solo to hear its single job.

**Sources:** [manual](https://www.ableton.com/en/manual/live-audio-effect-reference/) · [Drum Buss video](https://www.youtube.com/watch?v=_okKGKp5a9I)

---

## Limiter
**What it is:** A transparent **brickwall limiter** — effectively a compressor with an infinite ratio and very fast response. Its job: stop the signal from ever exceeding a set **ceiling**, and (on the master) raise loudness safely. Overhauled in Live 12.1 with smoother release and better metering. This is a **mastering** device — typically the *very last* thing in your Main chain.

**Key controls:**
- **Input Gain** — drives the signal into the limiter (more input = more limiting/loudness).
- **Ceiling** — the maximum output level the signal can reach (e.g. −0.3 dB). Nothing gets past it.
- **Maximize** (toggle) — turns Ceiling into a single **Threshold** loudness control; Input Gain becomes **Output** (target level). One-knob loudness.
- **Release** — how fast limiting lets go. Fast = louder/punchier; slow = smoother but can dull dynamics. **Auto** adapts release to the material.
- **Lookahead** — lets it "see" peaks slightly early to catch them cleanly (adds latency).
- **Ceiling modes** — **Standard** (default), **Soft Clip** (gentle clipping near the ceiling for color/punch on transients — an LED flags clipping), **True Peak** (prevents inter-sample peaks — safest for streaming/export).
- **Routing** — Stereo, **L/R** (more limiting, slight image shift), or **M/S** (limit center vs. width independently, preserves image). **Gain Reduction Link** blends how much the channels share reduction.
- **Gain Reduction meter** — watch how hard it's working.

**In your track:** Guido introduced this in the **mastering** stage — it belongs at the end of your **Main** track, after your mastering EQ/comp. *Listen for:* as you push Input Gain (or lower Threshold in Maximize), the whole track gets louder but peaks never cross the ceiling; push too far and it goes flat/pumpy and transients (the kick's snap) disappear. Use True Peak for the final export.

**Sources:** [manual](https://www.ableton.com/en/manual/live-audio-effect-reference/) · [Limiter video](https://www.youtube.com/watch?v=Gvbf90IffRo)

---

## Split Band Compressor (DIY multiband / de-esser)
**What it is:** A homemade **multiband compressor** built from native devices (Guido's rack). An **Audio Effect Rack** with **three parallel chains**, each starting with an **EQ Three** that solos one band (chain 1 = Low only, chain 2 = Mid only, chain 3 = High only, via the L/M/H kill buttons). Parallel chains sum back to the full signal, so with no processing it's transparent. Then process one band alone — e.g. a **Compressor only on the High chain** = compress just the highs.

**Settings shown:** crossovers **FreqLow 250 Hz / FreqHi 2.5 kHz**, **48 dB** slope (tight separation). High-chain Compressor with **SC Filter ~7.74 kHz** → clamps only when sibilance spikes = a **dynamic de-esser**.

**Why:** full independent control per band (a whole Compressor, with sidechain filter, on each band) — the transparent, hands-on alternative to OTT/Multiband Dynamics. Put the compressor on the High band to de-ess/tame harsh highs, or the Low band to tighten boomy bass.

**Tradeoff:** splitting and recombining bands can cause slight **phase interaction at the crossovers** — fine for most work, but the reason dedicated multiband/compander tools (with optimized crossovers) exist.

**Ties to:** Audio Effect Rack (parallel chains), EQ Three (kill bands), Compressor (sidechain filter), Multiband Dynamics/OTT.

**Sources:** [manual — EQ Three & Compressor](https://www.ableton.com/en/manual/live-audio-effect-reference/)

---

## Vocal leveling compressor (recipe)
**Goal:** shrink a vocal's **dynamic range** (gap between loud & quiet) so it sits consistently, without sounding squashed. This is the *how-to-dial-it* recipe — distinct from the Compressor *device* note above.

**Guido's vocal settings:**
- **Threshold ~−23 dB (low)** — reach into the whole performance, not just peaks → leveling, not just peak-catching.
- **Ratio ~12:1 (high, near-limiting)** — firm control of the loud parts.
- **Knee ~18 dB (wide/soft)** — eases that hard ratio in gradually; only the biggest peaks feel the full 12:1.
- **Attack ~120 ms (slow)** — lets consonants/transients through → stays crisp.
- **Release ~30 ms (quick)** — recovers between words → natural.
- **Peak** detection — catches the actual instantaneous peaks.
- **Makeup ~+5 dB** — lifts it all back up so quiet detail rises to meet the tamed peaks.
- **SC Filter ~80 Hz** — so low-end thumps/plosives don't trigger it.

**What it does:** loud comes down (compression) + everything comes up (makeup) → dynamic range collapses into something even and forward, but peaks still poke through so it stays authentic, not jumpy. The **high-ratio + wide-knee** pairing is the key: strong control that only fully bites on the loudest moments.

**Sources:** [manual — Compressor](https://www.ableton.com/en/manual/live-audio-effect-reference/)
