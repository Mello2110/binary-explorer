---
id: "binary-explorer"
title: "0 / 1 — Binary Architecture & Data Explorer"
tagline: "Interactive zero-dependency explorer showing how identical binary sequences map across CPUs and data standards."
category: "tool"
status: "production"
featured: false
badge: "Open Source"
problemStatement: "Raw binary numbers look uniform on disk, making it difficult to grasp how identical sequences of ones and zeros are interpreted completely differently depending on the target processor instruction set or data encoding standard. Most online converters only translate binary to ASCII text without exposing machine-level decoding or abstraction layers."
technicalSolution: "A single-file, zero-dependency web application implements deterministic instruction decoders and register-level execution for MOS 6502, Zilog Z80, CHIP-8, and Intel 8086 alongside bidirectional UTF-8, raw hex dump, 24-bit RGB, and 24-bit HSL views. Every decoded line, character, or color swatch links back to its exact source bytes via hover highlighting and contextual error tooltips."
techStack:
  - "HTML5"
  - "CSS3"
  - "Vanilla JavaScript"
  - "Web Encoding API"
architectureHighlights:
  - "Deterministic opcode decoders and register-level ALU state execution for MOS 6502, Zilog Z80, CHIP-8, and Intel 8086."
  - "Two-dimensional navigation separating CPU architectures and abstraction layers (Assembler, C++, Python) from independent data standards (UTF-8, HEX, RGB, HSL)."
  - "Bidirectional UTF-8 encoding/decoding using native TextEncoder and TextDecoder with per-byte error classification tooltips."
  - "Zero-dependency single-page architecture with responsive mobile touch controls and bilingual EN/DE interface."
screenshots:
  - "/screenshots/binary-explorer/desktop.png"
  - "/screenshots/binary-explorer/mobile.png"
links:
  chromeWebStore: ""
  demoUrl: "https://mello2110.github.io/binary-explorer/"
  githubUrl: "https://github.com/Mello2110/binary-explorer"
sandbox:
  enabled: true
  type: "remote"
  embedUrl: "https://mello2110.github.io/binary-explorer/"
  notes: "Zero-dependency static web application hosted on GitHub Pages."
stats:
  version: "v1.0.0"
---

# 0 / 1 — Binary Architecture & Data Explorer

[![Status](https://img.shields.io/badge/Status-Active-emerald?style=flat-square)](#)
[![License](https://img.shields.io/badge/License-MIT-blue?style=flat-square)](#)

> Interactive zero-dependency explorer showing how identical binary sequences map across CPUs and data standards.

<p align="left">
  <a href="https://mello2110.github.io/binary-explorer/"><b>Live Demo / Web App</b></a> &nbsp;|&nbsp;
  <a href="https://mellow-solutions-hub.vercel.app"><b>Mellow Solutions Hub</b></a> &nbsp;|&nbsp;
  <a href="https://github.com/Mello2110"><b>Mellow Solutions on GitHub</b></a> &nbsp;|&nbsp;
  <a href="https://buymeacoffee.com/mellowsolutions"><b>Buy Me a Coffee</b></a>
</p>

---

## Problem & Motivation
Raw binary streams (`0` and `1`) are universal at the bit level, yet their meaning depends entirely on the ruleset reading them. A sequence that loads and adds values on a 6502 processor decodes to completely different instructions on a Z80, CHIP-8, or 16-bit Intel 8086 — and represents text or color pixels when read as UTF-8, RGB, or HSL.

## Technical Solution
**0 / 1** provides a calm, distraction-free workspace where users enter bits via keyboard (`0`, `1`, `Backspace`, `Esc`, `Ctrl+V`) or touch controls and switch in real time across two independent axes:
- **Processor & Abstraction Layer:** Switch horizontally between `6502`, `Z80`, `CHIP-8`, and `8086`, and vertically between `Assembler`, functional `C++`, and `Python` equivalents with logical operation categories (`load`, `add`, `logic`, `jump`, etc.).
- **Data Standards:** Switch cleanly to `UTF-8` (with bidirectional text-to-binary input), `HEX` (hex/decimal/ASCII byte dump), `RGB` (24-bit additive color), and `HSL` (24-bit perceptual color).

## Architecture & Tech Stack
- **Languages & Frameworks:** Vanilla HTML5, CSS3, and ES6+ JavaScript with zero external runtime dependencies or build steps.
- **Core Architecture:** Pure client-side state (`bits`, `arch`, `level`, `lang`) driving deterministic opcode tables, a live 8-bit progress indicator, hover-to-byte highlighting, clipboard copy actions, and a full `EN | DE` internationalization dictionary.

## Installation & Usage
1. Open the [Live Web App](https://mello2110.github.io/binary-explorer/) directly in any modern browser, or clone the repository and open `index.html`:
   ```bash
   git clone https://github.com/Mello2110/binary-explorer.git
   ```
2. Type `0` and `1` on your keyboard (or use the bottom touch controls) to build bytes and switch between architectures, abstraction layers, and data standards.

## License & Disclaimer
Part of the **Mellow Solutions** portfolio. Provided under the MIT License as-is for non-commercial and personal utility.
