# Logn — roadmap

**Status:** live · standalone PWA ([tribbles69/logn](https://github.com/tribbles69/logn))

*Logn* (Icelandic: dead calm). Visuals, breath and attention for shifting state: Downshift
(breath pacer), Cool-down (box breathing over Drift's Silk scene, with watch heart rate),
HRV check (camera or RR intervals), Drift (wind-down before bed) and Lock-in (pre-single
focus drill). Data stays in the browser with a JSON export.

## Built
- [x] Downshift, Cool-down, HRV check, Drift and Lock-in modes
- [x] Before/after check-ins, pulse and control-pause measures, Cool-down comparison
- [x] Watch heart rate over Web Bluetooth, same approach as Ironlog's cardio
- [x] HRV camera check fix for a saturated torch image (logn #4)

## Next
- [ ] Use it for a few weeks and read the Cool-down comparison: which setup actually works?
- [ ] Google Drive backup, following Ironlog's approach (`STANDARDS.md`)
- [ ] `version.json` so the launcher can show the version

## Into Ironlog
- [ ] Cool-down, calm rests, Lock-in and the HRV check move into Ironlog — tracked as
      **Ironlog roadmap E15** (added 2026-11-09). Logn stays a standalone app.
