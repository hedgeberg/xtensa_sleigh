GHIDRA XTENSA ESP32
=============

WIP WIP WIP PLEASE DOUBLE CHECK ALL DECOMP

Implementation of Xtensa architecture in SLEIGH. Targets esp32 specifically, meaning the xtensa variant is effectively hardcoded to be Little-Endian with Narrow Opcode and Register Window features. Tackled this because the only currently public Xtensa implementation lacks a huge set of instruction implementations & has no register windowing.

Decomp is pretty clean, surprisingly, but if you choose to use this please please please check all your decompilation results against the disassembly and make sure that you're getting the right behaviors. 

Several "odd" instructions like hardware loops and special register writes currently just emit opaque pcode in decompilation. Hope to change this soon, should not affect code flow for the most part. 

More details coming soon. Building details are the same as in my RL78 SLEIGH repo.
