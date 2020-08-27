# Awesome Game Boy Advance development

A curated list of development resources for Game Boy Advance.

#### Work in progress notice
This list is still in early development. Please contribute adding resources or providing feedback through Pull Requests, Issues or joining us on [Discord](https://discord.gg/3ktqzBY).

## Table of Content

- [Introduction](#introduction)
  * [Community](#community)
- [Documentation](#documentation)
  * [Tutorials](#tutorials)
  * [Articles](#articles)
- [Software Development](#software-development)
  * [Compilers](#compilers)
  * [Toolkits](#toolkits)
  * [Libraries](#libraries)
  * [Emulators](#emulators)
- [Emulator Development](#emulator-development)
  * [Testing](#testing)
- [Homebrews](#homebrews)
- [Miscellanea](#miscellanea)
  * [Dumping the GBA BIOS](#dumping-the-gba-bios)
  * [Reverse engineering](#reverse-engineering)

---

Links marked with *WIP* are Work In Progress and still in development - don't expect complete resources.

# Introduction

- [Technical introduction to the GBA](https://copetti.org/projects/consoles/game-boy-advance)

## Community

- [#gba on gbdev Discord Server](https://discord.gg/gpBxq85) - Perhaps the only truely active GBA community today.
- [GBADEV](https://gbadev.org) - Tons and tons of info on GBA development: homebrew, tools, documentation.. Clearly laid out.
- [GBATEMP](https://gbatemp.net/categories/nintendo-gba-discussions.32/) - The site carries the GBA name, but now the console is relegated to the backbenches.

# Documentation

- [GBATEK](https://problemkaputt.de/gbatek.htm) - Technical Info
- [CowBite Virtual Hardware Specifications](https://www.cs.rit.edu/~tjh8300/CowBite/CowBiteSpec.htm) - Incomplete GBA hardware documentation
- [The Audio Advance](http://belogic.com/gba/) - Audio hardware documentation and basic test ROMs

## Tutorials

- [Tonc](https://www.coranac.com/tonc/text/toc.htm) - Complete programming tutorial
- [Sound on the Gameboy Advance](https://deku.gbadev.org/program/sound1.html) - How to write your own sound mixer / MOD music player

## Articles

- [Gameboy Advance Resource Management](https://www.gamasutra.com/view/feature/131491/gameboy_advance_resource_management.php) - Allocation techniques for the GBA's various memory regions
- [Managing Sprite Cel VRAM on the Game Boy Advance](https://pineight.com/gba/managing-sprite-vram.txt) - Analysis of the VRAM streaming approach for animated sprites



# Software Development

## Compilers

- [devkitARM](https://devkitpro.org) - C/C++ cross-compiler toolchain, which includes libgba, libtonc, maxmod, and various tools and example projects.
- [gba-toolchain](https://github.com/felixjones/gba-toolchain) - GNU Arm Embedded Toolchain based alternative to devkitARM.

### Toolkits

- [rust-console](https://github.com/rust-console/gba) - GBA programming in Rust, plus tutorial.
- [natu](https://github.com/exelotl/natu) - GBA programming in Nim (provides wrapper around libtonc, maxmod and more).
- [gba-modern](https://github.com/JoaoBaptMG/gba-modern) - Write GBA games using modern C++.
- [ZigGBA](https://github.com/wendigojaeger/ZigGBA) - WIP SDK for creating GBA games using Zig (Inspired by Tonc).

## Libraries

- [gba++](https://github.com/felixjones/gbaplusplus) - WIP modern C++ header-only library for GBA.
- [HeartLib](https://github.com/Sterophonick/HeartLib) - Comprehensive C library inspired by the classic HAMLib.
- [GBAdv](https://github.com/sverx/GBAdv) - High level utilities on top of libgba.
- [Maxmod](https://maxmod.devkitpro.org) - Music and sound effects library (supports .mod, .xm, .s3m, .it)
- [Krawall](https://github.com/sebknzl/krawall) - Music and sound effects library (supports .xm, .s3m)
- [Pimpmobile](https://github.com/kusma/pimpmobile) - Music library (supports .mod, .xm)
- [posprintf](http://www.danposluns.com/gbadev/posprintf/index.html) - An `sprintf` routine written in Thumb assembler.
- [GBFS](https://pineight.com/gba) - Practical filesystem

## Emulators

- [mGBA](https://mgba.io) - Actively developed GBA emulator. Runs on a bunch of platforms. Text debugger through GDB stub.
- [No$gba](https://problemkaputt.de/gba.htm) - Venerable GBA emulator. Windows only, but runs well under Wine. Not very actively maintained but still gets updates now and then. Sports graphical debugger.
- [MiSTer FPGA implementation](https://github.com/MiSTer-devel/GBA_MiSTer) - Needs [MiSTer](https://github.com/MiSTer-devel/Main_MiSTer/wiki) setup to run.

# Emulator Development

## Testing

- [mGBA test suite](https://github.com/mgba-emu/suite)
- [GBA Suite](https://github.com/jsmolka/gba-suite)
- [240p-test-mini](https://github.com/pinobatch/240p-test-mini) - video signal tests

# Homebrews

- [Goodboy Advance](https://github.com/exelotl/goodboy-advance) - Made in 2018, and has a nice bit of information on how it's made.
- [Celeste Classic](https://github.com/JeffRuLz/Celeste-Classic-GBA) - 2019 port of Pico8 version of Celeste.
- [GBADoom](https://github.com/doomhack/GBADoom) - 2019/2020 GBA port of prBoom version of Doom.

# Miscellanea

- [gba_bios](https://github.com/PikalaxALT/gba_bios) - WIP disassembly of the Game Boy Advance BIOS
- [GBA bare metal code](https://github.com/PeterLemon/GBA) - Various experiments by Krom, such as video playback and 3D, written in ARM Assembly

## Dumping the GBA BIOS

- [Software interrupt $1F / MidiKey2Freq](https://gist.github.com/modwizcode/b4afc78ea74fb453be3bcaf3d3bc8adc), canonical method
- [Cracking the GBA BIOS](https://mgba.io/2017/06/30/cracking-gba-bios/) by endrift
- [Dumping the GBA BIOS](https://gist.github.com/MerryMage/797c523724e2dc02ada86a1cfadea3ee), another method by MerryMage

## Reverse engineering

- [Reverse Engineering a GameBoy Advance Game](https://medium.com/@bruno.macabeus/reverse-engineering-a-gameboy-advance-game-introduction-ec185bd8e02) - A series of detailed posts and talks about developing a [level editor](https://github.com/macabeus/klo-gba.js) for *Klonoa: Empire of Dreams*

## Historical links
- [HAM mirror](https://github.com/Sterophonick/Mirror-HAM) - A classic SDK from back in the day :)
- [Headspin's Guide](http://members.iinet.net.au/~freeaxs/gbacomp/) to Compression, Files Systems, Screen Effects and MOD Players for the Gameboy Advance
