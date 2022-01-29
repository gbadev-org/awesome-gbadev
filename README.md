# Awesome Game Boy Advance development

A curated list of development resources for Game Boy Advance.

Contribute adding resources or providing feedback through Pull Requests, Issues or joining us on [Discord](https://discord.io/gbadev). You can find a web version of this list [here](https://gbadev.net).

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
  * [Jams](#jams)
- [Miscellanea](#miscellanea)
  * [Dumping the GBA BIOS](#dumping-the-gba-bios)
  * [Reverse engineering](#reverse-engineering)
  * [Historical links](#historical-links)

---

# Introduction

- [Technical introduction to the GBA](https://copetti.org/projects/consoles/game-boy-advance)

## Community

- [GBADev Discord Server](https://discord.io/gbadev) - This is where everyone hangs out nowadays. Come say hi!  
  <details>
  <summary><em>Info for IRC users</em></summary>

  All rooms are bridged to IRC channels on [EFnet](http://www.efnet.org/?module=servers).

  **Main channel**  
  `#gbadev`        - general chat  

  **Additional channels**  
  `#gba-meta`      - community feedback/discussion  
  `#gba-help`      - help & support  
  `#gba-emudev`    - emulator development  
  `#gba-asm`       - ARM/Thumb assembly and CPU architecture  
  `#gba-showcase`  - share what you're working on!  
  `#gba-music`     - listening, composing and audio programming  
  `#gba-offtopic`  - off-topic chat  
  `#gba-docs`      - community documentation projects (tutorials, technical docs etc.)  
  `#gba-tools`     - tool discussion (grit, tiled, aseprite, etc.)  

  **Project-specific channels**  
  `#gba-toolchain` - gba-toolchain, agbabi and gba-plusplus development & support  
  `#butano`        - Butano engine development & support  
  `#natu`          - Natu toolkit development & support  
  </details>
- [GBADev](https://gbadev.org) - The longstanding homepage of the scene. Regularly updated with the lastest news and releases.
- [GBAtemp](https://gbatemp.net/categories/nintendo-gba-discussions.32/) - The site carries the GBA name, but now the console is relegated to the backbenches.

# Documentation

- [GBATEK](https://problemkaputt.de/gbatek.htm) - Programming specs for the GBA and NDS hardware
- [CowBite Virtual Hardware Specifications](https://www.cs.rit.edu/~tjh8300/CowBite/CowBiteSpec.htm) - Older GBA hardware documentation
- [The Audio Advance](http://belogic.com/gba/) - Audio hardware documentation and basic test ROMs

## Tutorials

- [Tonc](https://www.coranac.com/tonc/text/toc.htm) - Complete programming tutorial
- [Sound on the Gameboy Advance](https://deku.gbadev.org/program/sound1.html) - How to write your own sound mixer / MOD music player

## Articles

- [Gameboy Advance Resource Management](https://www.gamasutra.com/view/feature/131491/gameboy_advance_resource_management.php) - Allocation techniques for the GBA's various memory regions
- [Managing Sprite Cel VRAM on the Game Boy Advance](https://pineight.com/gba/managing-sprite-vram.txt) - Analysis of the VRAM streaming approach for animated sprites
- [Using Beepbox for GBA Music Composition](https://rentry.org/beepbox-gba-music)




# Software Development

## Compilers

- [devkitARM](https://devkitpro.org) - C/C++ cross-compiler toolchain, which includes libgba, libtonc, maxmod, and various tools and example projects.
- [gba-toolchain](https://github.com/felixjones/gba-toolchain) - GNU Arm Embedded Toolchain based alternative to devkitARM.
- [gvasm](https://github.com/velipso/gvasm) - Stand-alone assembler and disassembler (WIP) designed specifically for GBA homebrew

## Toolkits

- [rust-console](https://github.com/rust-console/gba) - GBA programming in Rust, plus tutorial.
- [natu](https://github.com/exelotl/natu) - GBA programming in Nim (provides wrapper around libtonc, maxmod and more).
- [gba-modern](https://github.com/JoaoBaptMG/gba-modern) - Write GBA games using modern C++.
- [ZigGBA](https://github.com/wendigojaeger/ZigGBA) - WIP SDK for creating GBA games using Zig (Inspired by Tonc).
- [Butano](https://github.com/GValiente/butano) - Modern C++ high level engine for the GBA.
- [BPCore Engine](https://github.com/evanbowman/BPCore-Engine) - Create GBA applications with the Lua programming language

## Libraries

- [agbabi](https://github.com/felixjones/agbabi) - Drop-in application binary interface library (context switching, division, irq, memcpy, sine).
- [gba-plusplus](https://github.com/felixjones/gba-plusplus) - Modern C++ alternative to libgba and libtonc.
- [HeartLib](https://github.com/Sterophonick/HeartLib) - Comprehensive C library inspired by the classic HAMLib.
- [libseven](https://github.com/LunarLambda/libseven) - Lightweight, from-scratch replacement for libgba.
- [GBAdv](https://github.com/sverx/GBAdv) - High level utilities on top of libgba.
- [Maxmod](https://maxmod.devkitpro.org) - Music and sound library (supports .mod, .xm, .s3m, .it)
- [Apex Audio System](https://github.com/stuij/apex-audio-system) - Music and sound library (supports .mod only, but _very_ good performance)
- [Krawall](https://github.com/sebknzl/krawall) - Music and sound library (supports .xm, .s3m)
- [Pimpmobile](https://github.com/kusma/pimpmobile) - Music library (supports .mod, .xm)
- [posprintf](http://www.danposluns.com/gbadev/posprintf/index.html) - An `sprintf` routine written in Thumb assembler.
- [GBFS](https://pineight.com/gba/#gbfs) - Practical filesystem

## Emulators

- [mGBA](https://mgba.io) - Actively developed GBA emulator. Runs on a bunch of platforms. Text debugger through GDB stub.
- [No$gba](https://problemkaputt.de/gba.htm) - Venerable GBA emulator. Windows only, but runs well under Wine. Not very actively maintained but still gets updates now and then. Sports graphical debugger.
- [NanoBoyAdvance](https://github.com/fleroviux/NanoBoyAdvance) - GBA emulator with high accuracy, especially in timing and CPU emulation. Currently lacking a GUI or debugger.
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
- [BlindJump](https://github.com/evanbowman/blind-jump-portable) - Adventure game, developed in 2020. Implementation of link-cable multiplayer, fully digital audio.
- [Tigermoth](https://github.com/pmprog/TigermothGBA) - Bullet hell game, developed for the GBAJam 2021
- [Duster](https://github.com/redthing1/duster) - A sleek strategy board game for the gba 
- [OpenLara](https://github.com/XProger/OpenLara) - Classic Tomb Raider open-source engine

# Jams

- [GBA Jam 2021](https://itch.io/jam/gbajam21/entries)
- [GBA Winter Jam '21](https://itch.io/jam/gba-winter-jam-2021/entries)

# Miscellanea

- [gba_bios](https://github.com/PikalaxALT/gba_bios) - WIP disassembly of the Game Boy Advance BIOS
- [GBA bare metal code](https://github.com/PeterLemon/GBA) - Various experiments by Krom, such as video playback and 3D, written in ARM Assembly

## Dumping the GBA BIOS

- [Software interrupt $1F / MidiKey2Freq](https://gist.github.com/modwizcode/b4afc78ea74fb453be3bcaf3d3bc8adc), canonical method
- [Cracking the GBA BIOS](https://mgba.io/2017/06/30/cracking-gba-bios/) by endrift
- [Dumping the GBA BIOS](https://gist.github.com/MerryMage/797c523724e2dc02ada86a1cfadea3ee), another method by MerryMage

## Reverse engineering

- [Reverse Engineering a GameBoy Advance Game](https://medium.com/@bruno.macabeus/reverse-engineering-a-gameboy-advance-game-introduction-ec185bd8e02) - A series of detailed posts and talks about developing a [level editor](https://github.com/macabeus/klo-gba.js) for *Klonoa: Empire of Dreams*
- [Pokemon Ruby](https://github.com/pret/pokeruby) - C programming language annotation of a Pokemon Ruby disassembly

## Historical links
- [HEL](http://www.console-dev.de/project/hel-library-for-gba/) - GBA C library built on top of HAM (a classic SDK from back in the day)
- [Headspin's Guide](http://members.iinet.net.au/~freeaxs/gbacomp/) to Compression, Files Systems, Screen Effects and MOD Players for the Gameboy Advance
