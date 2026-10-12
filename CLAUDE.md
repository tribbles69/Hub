# Working in this repo

This is Aaron's app hub: an index and roadmaps, plus a small launcher page (`index.html`).

- `apps.json` is the source of truth for which apps exist. When an app is created, renamed,
  ships a version or changes status, update `apps.json` **and** the table in `README.md`.
- Roadmaps in `roadmaps/` use `- [ ]` / `- [x]` checkboxes; the launcher counts them for its
  progress bars, so keep tasks as checkboxes and tick them with the version that shipped them.
- When an app gets its own repo, move its roadmap to that repo's `r&d/ROADMAP.md`, point
  `apps.json` `roadmap` at the raw URL, and delete the copy here.
- Apps follow `STANDARDS.md`. Don't change a standard without asking Aaron.
- Launcher changes: bump `VERSION` in `index.html` and the cache name in `sw.js` together.
- British English, kg, ISO dates.
