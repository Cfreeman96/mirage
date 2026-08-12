# Principles — the primitives that recur everywhere

These concepts show up on device after device. Learn each once and every device gets easier to read. Device notes point back here.

## Device categories — the mental model
A sound has five properties you can shape, and each category of device targets one of them. This is *why* the knowledge base is grouped the way it is:

| Category | Shapes… | Does it add new frequencies? | Examples |
|---|---|---|---|
| **Dynamics** | **Loudness** over time (how loud, moment to moment) | No | Compressor, Glue, Multiband/OTT, Drum Buss, Limiter, Gate |
| **EQ & Filter** | **Tone / balance** (which frequencies are louder, quieter, or removed) | No — only turns existing frequencies up/down | EQ Eight, Auto Filter, Channel EQ, Utility |
| **Distortion & Character** | **Harmonic richness** (dirt, warmth, grit) by reshaping the waveform | **Yes** — creates frequencies that weren't there | Roar, Overdrive, Saturator, Vocoder |
| **Time-based** | **Space & repeats** (echoes, rooms, ambience) | No — copies the signal in time | Delay, Echo, Reverb |
| **Modulation & Movement** | **Motion** (an LFO/envelope moves a parameter over time) | No — moves pan, volume, pitch, filter, phase | Auto Pan-Tremolo, Chorus-Ensemble, Phaser-Flanger, Shifter, Shaper |
| **Instruments & Racks** | **The source itself** (generate sound, or bundle devices) | Generates the sound | Wavetable, Sampler, Drum Rack, Racks |

**The one-line test to place any device:** ask *"is it changing loudness, tone, harmonic content, space, or motion?"*
- Louder/quieter transients → **Dynamics**
- Brighter/darker, thinner/fuller → **EQ & Filter**
- Dirtier/warmer/crunchier → **Distortion**
- Echoey/roomy → **Time-based**
- Moving/sweeping/wobbling → **Modulation**

**Where the lines blur (and how to decide):** some devices do two jobs. Auto Filter is a filter *with* Drive (distortion) and an LFO (modulation) — filed under EQ/Filter because filtering is its *primary* job. Saturator can act as gentle "glue" but its core job is adding harmonics, so it's Distortion. Drum Buss is a genuine multi-tool (comp + distortion + transient + low-end) — filed under Dynamics because that's how you reach for it. **Rule: file by primary purpose, cross-reference the rest.**

## Dry/Wet
The balance between the untouched ("dry") signal and the processed ("wet") one. 0% = effect bypassed; 100% = only the processed sound. On an insert, you usually blend; on a **return track**, set it to 100% (the dry already exists on the source track). It's the single most reused knob — on Reverb, Delay, Echo, Roar, Overdrive, Shifter, compressors (as parallel blend), and more.

## Threshold
The level where a processor starts acting. Above the threshold, a compressor turns the signal down; a gate opens; a ducker begins reducing. Lower threshold = more of the signal gets affected.

## Ratio
How *hard* a compressor turns down what's over the threshold. 2:1 is gentle (4 dB over becomes 2 dB over); 10:1 is firm; ∞:1 is limiting. Higher ratio = more squash.

## Attack & Release
**Attack** = how fast the processor clamps once the signal crosses the threshold. Fast attack catches transients (tames the snap); slow attack lets the transient through, then compresses the body (keeps punch). **Release** = how fast it lets go afterward. Too fast can "pump/breathe"; too slow can stay clamped and dull. Release timed to the tempo feels musical.

## Knee
How abruptly compression kicks in around the threshold. A **soft knee** eases in gradually (transparent); a **hard knee** grabs suddenly (aggressive). Live's Compressor lets you set it; the Glue Compressor doesn't — its knee just sharpens as the ratio rises.

## Makeup gain
Compression lowers overall level, so **Makeup** adds gain back to match the original loudness — this is what lets you fairly A/B "compressed vs not" instead of just "quieter vs louder."

