# TARS Personality AI

> A TARS-inspired assistant (Interstellar) with adjustable honesty, humor and discretion settings — software first, robot later.

**Status:** pre-alpha scaffold (no code yet). **Feasibility rating:** 4/10 — fun and memorable; hardware cost and safety make the robot a long-term goal.
**Idea:** #04 in the owner's ideas backlog. **Author:** Oussama Elhadji (`@Bosaj`) <oussousselhadji@gmail.com>.

---

## Problem

Assistants have one fixed tone. TARS made personality a setting ("humor 75%") that the user controls. That idea is a good UX experiment for LLM assistants.

## Why build it (gap analysis)

The mechanical robot (four rotating blocks) needs servos, a frame, power and safety work. The personality controls can be built and tested now in software.

## Prior art & open bases to fork

- [pipecat-ai/pipecat](https://github.com/pipecat-ai/pipecat) — Real-time voice agent framework.
- [rhasspy/piper](https://github.com/rhasspy/piper) — Local TTS; pick a dry, robotic voice.
- [openai/whisper](https://github.com/openai/whisper) — Speech-to-text.

## Proposed architecture

1. Personality model: honesty, humor and discretion values (0-100) compiled into the system prompt and response style rules.
2. Voice front end shared with the Baymax companion idea.
3. Settings UI: "TARS, set humor to 60%" by voice, plus sliders in an app.
4. Robot phase: servo-driven block body, controlled over serial from the same software.

## Tech stack (proposed)

- TypeScript or Python voice agent
- LLM with structured style controls
- Web settings panel
- Later: ESP32 + servos

## Roadmap

- v0.1 — Personality sliders mapped to prompt + style rules, with tests.
- v0.2 — Voice commands to change settings.
- v0.3 — Desktop app with TARS-style UI.
- v0.4 — Robot body prototype.

---

## For LLM agents & contributors continuing this project

This repo is a **scaffold**: README + standard files, no implementation yet. If you are an AI agent asked to "continue developing", read this section first.

- Treat each slider as a testable contract: write example prompts and expected tone for 0, 50 and 100.
- Share the voice pipeline with `baymax-ai-companion` instead of building two.

**Ground rules:** keep this README in sync with reality as you build; prefer forking/reusing the bases above over greenfield code; write tests for anything correctness-critical; never commit secrets (see `.gitignore`); follow Conventional Commits (see `CONTRIBUTING.md`).

## Getting started

```bash
# nothing to run yet — this is a scaffold.
```

## 📄 License
**Proprietary & Commercial Software License** — All Rights Reserved © 2026 Oussama Elhadji (`@Bosaj`) <[oussousselhadji@gmail.com](mailto:oussousselhadji@gmail.com)>.

Unauthorized copying, distribution, resale, or reverse engineering is strictly prohibited. See [LICENSE](LICENSE) for full legal terms.
