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

- [GBAdev Forum](https://forum.gbadev.net) - Our new hub for announcements and long-form discussion. It's a good place to ask questions and share progress on your projects.
- [GBAdev Discord](https://gbadev.net) - This is where everyone hangs out to chat nowadays. Come say hi!  
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
  `#gbajam`        - hang out with other GBA Jam participants & share your progress  

  **Project-specific channels**  
  `#gba-toolchain` - gba-toolchain, agbabi, and gba-hpp development & support  
  `#butano`        - Butano engine development & support  
  `#natu`          - Natu toolkit development & support  
  </details>
  
### Other places
- [GBAdev.org](https://gbadev.org) - The longstanding homepage of the scene. Still updated with news and releases (but the forums have been broken for a while).
- [GBAtemp](https://gbatemp.net/categories/nintendo-gba-discussions.32/) - The site carries the GBA name, but nowadays the console is relegated to the backbenches. It's a good place to talk about gaming and hardware though.

# Documentation

- [GBATEK](https://problemkaputt.de/gbatek.htm) - Programming specs for the GBA and NDS hardware
- [CowBite Virtual Hardware Specifications](https://www.cs.rit.edu/~tjh8300/CowBite/CowBiteSpec.htm) - Older GBA hardware documentation
- [The Audio Advance](http://belogic.com/gba/) - Audio hardware documentation and basic test ROMs

## Tutorials

- [Tonc](https://www.coranac.com/tonc/text/toc.htm) - Complete programming tutorial
- [Compile C++ for GBA in under an hour](https://www.youtube.com/watch?v=EMeie_gSgDU) - Cinemint's video for getting started with C++/Butano
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
- [TinyGo](https://github.com/tinygo-org/tinygo) - An alternative Go compiler for embedded systems, that supports GBA compilation

## Toolkits

- [rust-console](https://github.com/rust-console/gba) - GBA programming in Rust, plus tutorial.
- [natu](https://github.com/exelotl/natu) - GBA programming in Nim (provides wrapper around libtonc, maxmod and more).
- [gba-modern](https://github.com/JoaoBaptMG/gba-modern) - Write GBA games using modern C++.
- [ZigGBA](https://github.com/wendigojaeger/ZigGBA) - WIP SDK for creating GBA games using Zig (Inspired by Tonc).
- [Butano](https://github.com/GValiente/butano) - Modern C++ high level engine for the GBA.
- [BPCore Engine](https://github.com/evanbowman/BPCore-Engine) - Create GBA applications with the Lua programming language
- [GBA Dlang](https://github.com/redthing1/gba_dlang) - WIP SDK for GBA development using D, using LLVM toolchain. provides fully functional TONC, GBFS, Maxmod.
- [dusk](https://github.com/redthing1/dusk) - Simple, lightweight, intuitive framework for GBA game development
- [gbsenpai](https://github.com/asiekierka/gbsenpai) - GB Studio player GBA port with some enhancements.
- [meson-gba](https://github.com/LunarLambda/meson-gba) - Meson-based GBA toolkit with support for many different libraries and tools.
- [sdk-seven](https://github.com/LunarLambda/sdk-seven) - (WIP) Modern C libraries, runtimes, and tooling for GBA development.
- [rath](https://github.com/stuij/rath) - Forth programming environment for the Game Boy Advance
- [ada-gba-dev](https://github.com/98devin/ada-gba-dev) - A build system, libraries, and tools for producing programs for the Game Boy Advance using the Ada programming language.

## Libraries

- [agbabi](https://github.com/felixjones/agbabi) - Drop-in application binary interface library (context switching, division, irq, memcpy, sine).
- [gba-hpp](https://github.com/felixjones/gba-hpp) - C++20 header-only library for GBA development.
- [HeartLib](https://github.com/Sterophonick/HeartLib) - Comprehensive C library inspired by the classic HAMLib.
- [libseven](https://github.com/LunarLambda/sdk-seven) - Modern, from-scratch replacement for libgba and libtonc.
- [GBAdv](https://github.com/sverx/GBAdv) - High level utilities on top of libgba.
- [Maxmod](https://maxmod.devkitpro.org) - Music and sound library (supports .mod, .xm, .s3m, .it)
- [Apex Audio System](https://github.com/stuij/apex-audio-system) - Music and sound library (supports .mod only, but _very_ good performance)
- [Krawall](https://github.com/sebknzl/krawall) - Music and sound library (supports .xm, .s3m)
- [Pimpmobile](https://github.com/kusma/pimpmobile) - Music library (supports .mod, .xm)
- [GBT Player](https://github.com/AntonioND/gbt-player) - Music library that uses the DMG sound channels (close to 0% CPU usage).
- [posprintf](http://www.danposluns.com/gbadev/posprintf/index.html) - An `sprintf` routine written in Thumb assembler.
- [GBFS](https://pineight.com/gba/#gbfs) - Practical filesystem
- [agb](https://github.com/agbrs/agb) - Rust library. It attempts to be a high level abstraction over the internal workings of the Game Boy Advance whilst still being high performance and memory efficient.
- [gbaLib](https://github.com/MnlPhlp/gbaLib) - Library for programming the GBA with TinyGo

## Emulators

- [mGBA](https://mgba.io) - Actively developed GBA emulator. Runs on a bunch of platforms. Text debugger through GDB stub.
- [No$gba](https://problemkaputt.de/gba.htm) - Venerable GBA emulator. Windows only, but runs well under Wine. Not very actively maintained but still gets updates now and then. Sports graphical debugger.
- [NanoBoyAdvance](https://github.com/nba-emu/NanoBoyAdvance) - GBA emulator with high accuracy, especially in timing and CPU emulation. Does not have debugging features.
- [SkyEmu](https://github.com/skylersaleh/SkyEmu) - GB/GBA/NDS Emulator with built in debuggers, REST API for scripting, and high accuracy. 
- [MiSTer FPGA implementation](https://github.com/MiSTer-devel/GBA_MiSTer) - Needs [MiSTer](https://github.com/MiSTer-devel/Main_MiSTer/wiki) setup to run.

# Emulator Development

## Testing

- [mGBA test suite](https://github.com/mgba-emu/suite)
- [GBA Suite](https://github.com/jsmolka/gba-suite)
- [240p-test-mini](https://github.com/pinobatch/240p-test-mini) - video signal tests
- [NBA hardware tests](https://github.com/nba-emu/hw-test)

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
- [GBA Jam 2022](https://itch.io/jam/gbajam22/entries)
- [GBA Winter Jam '23](https://itch.io/jam/gba-winter-jam-23)

# Miscellanea

- [gba_bios](https://github.com/PikalaxALT/gba_bios) - WIP disassembly of the Game Boy Advance BIOS
- [GBA bare metal code](https://github.com/PeterLemon/GBA) - Various experiments by Krom, such as video playback and 3D, written in ARM Assembly
- [dkarm_gba_docker](https://github.com/redthing1/dkarm_gba_docker) - A Docker image that includes DevkitARM and other GBA SDK tools, packaged together to allow a consistent toolchain configuration and reproducibility in builds. Also can be helpful in ensuring a consistent build environment for continuous integration.

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
