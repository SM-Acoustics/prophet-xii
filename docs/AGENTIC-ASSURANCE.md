# Agentic assurance — Prophet-XII

Adopts the proposed [SM-ENG-005 organization standard](https://github.com/SM-Acoustics/.github/blob/main/standards/SM-ENG-005-AGENTIC-ASSURANCE.md) after maintainer acceptance. Do not override the existing project baseline or other accepted requirements.

For every audio/UI feature, demonstrate an actual production signal/control path: MIDI -> voice/state -> DSP -> output and knob/automation -> parameter -> audible DSP effect. A UI indicator, generated stub, dead control, disabled test or mock-only audio output must not be called implemented. Validate glide, pitch wheel, envelopes, sustain, unison, filter resonance, drive and effects using independent numeric/audio references where available; include phase continuity, transition and polyphonic stress tests.

Hard real-time audio callbacks cannot allocate, block, perform disk/network I/O or invoke unbounded formatting. Provide callback timing distributions and max observed processing under representative stress; distinguish observed worst-case from proven WCET. Track oversampling/voice count, buffer size, CPU and target OS/plugin host. Review `unsafe`, thread ownership, data races, UI-to-audio parameter updates, serialization and security/licensing of presets and dependencies. A passing Rust test or standalone build is not proof of plugin-host compatibility.

Each PR must report new code reachability, original source/commit, test oracle, positive/negative audio cases, actual command/target, evidence hashes, capability status and failures. No agent changes CI or tests to manufacture PASS; no autonomous merge/release.
