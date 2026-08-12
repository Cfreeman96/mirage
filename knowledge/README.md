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
- **2026-07-23** — Added **RX 9 Voice De-click vs De-noise** card in a new **Cleanup** category (note: iZotope RX is third-party, not in the Ableton manual cache) → app now **54 cards**.
- **2026-07-23** — Added **De-essing** card (Cleanup) — sibilance, the static EQ Eight high-Q cut vs the dynamic Compressor-sidechain method → app now **55 cards**.
- **2026-07-23** — Added **EQ Three** card (EQ & Filter) — DJ-style 3-band kill EQ vs surgical EQ Eight → app now **56 cards**; matching note added to `02-eq-filter.md`.
- **2026-07-23** — Added **Split Band Compressor (DIY multiband/de-esser)** card (Dynamics) → app now **57 cards**; matching note in `01-dynamics.md`. NOTE: "Compandr" tool Guido praised could not be verified via web search — awaiting maker/spelling from Charlie before carding the compander comparison.
- **2026-07-23** — Added **Vocal leveling compressor (recipe)** card (Dynamics) — the settings recipe + dynamic-range reasoning; intentionally distinct from the device-choice "Compressor" card → app now **58 cards**; matching note in `01-dynamics.md`.
- **2026-07-23** — Audit pass: renamed card category **"Instruments" → "Instruments & Racks"** (so the Audio Effect Rack / PML racks cards fit honestly), and added a **dark-mode toggle** (top-right, choice remembered via localStorage). Optional cross-refs between related-card families held pending Charlie's go-ahead. Also added a 🏝️ inline-SVG favicon.
- **2026-07-23** — Added **Delay filter (the orange dot)** and **Echo vs Delay** cards (Time-based) → app now **60 cards**. (Envelope card offered — Charlie flagged the term as a recurring hang-up.)
- **2026-07-23** — Evolved the app from a flashcard deck into a **3-tab hub** (still one self-contained HTML): **Quiz** (the reveal-first deck, unchanged), **Browse** (searchable, category-grouped, expandable library of all cards), and **Journey** (home: artist ID, current course position, goals, library stats — sourced from Producer-Profile). Quiz kept central; active recall preserved.
- **2026-07-23** — **Pilot Mirage website**: added a brand wordmark + nav; renamed Journey→**Home** and made it the branded landing (hero + live practice snapshot). Added the **Gym** tab — a practice tracker with drill cards (Basslines, Synths, Drums, Chords, Echo, Mixing, Loops · target 25 each), tap-to-log reps, day-streak / this-week / total stats, a 7-day activity strip, and a **Back up my data** export. Persists via `localStorage` (works on the live Vercel site; NOT in the Claude preview; clearing browser data resets it — hence the export). Title→"Mirage 🏝️".
- **2026-07-23** — Gym upgrades: **per-rep notes + Recent-activity log** (each rep can carry a one-line note; scrollable history), and **repeatable drills + weekly goal** (drills complete-and-restart, showing "×N done" cycles; editable weekly rep goal with its own progress bar). Runtime-tested. Not built (Charlie declined for now): scheduled reminder, random prompts, editable drills/import.
- **2026-07-23** — Gym **Insights**: a GitHub-style **year activity heatmap** plus a **Daily / Weekly / Monthly / Year** view switcher (bar charts for the first three, heatmap for Year), and a **reps-by-weekday** panel to spot free days. Pure CSS/HTML — no libraries, stays offline-capable. Chosen view remembered in localStorage. Aggregation logic runtime-tested. Storage still localStorage — cloud/durable storage remains the future inflection point (esp. for cross-device + track-cover images).
- **2026-07-23** — Renamed the **Gym tab → Reps**; added a new **Lab** tab (Effect Lab). Assigns an effect (🎲 random from a 21-device list, or pick), suggests 3 contrasting loop sources, shows key knobs + a 4-step sweep protocol, and logs the session into Reps (drill id "efflab" → "Effect Lab" in the activity log, counts toward streak/heatmap). Includes a loop-bank setup guide. Closes the Learn→Practice loop (Quiz → Browse → Lab → Reps).
- **2026-07-23** — Added **Redux** card (Distortion — lo-fi: downsampling + bit reduction) → app now **61 cards**; also added Redux to the Effect Lab device list. Matching note in `03-distortion-character.md`.
- **2026-07-23** — Added a **Shortcuts** tab: ~36 Ableton keyboard shortcuts grounded in the Live 12 manual, grouped (Transport/Tracks/Editing/Grid/Zoom), searchable, with an add-your-own "My shortcuts" section (localStorage). Mac symbols shown. Tab lineup now Home · Quiz · Browse · Reps · Lab · Tools · Shortcuts.
- **2026-07-23** — Added a **Tools** tab (third-party tools) + a durable memory file `../Suggested-Tools.md`. **STANDING RULE:** whenever Guido/anyone Charlie respects recommends an external tool, capture it (name, who, why) — don't deep-dive, just log to revisit later. In-app list: add / delete / cycle status (To try → Exploring → Using it → Passed), localStorage. Seeded with **Type A — AudioThing** (via Guido; "better OTT for thickening vocals").

## Personalization source
Charlie's signal chains and course position live in `../../../Music Learning/Producer-Profile.md` (Producer Profile). Update that when his project changes, and these "In your track" notes with it.
