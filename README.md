# Hub

Index of Aaron's own apps: what exists, where it lives, what's next. The aim is to
replace the third-party apps on the phone with our own, one at a time, so the data
stays ours. Open the launcher at the hub's GitHub Pages link to see it all on the phone.

- `apps.json` — the registry the launcher reads. Add an app here first.
- `roadmaps/` — a roadmap per app until it has its own repo.
- `STANDARDS.md` — house rules every app follows (storage, backups, versioning).
- Full audit of every app on the phone: the "App Audit — Rebuild Plan" doc in Claude.

## Apps

| App | Status | Replaces | Repo | Roadmap |
| --- | --- | --- | --- | --- |
| Ironlog | Live | Hevy, Lyfta, Liftosaur, JuggernautAI, Tonnage, Liftoff, StrengthLog, VBT apps, mobility apps | [Ironlog](https://github.com/tribbles69/Ironlog) | [in repo](https://github.com/tribbles69/Ironlog/blob/main/r%26d/ROADMAP.md) + [audit extras](roadmaps/ironlog-from-audit.md) |
| Kraftur | Live | Sleep Tracker | [Boner](https://github.com/tribbles69/Boner) | [kraftur](roadmaps/kraftur.md) |
| Rounds | Live | — | [rounds](https://github.com/tribbles69/rounds) | [rounds](roadmaps/rounds.md) |
| Food | Next | Cronometer, MyFitnessPal | — | [food](roadmaps/food.md) |
| Tally | Next | Finch, Streakletics, Click Counter | — | [tally](roadmaps/tally.md) |
| Toolkit | Idea | scolio meter, Inclinometer, Compass, Soundcorset | — | [toolkit](roadmaps/toolkit.md) |
| Home Rounds | Idea | Chorefriend | — | [chores](roadmaps/chores.md) |
| Stamina Meter | Idea | — | — | [stamina](roadmaps/stamina.md) |
| Pay-later Tracker | Idea | — | — | [paylater](roadmaps/paylater.md) |
| Food Bank Stock | Idea | — | — | [foodbank](roadmaps/foodbank.md) |
| Hlusta (PC) | Idea | — | — | [hlusta](roadmaps/hlusta.md) |
| Social Manager | Idea | — | — | [social](roadmaps/social.md) |
| Presence Monitor | Idea | — | — | [presence](roadmaps/presence.md) |
| Kpho | Retired | → Food | [Kpho](https://github.com/tribbles69/Kpho) | — |

## Build order

1. **Food** — two paid apps out; Ironlog's food export and lookup tables are waiting in `Ironlog/r&d/food-handover`.
2. **Tally** — small, already designed.
3. **Ironlog audit extras** — then delete the lifting and VBT apps.
4. **Toolkit** — quick sensor builds; the spine meter helps the Schroth experiment.
5. **Home Rounds**, **Stamina Meter**, **Pay-later Tracker**.

Other projects that aren't phone apps (Bergmál, Endalaus, Hollow Pawns, Wythall Civic Watch,
the AI teammate bots) stay out of this index unless they grow an app.

## Adding a new app
1. Create the repo on GitHub (Aaron), then Settings → Pages → deploy from `main`, root.
2. Add it to `apps.json` and the table above, with a roadmap in `roadmaps/`.
3. Follow `STANDARDS.md`.
