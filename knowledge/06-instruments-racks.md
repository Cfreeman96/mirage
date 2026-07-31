# Instruments & Racks — Wavetable, Sampler, Drum Rack, PML Custom Racks

_Source: Ableton Live 12 manual. Synced 2026-07-23. See `principles.md` for Cutoff/Resonance, LFO, Attack/Release, Parallel processing._

---

## Wavetable
**What it is:** Your main synth in this course (bass, plucks, risers). Two wavetable oscillators + two analog-modeled filters + a deep, approachable modulation system.

**Three sections to learn:**
- **Oscillators** — each osc plays through a **wavetable** (a set of waveforms). The **Position** sweeps through that table, morphing timbre (drag/modulate Position for movement). Pick different wavetable categories for different characters. Each osc has its own tab.
- **Sub oscillator** — adds weight below the mains. **Tone** at 0% = pure sine (clean sub); turn up for more harmonics. **Octave** switches drop it 1–2 octaves. Great for bass foundation.
- **Filters (×2)** — shape brightness (LP/HP/BP etc.) with Cutoff/Resonance/Drive; can be routed in series or parallel.
- **Modulation** — envelopes, two LFOs, and a **modulation matrix** to route anything (e.g., an envelope to filter cutoff, an LFO to osc Position). This is where a static patch becomes alive.
- **Unison** — stack detuned voices for width/thickness.

**In your track:** the **bass, art pluck, lead, and risers** are all Wavetable. *Listen for:* modulating **Position** morphs the tone over time; the **sub osc** is what makes the bass feel physically low — mute it and the bass thins out.

**Sources:** [manual (instruments)](https://www.ableton.com/en/manual/live-instrument-reference/) · [Wavetable Overview](https://www.youtube.com/watch?v=9wovKSfR66A)

---

## Sampler (and Simpler)
**What it is:** Plays back audio samples as a playable instrument. **Simpler** is the streamlined one (one sample, quick ADSR); **Sampler** is the full version (multisamples mapped across zones).

**Key controls:**
- **ADSR envelopes** (Attack/Decay/Sustain/Release) — shape amplitude, and can also modulate filter cutoff and pitch. Attack = time to peak; Decay = fall to Sustain; Sustain = held level; Release = tail after note-off.
- **Filter** — cutoff/resonance with its own envelope amount.
- **Zones (Sampler)** — map many samples across **Key**, **Velocity**, and **Sample-Select** ranges (as "layers") to build realistic multisampled instruments.
- **Warp/loop** — time-stretch and loop behavior.

**In your track:** you used a **Sampler on the vocals** and noted you "didn't touch ADSR at all." *Listen for:* that means the vocal plays with its natural envelope — if you *did* shorten Release, tails would cut off faster; lengthen Attack and each note would fade in. Good next experiment.

**Sources:** [manual (instruments)](https://www.ableton.com/en/manual/live-instrument-reference/) · [Drum Sampler video](https://www.youtube.com/watch?v=rKGkthvnDSA)

---

## Drum Rack
**What it is:** A container that hosts a full kit — each pad is its own chain (a Simpler/Sampler/instrument + its own effects), laid out on a 4×4 grid.

**Key features:**
- **Pads / chains** — each pad = one drum voice with independent devices and mixer.
- **Receive / Play notes** — the incoming MIDI note a pad responds to, and the note it sends on.
- **Choke groups** (16) — chains in the same group silence each other; classic use: an open hat choked by a closed hat.
- **Return chains** — built-in sends/returns *inside* the rack, fed by each pad's send sliders, so you can share one reverb/delay across the kit (route to rack output or the Set's returns).

**In your track:** you built kits in Drum Racks — the **replacement kick**, and the **snare** (a 4-instrument percussion rack duplicated and soloed to the snare). *Listen for:* choke groups keep hats tight; per-pad effects let you process one drum without touching the others.

**Sources:** [manual (Drum Racks)](https://www.ableton.com/en/manual/instrument-drum-and-effect-racks/) · [Drum Rack routing](https://www.youtube.com/watch?v=Y_tUyHebxko)

---

## Audio Effect Rack — parallel chains
**What it is:** A container that wraps one or more device **chains** and behaves like a single device in your track. Its power for effects is **parallel chains**: every chain receives the **same input at once**, processes it serially through its own devices, and all chain outputs are **mixed together** to form the Rack's output. Each chain has its own **volume/pan**, plus Solo and Chain-Activator buttons, so you can balance the pathways independently.

**Signal flow:** normally devices are serial (left→right, each feeds the next). A Rack lets you branch into parallel paths instead — great for blending a processed version alongside the dry, without a single dry/wet compromise.

**How to build a parallel path (e.g. dry lead + separate delay):**
1. Select the lead's devices → **Group** (Cmd/Ctrl+G) → they become **Chain 1** in the Rack.
2. Click the **Chain List** (left view button) to reveal the chains and the **drop area** below.
3. Drag a **Delay** into the drop area to start **Chain 2** (gets the same raw input, fully separate signal).
4. Shape Chain 2 independently — e.g. **Ping Pong** + low-pass ~515 Hz so only the low end echoes, dark and distinct from the dry lead.
5. Balance with each chain's **volume slider**; **Solo** a chain to hear it alone. Optionally map a chain's volume to a **Macro**.

**In your track:** this is the rack Charlie built on the **lead** — Chain 1 = the lead's sound design (as-is), Chain 2 = a ping-pong delay filtered to ~515 Hz. Two pathways, tuned separately, mixed at the output. *Listen for:* the delayed low-end shadow trailing under the bright dry lead; pull Chain 2's volume down and the shadow recedes without changing the lead itself.

**Sources:** [manual (Instrument/Drum/Effect Racks)](https://www.ableton.com/en/manual/instrument-drum-and-effect-racks/) · [Parallel effect chains](https://www.youtube.com/watch?v=PGxvwjX0dU0)

---

## PML custom racks (from the course files)
These aren't stock Ableton devices — they're **Racks** the PML instructors built (a Rack bundles devices + Macro knobs into one panel). Two you flagged:

- **"Drum Full Parallel"** (on your clap) — a **parallel compression** rack: internally it splits to a heavily-compressed copy blended under the dry, so the clap keeps its snap while gaining body. See *Parallel processing* in `principles.md`. This is the same concept Guido is teaching in 4.x.
- **"2×2 Tile" custom editor** (on the brake piano) — a PML Rack with **Macro controls** wired to several underlying device parameters at once, so one knob move does a musical, multi-parameter change. The "custom editor" look is just the Rack's Macro panel.

**How to inspect any rack:** click the **unfold/chain-list** triangle on the Rack's title bar to see the actual devices inside, and right-click a **Macro** to see what parameter(s) it controls. That's how you demystify any preset rack.

**Sources:** [manual (Instrument/Drum/Effect Racks)](https://www.ableton.com/en/manual/instrument-drum-and-effect-racks/)
