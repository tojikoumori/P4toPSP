# Persona 4 PSP Port

<img width="300" height="517" alt="Senza titolo 269_20260917051917" src="https://github.com/user-attachments/assets/07a90065-9da6-440b-a80c-9d409b7347e4" />

[![Buy Me a Coffee](https://img.shields.io/badge/Buy%20me%20a%20coffee-support-yellow?logo=buy-me-a-coffee)](https://buymeacoffee.com/tojikoumori)

--------------------------------------------------
This is an unofficial, fan-made project and is not affiliated with the original game's publisher or rights holders in any way.
All trademarks, characters, artwork, music, and other copyrighted material belong to ATLUS.

--------------------------------------------------
## Current Status / Progress

Extracted the European PS2 game files.

Built the recompilation tools needed to translate the game's code into C++.

Used PS2Recomp to translate thousands of functions from the original game's compiled code into C++ source files.

Built a custom runtime to recreate some of the PS2 system functions the game expects.

Got a diagnostic build past the initial kernel and memory setup.

Got the PS2 I/O system to start and respond to disc-file requests.

**16/10/2026 status**

The game now processes its file request buffer (all 7 request entries).

It performs the actual exchange with the (simulated) PS2 co-processor: it opens `DATA.CVM`, reads sector 0, and gets a status reply back.

**Real data is flowing** for the first time.