## Sidechain
Make a processor react to a *different* signal than the one it's processing. Classic: a compressor on the bass, triggered by the kick, so every kick ducks the bass ("pumping"). Live's Compressor, Glue Compressor, Auto Filter (envelope follower), and Roar all offer sidechain inputs. There's usually a **headphones/listen** button to hear what's triggering it.

## Cutoff & resonance (filters)
**Cutoff** = the frequency where a filter starts removing sound. **Resonance** = a boost right at the cutoff that adds emphasis/whistle. Sweeping cutoff is the classic build/tension move.

## Filter types
- **Low-pass (LPF):** keeps lows, removes highs (darkens). "LPF" = low-pass filter.
- **High-pass (HPF):** keeps highs, removes lows (thins/cleans rumble).
- **Band-pass:** keeps a band, removes above and below.
- **Notch:** removes a narrow band.

## LFO (Low-Frequency Oscillator)
A slow, inaudible wave that *moves a control for you* over time — cutoff, volume, pan, pitch. It's the engine behind auto-filter sweeps, tremolo, auto-pan, chorus, phaser. Can run free (in Hz) or **tempo-synced** to note divisions.

## Q / bandwidth (EQ)
How wide or narrow an EQ band is. High Q = surgical (notch out one resonance); low Q = broad (gentle tonal shaping). Charlie's "really high Q around 10 kHz" = a narrow, precise move.

## Mid/Side (M/S)
A way of viewing stereo: **Mid** = what left and right share (the center — kick, bass, snare, lead vocal); **Side** = what differs (width — reverb, wide synths, room). Lets you EQ/compress/narrow "the center" and "the width" independently. Found in EQ Eight (M/S mode), Utility (Width / Mid-Side), Roar (Mid Side routing).

## Stereo width & mono
**Mono** = one signal, dead center. **Stereo** = separate L/R. Width controls how far a sound spreads. Pro default: keep lows (below ~120 Hz) mono for a solid, phase-safe low end; save width for the highs. **Exception (Guido):** match the low end to the *section's job* — in a **breakdown** / atmospheric section (often kickless, going for dreamy immersion), letting the bass go **wide** is a feature, not a bug. Mono for power (drops); wide for feeling (breakdowns).

## Sync divisions
When a time-based effect (Delay, Echo, Auto Pan, LFO) is **synced**, its timing locks to the tempo in note values: 1/4, 1/8, 1/16, plus **Dotted** (1.5×, a longer swung feel) and **Triplet** (3-in-the-space-of-2, a rolling feel). Unsynced = free milliseconds.

## Feedback
How much of an effect's output is fed back into its own input. On a delay/echo, more feedback = more repeats (toward infinite). On chorus/flanger/phaser, feedback intensifies the resonant character. High feedback can self-oscillate.

## Parallel processing
Blend a heavily-processed copy *under* the dry original instead of replacing it. **Parallel compression:** dry keeps the transients/punch, the crushed copy adds body/sustain — power without killing dynamics. Achieved via a return track, a rack chain, or a device's own Dry/Wet.

## Gain staging
Keeping levels sensible at each step so nothing clips and every processor "sees" a healthy signal. EQ curves that sit entirely below 0 dB (cuts, not boosts) are good gain-staging hygiene — carve first, add makeup only where needed.

## Harmonics (overtones)
Every musical note secretly contains a stack of quieter tones *above* its main pitch (the **fundamental**) — these **harmonics/overtones** are what make a violin and a synth sound different on the same note. **Distortion and saturation** devices (Overdrive, Saturator, Roar, Drum Buss) work by *manufacturing more of these upper tones* that weren't there before. A clean sine wave is a single voice; adding harmonics turns it into a choir singing the same note with extra edge and sparkle up top — brighter, richer, grittier, and more able to **cut through a busy mix**. This is the "why" behind using Overdrive on a lead: it adds mid-high harmonics so the lead feels present and exciting without simply being louder.
