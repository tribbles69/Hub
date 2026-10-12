# Stamina Meter — roadmap

**Status:** idea · standalone app, not part of Ironlog

A game-style view of where your energy is. Food fills a **stamina bar** — fast carbs fill it
quickly and drain fast, slow carbs fill it slowly and last. An **HP bar** tracks the slower
fatigue (muscle and mental) that a day's food can't fix.

## Phase 1 — the bars
- [ ] Decide the model: how fast and slow carbs fill and drain stamina; what lowers and restores HP
- [ ] Read meals from the Food app's stored diary (same origin, read-only — see `STANDARDS.md`),
      with a manual quick-add until Food exists
- [ ] Stamina and HP bars that update through the day
- [ ] Repo, Pages, PWA shell

## Phase 2 — more inputs for HP
- [ ] Sleep and drive from Kraftur
- [ ] Training load from Ironlog (same origin, read-only)
- [ ] Steps from the watch, entered by hand until there's a way to read them

## Phase 3 — make it a game
- [ ] XP and quests from cardio minutes (Cardio Quest)
- [ ] Steps as currency (Stepcraft)
- [ ] Climbing numbers and unlocks, the hook from idle games

## Open question
- Cronometer can't be read directly; the Food app is the route to real data.
