# Persona 4 PSP Port

<img width="300" height="517" alt="Senza titolo 269_20260917051917" src="https://github.com/user-attachments/assets/07a90065-9da6-440b-a80c-9d409b7347e4" />

--------------------------------------------------
This is an unofficial, fan-made project and is not affiliated with the original game's publisher or rights holders in any way.
All trademarks, characters, artwork, music, and other copyrighted material belong to ATLUS.

--------------------------------------------------
## Current Status / Progress

☑︎ Game decompiled 

☑︎ Project direction

-- Code Translation -- 

Built a tool that automatically converts Persona 4's original PS2 instructions into a form designed to run on the PSP.

The game contains about 1.1 million instructions. Around 76% can be converted directly. For instructions the PSP handles differently, the translator can rewrite them into steps the PSP can perform. This includes breaking down certain calculations and adapting how the game accesses memory.

The share of instructions that still need extra helper code has dropped from about 19% to 1.39%.

The generated code is estimated to be around 5 MB, which is promising for the PSP's limited memory. The translated code still needs further testing

