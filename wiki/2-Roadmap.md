# 2. Roadmap

- v0.1 — Personality sliders mapped to prompt + style rules, with tests.
- v0.2 — Voice commands to change settings.
- v0.3 — Desktop app with TARS-style UI.
- v0.4 — Robot body prototype.

## Notes for contributors / LLM agents
- Treat each slider as a testable contract: write example prompts and expected tone for 0, 50 and 100.
- Share the voice pipeline with `baymax-ai-companion` instead of building two.
