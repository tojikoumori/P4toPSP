# Persona 4 PSP Port

<img width="300" height="517" alt="Senza titolo 269_20260917051917" src="https://github.com/user-attachments/assets/07a90065-9da6-440b-a80c-9d409b7347e4" />

[![Buy Me a Coffee](https://img.shields.io/badge/Buy%20me%20a%20coffee-support-yellow?logo=buy-me-a-coffee)](https://buymeacoffee.com/tojikoumori)

--------------------------------------------------
This is an unofficial, fan-made project and is not affiliated with the original game's publisher or rights holders in any way.
All trademarks, characters, artwork, music, and other copyrighted material belong to ATLUS.

--------------------------------------------------
## Current Status / Progress

Where we stand

- PC research harness: stable and useful. The recompiled game boots cleanly and runs for a minute+ with zero crashes. Fixed a long-standing crash bug (a race in the disk/machine engine).
- A known "limbo" bug remains: the game's background jobs get stuck at one specific "loading music files" step. We found the likely culprit function and are one step from confirming. (This is polish-on-top — it no longer blocks feasibility.)
- Hardware scan (above): the game is "chip-light" — no direct special-chip reliance.

What the PSP port actually needs (feasibility short-list)

1. CPU: recompile the game's code to PSP machine code. The huge translation we already have (8,203 clean pieces) is the raw material; we need it emitted for a second kind of chip. Big but mechanical work — the process is known and already proven once.
2. Special chips the PSP lacks: graphics, sound, and animation "spells" the PS2 cast at chips PSP doesn't have. Those each need a replacement (either software on the CPU or remapped to PSP's own hardware). That's the main design risk — new engineering, not an unsolvable mystery.
3. Memory: the game's footprint (~19 MB of program data + the way it streams data from the disc) fits PSP's memory only if some assets are reorganized. Early numbers say "tight but possible."
4. Disc swapping: the 4 data bundles (world, music, battles, surroundings) read currently by the harness would be plain files on the Memory Stick — that part gets easier, not harder.

Honest confidence
- Feasibility: allowing, not yet "yes" — the remaining unknowns are all on the PSP-cpu/side replacements (graphics & animation), and we haven't measured the game's steady-state FPS-style workload on a 333 MHz chip yet.
- The PC harness is the least risky asset we hold; the groundwork behind the translation package ($8k files) is done and reusable.

