# Hlusta — roadmap

**Status:** idea · Windows desktop app, not a phone app · built with Claude Code

Your own take on the SPL HawkEye meter: analyses whatever music or game audio is playing on the
PC and shows it on the side monitor. Later, hosts VSTs so game audio can run through a mastering
chain.

## Phase 1 — the meter
- [ ] Capture system audio (WASAPI loopback) and choose the stack (e.g. JUCE)
- [ ] Loudness: momentary, short-term and integrated LUFS, true peak
- [ ] Spectrum analyser and stereo correlation / goniometer
- [ ] Borderless window sized for the side monitor

## Phase 2 — the host
- [ ] Load a VST3 chain on the system audio (compressor, limiter)
- [ ] Output through a virtual audio device so games play through the chain
- [ ] Save chains as presets

## Later
- [ ] Your old plugin ideas: multiband harmonic distortion; a synth with unlimited stacked waveforms
- [ ] The Toolkit's sound level meter is a cheap way to try the metering maths first
