# Awesome Game Boy Advance development

A curated list of development resources for Game Boy Advance.

> WORK IN PROGRESS
> You're welcome to contribute on discord or opening Issues

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

- [Devkitpro](https://devkitpro.org) - C/C++ compiler.

### GBA programming toolkit in language X

- [rust-console](https://github.com/rust-console/gba) - GBA programming in Rust, plus tutorial.
- [natu](https://github.com/exelotl/natu) - GBA programming in Nim (loosely based on Tonc tutorial)
- [gba-modern](https://github.com/JoaoBaptMG/gba-modern) - Write GBA games using modern C++.

## Libraries

- [gba++](https://github.com/felixjones/gbaplusplus) - Modern C++ library for GBA.
- [Maxmod](https://maxmod.devkitpro.org) - Mixes music and sound effects for your games.
- [posprintf](http://www.danposluns.com/gbadev/posprintf/index.html) - An `sprintf` routine written in Thumb assembler.
- [GBFS](https://pineight.com/gba) - practical filesystem

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

- [Goodboy Advance - game jam version](https://github.com/exelotl/goodboy-advance) - Made in 2018, and has a nice bit of information on how it's made.
- [Celeste Classic](https://github.com/JeffRuLz/Celeste-Classic-GBA) - 2019 port of Pico8 version of Celeste.
- [GBADoom](https://github.com/doomhack/GBADoom) - 2019/2020 GBA port of prBoom version of Doom.

# Miscellanea

- [gba_bios](https://github.com/PikalaxALT/gba_bios) - (Work in progress) Disassembly of the Game Boy Advance BIOS

## Dumping the GBA BIOS

- [Software interrupt $1F / MidiKey2Freq](https://gist.github.com/modwizcode/b4afc78ea74fb453be3bcaf3d3bc8adc), canonical method
- [Cracking the GBA BIOS](https://mgba.io/2017/06/30/cracking-gba-bios/) by endrift
- [Dumping the GBA BIOS](https://gist.github.com/MerryMage/797c523724e2dc02ada86a1cfadea3ee), another method by MerryMage

## Reverse engineering

- [Reverse Engineering a GameBoy Advance Game](https://medium.com/@bruno.macabeus/reverse-engineering-a-gameboy-advance-game-introduction-ec185bd8e02) - A series of detailed posts and talks about developing a [level editor](https://github.com/macabeus/klo-gba.js) for *Klonoa: Empire of Dreams*
