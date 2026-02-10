# Braille Drawing

The 256 braille Unicode characters (⠀ through ⣿) form a sub-pixel drawing system. Each character is a 2×4 grid of dots that can be individually on or off — giving double the horizontal resolution and quadruple the vertical resolution of regular text characters.

This means curves can be smooth. Gradients can be fine. Faces can have expression. Forms that feel impossible in text become possible.

## How Braille Characters Work

Each braille cell has 8 dot positions:

```
  ⠁ ⠈       dot 1  dot 4
  ⠂ ⠐       dot 2  dot 5
  ⠄ ⠠       dot 3  dot 6
  ⡀ ⢀       dot 7  dot 8
```

Any combination of dots makes a valid character. `⠁` is just the top-left dot. `⣿` is all dots filled. `⡇` is the entire left column. `⠛` is the top four dots. There are 256 total patterns.

## Smooth Curves

```
A circle:
          ⣀⣀⣠⣤⣤⣤⣄⣀⣀
       ⣠⠞⠉⠀⠀⠀⠀⠀⠀⠀⠉⠳⣄
     ⣠⠋⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠙⣄
    ⡞⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢳
   ⡇⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢸
   ⡇⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢸
    ⢳⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢀⡞
     ⠈⠳⣄⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣠⠞⠁
       ⠈⠙⠲⢤⣀⣀⣀⣀⣀⡤⠖⠋⠁

A wave:
⠀⠀⠀⠀⠀⠀⠀⠀⣀⣀⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣀⣀⡀
⠀⠀⠀⠀⠀⣠⠞⠉⠀⠀⠉⠳⣄⠀⠀⠀⠀⠀⠀⠀⣠⠞⠉⠀⠀⠉⠳⣄
⠀⠀⠀⣠⠞⠁⠀⠀⠀⠀⠀⠀⠈⠳⣄⠀⠀⠀⣠⠞⠁⠀⠀⠀⠀⠀⠀⠈⠳⣄
⣠⠞⠉⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⠳⣠⠞⠁
```

## Faces and Figures

```
A face:
         ⣀⣀⣀⣀⣀⣀⣀
      ⣠⠞⠉⠀⠀⠀⠀⠀⠉⠳⣄
    ⣠⠋⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠙⣄
   ⡏⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢹
  ⡇⠀⠀⣴⣦⠀⠀⠀⠀⠀⣴⣦⠀⠀⠀⢸
  ⡇⠀⠀⠛⠋⠀⠀⠀⠀⠀⠛⠋⠀⠀⠀⢸
  ⢳⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⡞
   ⢳⡀⠀⠀⠀⠙⠒⠒⠋⠀⠀⠀⠀⡞
    ⠈⠳⣄⠀⠀⠀⠀⠀⠀⠀⠀⣠⠞
       ⠉⠛⠒⠒⠒⠒⠛⠉

An eye:
    ⣠⣤⣤⣤⣤⣤⣤⣤⣤⣤⣄
   ⣿⣿⣿⡿⠟⠛⠛⠻⢿⣿⣿⣿
   ⣿⣿⠟⠁⠀⣴⣶⡄⠀⠈⠻⣿⣿
   ⣿⣿⠀⠀⠀⣿⣿⡇⠀⠀⠀⣿⣿
   ⣿⣿⣦⡀⠀⠙⠋⠀⢀⣴⣿⣿
   ⣿⣿⣿⣿⣶⣤⣤⣶⣿⣿⣿⣿
    ⠉⠛⠛⠛⠛⠛⠛⠛⠛⠉
```

## Braille Gradients

```
Light to dense, using dot count:
⠀⠀⠁⠂⠃⠄⠅⠆⠇⠈⠉⠊⠋⠌⠍⠎⠏⡀⡁⡂⣀⣁⣂⣃⣄⣅⣆⣇⣏⣟⣿⣿

Vertical gradient:
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⢀⢀⢀⢀⢀⢀⢀⢀⢀⢀⢀⢀⢀⢀
⣀⣀⣀⣀⣀⣀⣀⣀⣀⣀⣀⣀⣀⣀
⣄⣄⣄⣄⣄⣄⣄⣄⣄⣄⣄⣄⣄⣄
⣤⣤⣤⣤⣤⣤⣤⣤⣤⣤⣤⣤⣤⣤
⣶⣶⣶⣶⣶⣶⣶⣶⣶⣶⣶⣶⣶⣶
⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿
```

## Mixing Braille with Other Marks

Braille forms can live alongside any other mark system:

```
Stars above braille mountains:
  ✦   ·    ✧        ·    ✦
     ·        ☽           ·    ✧
           ⣀⣀⣀⣀⣀
        ⣠⠞⠉⠀⠀⠀⠀⠉⠳⣄
     ⣠⠞⠁⠀⠀⠀⠀⠀⠀⠀⠀⠈⠳⣄
  ░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░

Braille curves with density blocks:
                    ⣿
                ⣿⣿⣿⣿⣿
  ░░░░░░░░░⣿⣿⣿⣿⣿⣿⣿⣿⣿
  ▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒
  ▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓

Braille as atmosphere around a word:
  ⠁    ⠂         ⠁
     ⠄      ⠁       ⠂
  ⠂      wonder      ⠄
     ⠁         ⠂
  ⠄      ⠂      ⠁
```

## Useful Braille Building Blocks

```
Corners and edges:
⣠  ⣄  top-left curve    top-right curve
⠳  ⠙  bottom-left       bottom-right
⡇  ⢸  left wall         right wall
⣀  ⠉  top edge          bottom edge
⣿     filled solid

Common curve pieces:
⣠⠞  rising left
⠳⣄  falling right  
⠙⣄  curving down-right
⣠⠋  curving up-left
⠈⠳⣄ gentle slope down
⣠⠞⠁ gentle slope up
```

## Things to Try

Draw a tree with a smooth trunk and rounded canopy. Draw an animal. Draw a heart with actual curves. Draw a building with arched windows. Draw someone's face. Draw a planet. Mix braille with every other mark system and see what happens.

The 256 patterns are a drawing system hiding inside text. Keep exploring what they can do.
