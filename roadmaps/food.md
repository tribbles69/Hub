# Food — roadmap

**Status:** next up · **Replaces:** Cronometer, MyFitnessPal · **Working name** (rename before the repo is made)

A food diary that does what Cronometer and MyFitnessPal do for you, minus the upsells, with your
history in your hands. Starting material is already in `Ironlog/r&d/food-handover`: the CoFID
and curated food tables, the Haiku parser, and the `ironlog-food-log` v1 export format.

## Phase 1 — a diary you can switch to
- [ ] Repo, Pages, PWA shell per `STANDARDS.md`
- [ ] Import Ironlog's food export (`format: 'ironlog-food-log'`, `formatVersion: 1`) so no history is lost
- [ ] Diary by day and meal; add, edit, delete entries
- [ ] Food search over the local CoFID + curated tables (from the handover), local first
- [ ] Custom foods and saved favourites
- [ ] Daily targets with bars for kcal, protein, carbs, fat — the Cronometer screen you use
- [ ] Water tracker with a daily goal
- [ ] Copy yesterday, copy a meal (MyFitnessPal)
- [ ] Export / import in the shared backup envelope, plus CSV

## Phase 2 — fast logging
- [ ] Barcode scan with the camera (Chrome's barcode detector) → Open Food Facts lookup, cached locally
- [ ] Recipe builder: ingredients in, per-portion macros out (MyFitnessPal)
- [ ] Quick-add for a pub or takeaway meal by estimate
- [ ] Body weight on the same diary page

## Phase 3 — extras
- [ ] AI text parsing as a fallback only, on your own key (the Haiku parser contract from the handover)
- [ ] Micronutrient totals from CoFID (Cronometer)
- [ ] Read the Sinocare Bluetooth scales directly, if their protocol can be worked out
- [ ] Publish a documented read-only data shape so the Stamina Meter can use the diary

## Done when
Cronometer and MyFitnessPal can be deleted without missing anything you actually use.
