# Course 1 Recap — Guido's Mixing & Mastering (PML327)

*Finished 2026-08. A reflection to internalize before starting Serum 2. Two halves: (1) the recurring moves that made it better — the transferable stuff, and (2) the element-by-element log of what we actually did to the track.*

---

## Part 1 — The ten moves Guido kept using

The course wasn't a bag of tricks; it was the **same handful of techniques applied over and over**. Learn the patterns and the whole thing compresses into ten ideas.

1. **Fix, then place.** Two EQ Eights in a row: the first *corrects* the sound in isolation (tame a resonance, clean the lows), the second *sits it into the song* (carve where it clashes with neighbors). Signature move on the kick; reused on the clap.

2. **Split things apart for control.** Don't treat a loop as one unit — break it into parts you can automate independently. The hi-hat loop became an **up-hat + a 1/16 hat** (Boots-and-cats "flip it" at 50% re-timed the 1/16 so you could fade it in at the first drop). Same instinct: the **split-band de-esser** (low/mid/high) on the chorus. Divide, then control each piece.

3. **Tighten every low element the same way.** **Boots-and-cats** (the Shaper sidechain) lives on the bass, sub, and low elements — the default move to keep the low end punchy and out of the kick's way.

4. **Build a parallel "flavor box."** The bass FX rack: a **parallel** chain of delay + glue-comp (sidechained to the bass, ultra-fast attack/release, 100% wet) + a touch of reverb — character *underneath* the dry signal, not muddying it. Parallel, not in-line.

5. **Purpose-built sends, switched on by automation.** Not one reverb for everything — **dedicated returns** (vocal throw, breath, lead delay), automated *on* for single words or moments. Effects as punctuation, not wallpaper.

6. **Subtract noise ruthlessly.** Cut the top off vocals; pull ambience out of the drops and repeats; remove EQs doing nothing. A lot of "better" was just *removing* clutter.

7. **Replace, don't rescue.** When a sound wasn't right, he swapped it outright — the **kick**, and the **Wavetable lead → Meld lead**. Extending the lead notes to **legato + overlapping** is what made the glide work.

8. **Width by section job.** Mono/centered for power in the drops; wide for feeling in the breakdown (the low bass going wide there is a *feature*).

9. **Automate for movement.** The recurring trio — **Auto Filter → Auto Filter → Utility** — is the movement/energy engine reused across elements. (Auto Filter is still the one to internalize — needs more hands-on reps.)

10. **Master = shape then cap, always metered.** OTT (gentle) → mid-side EQ8 → GM clipper → limiter, with the Swiss Army meter + Ozone imager. Decide by numbers and width, not vibes.

---

## Part 2 — Element-by-element log

### Drums (drum group)
- **Kick** — originally a character kick off the Sampler (Drum Rack + EQ8 + Vocoder + double Auto Filter/Utility automation). **We replaced the kick sound** — much better. Then **EQ8 #1 to fix it**, **EQ8 #2 to place it in the song**. Same automation reused: Auto Filter, Auto Filter, Utility.
- **Clap** — **Gate** → Vocoder → **EQ8** to fix a resonance → a little **Reverb** (short decay, ~14% dry/wet) → automation at the end + an EQ8 fade. *(→ new Gate card banked.)*
- **Hi-hats** — split the loop into an **up-hat** and a **1/16 hat** using Boots-and-cats on both. Up-hat: flip **off**. 1/16 hat: flip **all the way to 50%** (the only difference) — this re-timed it so you could **fade the 1/16 in at the first drop**.
- **Snare** — nothing crazy.
- **Extra percussion** — untouched.

### Bass (bass group)
- **Bassline** — reshaped the **envelope**; **Roar** (mostly on the low). An EQ8 doing nothing + Boots-and-cats on it.
- **The "flavor box"** — an **Audio Effect Rack** on the bass: upper parallel chain = **Delay** (unsynced, L=3, R=6, feedback 29%) + **Glue Compressor** (sidechained to the bass itself, hyper-short attack + release, 100% dry/wet) + **Reverb** (~14%). Then Auto Filter · Utility · EQ8 at the end. **Utility mid-side at 44%** for the bass.
- **Sub** — added with a Tone %; basically just Boots-and-cats on the new track. Slight low bump (hyper-narrow ~0.3 Q, ~70 gain at 40 Hz). **Two Auto Filters** here — one legacy, one new.
- **Tonal-percussion / breakdown low bass** — the Wavetable low bass taken down from the breakdown. Since it's bass and in the bass group, we made it **wider** (breakdown = don't care about mono) — likely classic unison, or it was already wide and left alone.

