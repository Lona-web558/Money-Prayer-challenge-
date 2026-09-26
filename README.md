# Money-Prayer-challenge-

# Money Prayer — 10 Day Challenge

A single-file habit tracker for a 10-day Money Prayer challenge. Check off each day as you complete it.

## Files
- `money-prayer-challenge.html` — the entire app (HTML5, CSS3, Bootstrap 5, vanilla JS)

## Features
- 10 daily checklist items, one per day
- Sequential unlock — Day 2 stays locked until Day 1 is checked, and so on
- Unchecking a day re-locks every day after it
- Progress bar + "days completed" counter
- Completion banner when all 10 are done
- Reset button to start the challenge over
- Progress is saved automatically in the browser via `localStorage` — no backend, no build step

## Usage
1. Open `money-prayer-challenge.html` in any browser (double-click it, or host it — Render/Netlify/Neocities all work).
2. Tap a day to mark it done.
3. Progress persists per-browser/device. Clearing browser data or switching browsers resets it (or use the Reset button to do so manually).

## Customize
- **Label text**: edit the `<b>Day ${i+1}</b> — Money Prayer` line inside the `<script>` block.
- **Colors**: CSS variables at the top of the `<style>` block (`--gold`, `--cyan`, `--bg`, etc.).
- **Challenge length**: change every `10` (day count, `Array(10)`, `doneCount*10`) to your desired number of days.
- **Storage key**: `KEY = 'moneyPrayerChallenge10'` — change this if you want a fresh independent tracker alongside other localStorage-based apps on the same domain.
