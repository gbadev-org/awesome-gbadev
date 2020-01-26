# Awesome Game Boy Advance development

A curated list of development resources for Game Boy Advance.

> WORK IN PROGRESS
> You're welcome to contribute on discord or opening Issues

## Documentation

- [GBATEK](https://problemkaputt.de/gbatek.htm) - Technical Info
- [CowBite Virtual Hardware Specifications](https://www.cs.rit.edu/~tjh8300/CowBite/CowBiteSpec.htm) - Incomplete GBA hardware documentation
- [The Audio Advance](http://belogic.com/gba/) - Audio hardware documentation and basic test ROMs

## Tutorials

- [Tonc](https://www.coranac.com/tonc/text/toc.htm) - Complete programming tutorial
- [Sound on the Gameboy Advance](http://web.archive.org/web/20140511141055/http://deku.rydia.net/program/sound1.html) - How to write your own sound mixer / MOD music player

## Articles

- [Gameboy Advance Resource Management](https://www.gamasutra.com/view/feature/131491/gameboy_advance_resource_management.php) - Allocation techniques for the GBA's various memory regions
- [Managing Sprite Cel VRAM on the Game Boy Advance](https://pineight.com/gba/managing-sprite-vram.txt) - Analysis of the VRAM streaming approach for animated sprites

## Libraries

- [posprintf](http://www.danposluns.com/gbadev/posprintf/index.html) - An `sprintf` routine written in Thumb assembler.

## Miscellanea

- [gba_bios](https://github.com/PikalaxALT/gba_bios) - (Work in progress) Disassembly of the Game Boy Advance BIOS

#### Dumping the GBA BIOS

- [Software interrupt $1F / MidiKey2Freq](https://gist.github.com/modwizcode/b4afc78ea74fb453be3bcaf3d3bc8adc), canonical method
- [Cracking the GBA BIOS](https://mgba.io/2017/06/30/cracking-gba-bios/) by endrift
- [Dumping the GBA BIOS](https://gist.github.com/MerryMage/797c523724e2dc02ada86a1cfadea3ee), another method by MerryMage

## Rom Hacking

- [Reverse Engineering a GameBoy Advance Game](https://medium.com/@bruno.macabeus/reverse-engineering-a-gameboy-advance-game-introduction-ec185bd8e02) - A series of detailed posts and talks about developing a [level editor](https://github.com/macabeus/klo-gba.js) for *Klonoa: Empire of Dreams*
