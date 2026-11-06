<div align="center">
  <img src="branding/nexus-wordmark.svg" alt="Nexus logo" width="140">
  <h1>Nexus</h1>

  <p><strong>A personal voice AI assistant that runs on a $0 budget.</strong></p>

  <img src="https://img.shields.io/badge/status-Early%20prototype-C08A2E?style=flat-square" alt="status"> <img src="https://img.shields.io/badge/platform-macOS%20/%20Web-0B0E13?style=flat-square" alt="platform"> <img src="https://img.shields.io/badge/license-proprietary-555555?style=flat-square" alt="license"> <img src="https://img.shields.io/badge/by-Aquila%20Digital%20LLC-14213D?style=flat-square" alt="Aquila Digital LLC">
</div>

> **Showcase repository.** The source code for Nexus is not published. This page presents what the product is and how it works.

## Overview

A Jarvis-style voice assistant that listens, remembers facts about you, controls your Mac and grows new tools over time, powered by free-tier services and local models.

## How it works

```mermaid
flowchart LR
  A["Hold to talk (browser mic or terminal)"] --> B["Speech-to-text"] --> C["Groq Llama 3.3 70B with tool loop + memory.md"] --> D["Kokoro local voice speaks the reply"]
```

## Features

- Terminal and web "Command Center" interfaces
- Persistent memory file read on every turn
- Mac control tools: open apps, screenshots, AppleScript, shell
- Local offline voice (Kokoro) and live CPU/RAM/battery telemetry
- Hands Mode gesture control (MediaPipe), Face Mode overlay
- High-fidelity HUD design handoff included (`design/`)

## Tech stack

| Layer | Choice |
|---|---|
| Language | Python (Flask web UI) |
| Brain | Groq (Llama 3.3 70B), free tier |
| Voice | Kokoro (local), Web Speech API |
| UI | HTML/CSS/JS canvas HUD, Space Grotesk + JetBrains Mono |

## Privacy & security

Runs locally; only model calls go to Groq. API keys are kept out of the project files.

## Brand

| | Name | Hex | Role |
|---|---|---|---|
| <img src="https://placehold.co/44x22/0B0E13/0B0E13.png" alt="#0B0E13" /> | Background | `#0B0E13` | App background |
| <img src="https://placehold.co/44x22/1E2836/1E2836.png" alt="#1E2836" /> | Panel | `#1E2836` | Panels |
| <img src="https://placehold.co/44x22/C08A2E/C08A2E.png" alt="#C08A2E" /> | Gold | `#C08A2E` | Primary accent |
| <img src="https://placehold.co/44x22/E0AC4C/E0AC4C.png" alt="#E0AC4C" /> | Gold Light | `#E0AC4C` | Glow / highlight |
| <img src="https://placehold.co/44x22/7FBF8F/7FBF8F.png" alt="#7FBF8F" /> | Online | `#7FBF8F` | Status good |

**Mark.** Gold-on-obsidian command-center HUD with a rotating AI-core globe.

**Voice.** Futuristic, sharp and a little cocky.

## Roadmap

- Wire Conversations and System Log to real data
- Port the Command Center design into the app

## License

Proprietary. Shared publicly for portfolio and demonstration purposes only. See [LICENSE](LICENSE).

---

<div align="center">

Built by [Aquila Digital LLC](https://github.com/Steven6Brown) · *Per Aspera Ad Astra*

</div>
