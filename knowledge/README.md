# Mirage — Ableton Knowledge Base

A distilled, personalized cache of the Ableton Live 12 manual, covering every device Charlie has used in the PML327 course track. Built once from the official manual (via the Ableton Knowledge connector); read from here for routine work, re-synced from the connector when a detail is missing or when Ableton ships a manual update.

## How this is used
- **Source of truth:** the Ableton Live 12 manual (connector). **Fast read cache:** these files.
- Each device note is **distilled** (not copy-pasted): what it is, what each key control does, common uses, plus an **"In your track"** section tying it to Charlie's actual signal chains and — importantly — *what it audibly changes so he can listen for it*.
- The card-bank HTML app pulls its lesson content from these notes.

## Files
- `principles.md` — the cross-cutting primitives (Dry/Wet, Threshold, Ratio, Attack/Release, etc.) that recur across many devices. Learn once, reuse everywhere.
- `01-dynamics.md` — Compressor, Glue Compressor, Multiband Dynamics (OTT), Drum Buss, Limiter
- `02-eq-filter.md` — EQ Eight, Auto Filter, Utility
- `03-distortion-character.md` — Roar, Overdrive, Vocoder, Saturator
- `04-time-based.md` — Delay, Echo, Reverb
- `05-modulation.md` — Auto Pan-Tremolo, Chorus-Ensemble, Phaser-Flanger, Shifter, Shaper
- `06-instruments-racks.md` — Wavetable, Sampler, Drum Rack, PML custom racks

> Grouped by category for efficiency and easy reading; can be split into one-file-per-device anytime.

## Sync log
- **2026-07-23** — Initial build. All notes grounded in Live 12 manual / release notes. Note: Live 12.3 renamed *Auto Pan* → *Auto Pan-Tremolo*.
- **2026-07-23** — Added **Limiter** (→ 01-dynamics) and **Saturator** (→ 03-distortion-character) after Guido's walkthrough. Now 24 devices + 17 principles.
- **2026-07-23** — Added `principles.md` **Device categories** explainer, and built **`mirage-cards.html`** — the complete reveal-first card app (43 cards: 1 Foundations + 17 principles + 25 device cards, Roar split into routing + shaper). Self-contained, mobile-first, deploy-ready (e.g. Vercel).
- **2026-07-23** — Added **Harmonics** (principle) and **Audio Effect Rack / parallel chains** cards → app now **45 cards**. Added matching notes to `principles.md` (Harmonics) and `06-instruments-racks.md` (Audio Effect Rack — parallel chains).
- **2026-07-23** — Added 4 cards — **Chain vs track volume**, **Dotted eighth note**, **Glue Compressor — Attack & Release**, **Chorus-Ensemble — modes** — and enriched the **Dry/Wet** card (partial = parallel blend). App now **49 cards**.
- **2026-07-23** — Added **Spectral Time** (freeze + spectral delay) → card app now **50 cards**; matching note added to `04-time-based.md`.
- **2026-07-23** — Added 2 cards for Guido's **Bootsandcats** rack (the Shaper sidechain, + a "why two Utilities" card) → app now **52 cards**; matching note added to `05-modulation.md` under Shaper.
- **2026-07-23** — Added a dedicated **Bass Mono** card (why mono the lows) → app now **53 cards**.

## Personalization source
Charlie's signal chains and course position live in `../../../Music Learning/Producer-Profile.md` (Producer Profile). Update that when his project changes, and these "In your track" notes with it.
