# Tally — roadmap

**Status:** next · **Replaces:** Finch, Streakletics, Click Counter

Tick boxes at the end of the day, and a scrolling year grid per category where the colour
depth shows how much of that category got done. Layout based on the bullet-journal tracker
from r/monkmode. Categories: hygiene, wellness, physical, mental, weight, and "stop" habits.

## Decisions (2026-10-21)
- Seed a starter set of habits (below); everything is editable in the app.
- Try an evening reminder notification, best-effort (see note under Phase 1).
- Kraftur stays separate from Tally for now.
- Counter habits and the levelling creature come into the first build; streak freezes wait.

## Starter set
- **Hygiene:** teeth morning, teeth night, showered
- **Wellness:** water (counter, goal 8 glasses), in bed on time, daylight outside
- **Physical:** trained or did mobility, stretched
- **Mental:** read, wrote (book or project), screen-free before bed
- **Weight:** weighed in, logged food in Cronometer
- **Stop:** no doomscrolling in bed, no takeaway, no late snacking (ticked = didn't do it)

## Phase 1 — the tracker
- [ ] Repo, Pages, PWA shell per `STANDARDS.md` (storage key `tally.v1`)
- [ ] Categories and habits you can add, rename, reorder and archive; seeded with the starter set
- [ ] End-of-day tick screen, one tap per habit; fill in a missed day
- [ ] "Stop" habits scored the other way round (ticked = didn't do it)
- [ ] Counter habits — big tap counter with a daily goal, e.g. glasses of water (Click Counter)
- [ ] Year grid per category, colour depth = share of that category's habits done
- [ ] Levelling creature that grows as categories fill (Finch) — could share art with Ironlog's skins
- [ ] Evening reminder, best-effort: Android PWAs can't schedule exact notifications without a
      server, so this uses periodic background sync and may arrive late or not at all
- [ ] Export / import in the shared backup envelope, plus CSV

## Phase 2 — extras
- [ ] Streaks with a freeze day, so one miss doesn't wipe a run (Streakletics)
- [ ] Weight category pulls weigh-ins from wherever you log them, instead of retyping
- [ ] Optional: Kraftur's sleep log feeds the wellness row
