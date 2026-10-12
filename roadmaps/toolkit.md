# Toolkit — roadmap

**Status:** idea · **Replaces:** scolio meter, Inclinometer, Compass, Soundcorset tuner · **Working name**

One small app of phone-sensor tools. All of it works offline with no AI.

## Phase 1 — tilt tools
- [ ] Repo, Pages, PWA shell per `STANDARDS.md`
- [ ] Inclinometer: live angle from the motion sensor, hold to freeze, zero on any surface
- [ ] Spine meter: phone laid across the back while bending forward → angle of trunk rotation,
      saved with date and a note — a log for the Schroth experiment, comparable over months
- [ ] Joint range-of-motion helper: strap or hold the phone on a limb, read start and end angle
- [ ] Compass with a bearing lock

## Phase 2 — sound tools
- [ ] Tuner: pitch from the mic, note name and cents off
- [ ] Metronome with tap tempo
- [ ] Pitch trainer: live line of your voice against a target note (Vocalista idea)
- [ ] Simple sound level meter — a first small step towards Hlusta

## Notes
- iPhones need a permission tap for motion sensors; Android Chrome doesn't. Build for Android first.
- Phone tilt readings are good to about a degree; fine for tracking change, not for diagnosis.
