# 1. Architecture

1. Personality model: honesty, humor and discretion values (0-100) compiled into the system prompt and response style rules.
2. Voice front end shared with the Baymax companion idea.
3. Settings UI: "TARS, set humor to 60%" by voice, plus sliders in an app.
4. Robot phase: servo-driven block body, controlled over serial from the same software.

## Proposed stack
- TypeScript or Python voice agent
- LLM with structured style controls
- Web settings panel
- Later: ESP32 + servos

## Open bases to fork
- [pipecat-ai/pipecat](https://github.com/pipecat-ai/pipecat) — Real-time voice agent framework.
- [rhasspy/piper](https://github.com/rhasspy/piper) — Local TTS; pick a dry, robotic voice.
- [openai/whisper](https://github.com/openai/whisper) — Speech-to-text.
