# gadgets-games-scramble

Scramble for the gadgets of [polpo](https://github.com/polpo-system/polpo): the sliding puzzle: unscramble the picture.

```
portia.Install gadgets-games-scramble
```

## Playing

    Desktops.OpenDoc (Scramble.NewDoc)    a new puzzle
    Scramble.ChangePict ^                 another picture for the marked (*) document
    Scramble.ChangeSize ^                 another size, as columns and rows (3 3)

`tools/Scramble.Tool` has these commands to click.

## What is here

    src/Scramble.Mod                 the game
    share/Clown.Pict, Grapes.Pict    pictures to play with (Default.Pict comes with gadgets)
    tools/Scramble.Tool
    test/ScrambleTest.Mod

Scramble is by Emil Zeller, from ETH Native Oberon 2.3.6. The source was converted from an Oberon text to plain text; the first commit has it
unchanged. It compiles unchanged with all five of polpo's compilers (x86, ARM, ARMv7, RISC-V,
MIPS).

## Tests

    ScrambleTest.Run      2 checks: a puzzle document made and loaded; it needs the desktop's display

The license is GPL-3 (`LICENSE`); the code comes from ETH Oberon, whose license (`LICENSE.ETH`)
asks to keep its copyright notice and conditions, which `LICENSE.ETH` does.
