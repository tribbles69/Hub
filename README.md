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
| Ironlog | Live (APK planned) | Hevy, Lyfta, Liftosaur, JuggernautAI, Tonnage, Liftoff, StrengthLog, VBT apps, mobility apps | [Ironlog](https://github.com/tribbles69/Ironlog) | [in repo](https://github.com/tribbles69/Ironlog/blob/main/r%26d/ROADMAP.md) + [audit extras](roadmaps/ironlog-from-audit.md) |
| Kraftur | Live | Sleep Tracker | [Boner](https://github.com/tribbles69/Boner) | [kraftur](roadmaps/kraftur.md) |
| Rounds | Live | — | [rounds](https://github.com/tribbles69/rounds) | [rounds](roadmaps/rounds.md) |
| Tally | Live | Finch, Streakletics, Click Counter | [Tally](https://github.com/tribbles69/Tally) | [in repo](https://github.com/tribbles69/Tally/blob/main/r%26d/ROADMAP.md) |
| Logn | Live | — | [Logn](https://github.com/tribbles69/Logn) | [logn](roadmaps/logn.md) |
| Toolkit | Idea | scolio meter, Inclinometer, Compass, Soundcorset | — | [toolkit](roadmaps/toolkit.md) |
| Home Rounds | Idea | Chorefriend | — | [chores](roadmaps/chores.md) |
| Stamina Meter | Idea | — | — | [stamina](roadmaps/stamina.md) |
| Symptom Logger | Idea | — | — | [symptoms](roadmaps/symptoms.md) |
| Pay-later Tracker | Idea | — | — | [paylater](roadmaps/paylater.md) |
| Food Bank Stock | Idea | — | — | [foodbank](roadmaps/foodbank.md) |
| Hlusta (PC) | Idea | — | — | [hlusta](roadmaps/hlusta.md) |
| Social Manager | Idea | — | — | [social](roadmaps/social.md) |
| Presence Monitor | Idea | — | — | [presence](roadmaps/presence.md) |
| Clewsco Dashboard | Idea | — | [Clewsco](https://github.com/tribbles69/Clewsco) (private) | in repo |
| Food | Benched | Cronometer, MyFitnessPal | — | [food](roadmaps/food.md) |
| Kpho | Retired | → Food | [Kpho](https://github.com/tribbles69/Kpho) | — |

## Build order

1. **Ironlog audit extras** — then delete the lifting and VBT apps.
2. **Toolkit** — quick sensor builds; the spine meter helps the Schroth experiment.
3. **Home Rounds**, **Stamina Meter**, **Pay-later Tracker**.

Benched: **Food** (2026-10-21). Cronometer's free tier covers it well, so it stays on the phone
for now. Ironlog's food export and lookup tables wait in `Ironlog/r&d/food-handover` if it's revived.

Other projects that aren't phone apps (Bergmál, Endalaus, Hollow Pawns, Wythall Civic Watch,
the AI teammate bots, the strength records site, the Clewsco site, the Total War mods) stay out
of this index unless they grow an app.

## Hosting

Sites are moving from GitHub Pages to Cloudflare Pages so repos can go private while keeping
push-to-deploy. Static sites first. The `url` in `apps.json` changes as each one moves.

## Adding a new app
1. Create the repo on GitHub (Aaron), private, and connect it to Cloudflare Pages to deploy from `main`, root.
2. Add it to `apps.json` and the table above, with a roadmap in `roadmaps/`.
3. Follow `STANDARDS.md`.
