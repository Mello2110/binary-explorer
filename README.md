# 0 / 1 — Binary Architecture & Data Explorer

A minimalist, zero-dependency web app for exploring how raw binary sequences (`0` and `1`) are interpreted across different processor architectures and data standards.

## Features

- **CPU Architectures (`Assembler` / `C++` / `Python`):**
  - **MOS 6502** (8-bit: C64, NES, Apple II)
  - **Zilog Z80** (8-bit: Game Boy family, ZX Spectrum)
  - **CHIP-8** (16-bit fixed-width virtual machine)
  - **Intel 8086** (16-bit x86 ancestor)
- **Data Standards:**
  - **UTF-8** (bidirectional: type `0`/`1` or type text to generate UTF-8 binary)
  - **HEX** (raw hex, decimal, and ASCII byte view)
  - **RGB** (24-bit additive color)
  - **HSL** (24-bit perceptual color)
- **Interactive Details:** Live 8-bit progress indicator, hover-to-byte highlighting, logical instruction categories, contextual error tooltips, copy buttons, and `EN | DE` language toggle.

## Usage

Open `index.html` directly in any modern browser or host via GitHub Pages.
