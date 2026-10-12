# House rules for every app

Every app in this hub follows these, so they look and behave like one family and
your data always stays yours. Ironlog set most of them first; when in doubt, copy Ironlog.

## Your data
- **Local-first.** The phone is the source of truth. No server of ours ever holds
  your data.
- **Backups go to your own Google Drive** (when an app adds it, it follows
  Ironlog's Drive sync, shipped in Ironlog 0.33.0 (roadmap B6)). Until then: a manual export button.
- **AI is optional.** Every app works fully without it. When AI is used, it runs on
  your own API key, entered on the device.

## One backup format
Every app exports the same envelope, so one tool can back up or merge them all:

```json
{
  "app": "kraftur",
  "formatVersion": 1,
  "appVersion": "1.1.0",
  "exportedAt": "2026-10-12T19:30:00Z",
  "data": { }
}
```

- File name: `<app>-backup-YYYY-MM-DD.json`.
- Import must accept older `formatVersion`s and ignore unknown keys.
- Offer a CSV too wherever the data is a table (handy for a GP, a spreadsheet, or Claude).
- Existing apps: Ironlog has its own export; Kraftur uses `{app, version, exported, days}`.
  Move both to the envelope next time they're touched, keeping import of the old shapes.

## Same origin, so apps can share
Apps hosted under `tribbles69.github.io` (GitHub Pages) share **one origin** in the browser.
That means apps on the same phone can read each other's local data with no server:
the Stamina Meter could read Food's diary and Ironlog's sessions directly.

The catch: clearing site data for `tribbles69.github.io` in Chrome wipes **every**
app on that origin at once. Back up before clearing anything.

So:
- **Namespace every storage key**: `<app>.<thing>.v<n>` (e.g. `kraftur.v1`,
  `food.diary.v1`). Never use a bare key like `data` or `settings`.
- **Only the owning app writes its keys.** Other apps read, never write.
- Each app documents its stored shape in its repo (`r&d/DATA.md`) so others can read it safely.

## Building and shipping
- Installable PWA: `manifest.webmanifest`, icons (192, 512, maskable 512), `sw.js`.
- `version.json` → `{"version": "x.y.z"}`. Every shipped change bumps it **and** the
  cache name in `sw.js`, or installed copies keep the old version.
- `CHANGELOG.md` at the repo root, newest first.
- `r&d/ROADMAP.md` in each app's repo once it has its own repo; until then the roadmap
  lives here in `roadmaps/`.
- `CLAUDE.md` in each repo, so any Claude Code session can pick the work up cold.
- One feature per commit. Syntax-check script blocks before pushing a single-file app.

## Look and feel
- Phone-first, dark theme, big tap targets (48px+), works one-handed.
- Units: kg, cm, °C, 24-hour time. British English.
- Dates stored as ISO (`2026-10-12`), shown as `Mon 12 Oct`.
- No dark patterns, no streak guilt, no upsells.