### Leads
- **Wavetable lead → Meld lead** — liked the Meld a lot more; the original was very wet by comparison. **Extended the MIDI notes to legato** so they filled the space, then **overlapped them slightly** to trigger **glide**.

### Harmonies / pads
- **Art Pluck** — minor fine-tuning; took some EQs off.
- **Focal Pad** — noisy; Roar + Boots-and-cats.
- **Background pads / ambience / break pad / breakdown piano** — little done with Guido.

### Vocals (the big section)
- Cut off the top end. **Ensemble + Auto Filter + Delay**, aiming to be more surgical.
- **Chorus** — built the **split-band de-esser** (low/med/high) to make it less punchy; **Roar** too. Focused on the high end of that multi-band FX.
- Removed ambience from the drops/repeats + a couple of unnecessary pieces (noise cleanup).

### FX sends / return tracks we built (turned on via automation)
- **Return 1 — the LFO delay** — a Delay modulated by an **LFO** (rate 0.16 Hz, depth 27% — very slow), Dry/Wet 100%, smoothing, repitch, drifting L/R up to 2.54 ms, feedback 50%, + Reverb (100% wet, ~13 s decay). Used on the Wavetable lead and heavily on **vocals** (send one word into reverb).
- **Return 2 — Breath** — Delay 8× synced L/R, 50% feedback, filter 1.37 kHz + 1.62 ping-pong, 100% wet, limiter −24 dB; Reverb 43% dry/wet, 14 s decay. For a longer delay tail than the vocal-sync delay.
- **Return 3 — Throw (time-based, unsynced)** — Delay 3×, freq 1.6 Hz + 2.8; Reverb 60%, decay 14.1 s; Auto Pan-Tremolo 17%, amount 0.17, freq 1.7. **Used on the clap.**
- **Return 4 — Lead One** — Simple Delay 2×2 synced, 100% wet, freq 2.5, width 2.5, ping-pong; Reverb 63%, decay 6.5. **Used on the old Wavetable lead** (not really the Meld lead).

*(→ new FX-return/throw recipe card banked, capturing these four.)*

### Mix & master
- Mixed the main track.
- **Master chain:** slight **OTT** → very slight **EQ8 in mid-side mode** → **GM Audio Clipper** (paid) → **Limiter** → **Swiss Army** metering, with an **Ozone imager** to watch stereo width.

---

## Part 3 — Guido's lesson list (for re-watch / internalize)

Mirrored in the app's **Training** tab, where each can be marked *Internalized*.

**Drums:** Reverse-engineering common kick issues · Replacing the kick · Common snare & clap issues · How to mix it · Hi-hat & shaker issues · Mixing in the hi-hat · Percussion issues
**Bass:** Bass issues · Compressing the drums *(likely where Boots-and-cats saturation was introduced)*
**Harmony & FX:** Common harmony issues · FX sends · Common leads · Mixing the leads
**Vocals (big one):** Preparing for vocals · Vocal issues · Cleaning vocals · Vocal compression · Time-based effects for vocals · Vocal throw · Vocal width · Extra background vocals · Mixing the verse
**Breakdown & arrangement:** FX · Common breakdown issues · Mixing the breakdown · Quick mix of the whole arrangement · Filtering · FX cleanup
**Mastering:** Mastering · Limiters · Clippers · EQ · Multi-band dynamics · The nerdy stuff · Feedback for low end · Lead remake with Meld one-knob automation · Final tweaks · Thank you & feedback

---

## Part 4 — Open threads
- **Auto Filter** — still the concept to internalize; earmark hands-on reps.
- **Re-watch earlier lessons** away from the desk to catch anything forgotten (that's what the Training tab is for).
- Next up: **Serum 2** (6-hour sound-design course) — its own card space in the app.
