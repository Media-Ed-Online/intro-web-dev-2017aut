---
title: Introduction to Color
module: 07
---

## Let's Add Some Color:
<img src="./../../../img/arrow-divider.svg" style="width: 75px; border: none;" />

Now that you are familiar with the basics or CSS, including how to apply rules, cascading, and selectors, lets start using it. The first major topic in CSS will focus on color. Specifically, how to specify colors for text and backgrounds.



### Specifying Color

There are two common ways of specifying color in CSS;

- RGB
- hex values

Both work in a practically the same way, by specifying the amount of red, green, and blue that should be combined to make a color.

Each color has a possible range of 256 values, 0-255. (Remember in a 0-based system, '0' counts as a value.)


#### RGB

In RGB, each of these three color values is represented as a decimal-based number, comma separated. These values are almost always wrapped in a  `rgb(rrr, ggg, bbb)`.


#### Hexadecimal

Hexadecimal (or hex) values, are written as a single string, prepended with a number sign, with digits for each color. `#RRGGBB`


**THE MAJOR DIFFERENCE** is that you can represent 256 values with a two-bit hexadecimal number. In hexadecimal numbering, each digit has 16 values (0-f). And, 16 * 16 = 256.

If we were translate this to binary:


<style>
table {
    width: 50%;
    margin: auto;
}
</style>

| Binary | Hex |
| :------: | :------: |
| 0 | 0 |
| 1 | 1 |
| 2 | 2 |
| 3 | 3 |
| 4 | 4 |
| 5 | 5 |
| 6 | 6 |
| 7 | 7 |
| 8 | 8 |
| 9 | 9 |
| 10 | a |
| 11 | b |
| 12 | c |
| 13 | d |
| 14 | e |
| 15 | f |

So, in hex, we write the value:

- `000` as `00`
- `010` as `0a`
- `015` as `0f`
- `016` as `10`
- `017` as `11`
- `031` as `1f`
- `032` as `20`
- `050` as `32`
- `100` as `64`
- `150` as `96`
- `200` as `c8`
- `250` as `fa`
- `255` as `ff`


### Red, Green, or Blue

So, to specify a color of full red in either system, we set the first number to 255, and the other two to 0.


- RGB: rgb(255, 0, 0);
- Hex: #ff0000;

<div width="50%" height="20px"
    style="background-color:rgb(255, 0, 0);padding:10px;">
</div>

Likewise, to specify a color of full green or full blue, use a value of 255 for the color in question, and 0 for the others.

- RGB: rgb(0, 255, 0);
- Hex: ##00ff00;

<div width="50%" height="20px"
    style="background-color:rgb(0, 255, 0);padding:10px;">
</div>

- RGB: rgb(0, 0, 255);
- Hex: ##0000ff;

<div width="50%" height="20px"
    style="background-color:rgb(0, 0, 255);padding:10px;">
</div>


### White & Black

We know from color theory, that white is the presence of all colors and black is the absence of all colors. Knowing this, we can deduce that black would be all 0's and white would be all full value.

**Black:**

- rgb(0, 0, 0);
- #000000;

<div width="50%" height="20px"
    style="background-color:rgb(0, 0, 0);padding:10px;">
</div>

**White:**

- rgb(255, 255, 255);
- #ffffff;

<div width="50%" height="20px"
    style="background-color:#ffffff;border-style:solid;border-width:1px;border-color:#000;padding:10px;">
</div>

Following from this principle, to get any color within the grey scale, we simply need to provide the same value for each color.

<div style="border-style:solid;border-width:1px;border-color:#000;text-align:center;">
<div width="50%" height="20px"
    style="background-color:#000000;color:#ffffff;padding:10px;">
    #000000 - rgb(0, 0, 0);
</div>
<div width="50%" height="20px"
    style="background-color:#101010;color:#f0f0f0;padding:10px;">
    #101010 - rgb(16, 16, 16);
</div>
<div width="50%" height="20px"
    style="background-color:#202020;color:#e0e0e0;padding:10px;">
    #202020 - rgb(32, 32, 32);
</div>
<div width="50%" height="20px"
    style="background-color:#303030;color:#d0d0d0;padding:10px;">
    #303030 - rgb(48, 48, 48);
</div>
<div width="50%" height="20px"
    style="background-color:#404040;color:#c0c0c0;padding:10px;">
    #404040 - rgb(64, 64, 64);
</div>
<div width="50%" height="20px"
    style="background-color:#505050;color:#b0b0b0;padding:10px;">
    #505050 - rgb(80, 80, 80);
</div>
<div width="50%" height="20px"
    style="background-color:#606060;color:#a0a0a0;padding:10px;">
    #606060 - rgb(96, 96, 96);
</div>
<div width="50%" height="20px"
    style="background-color:#707070;color:#909090;padding:10px;">
    #707070 - rgb(112, 112, 112);
</div>
<div width="50%" height="20px"
    style="background-color:#808080;color:#808080;padding:10px;">
    #808080 - rgb(128, 128, 128);
</div>
<div width="50%" height="20px"
    style="background-color:#909090;color:#707070;padding:10px;">
    #909090 - rgb(144, 144, 144);
</div>
<div width="50%" height="20px"
    style="background-color:#a0a0a0;color:#606060;padding:10px;">
    #a0a0a0 - rgb(160, 160, 160);
</div>
<div width="50%" height="20px"
    style="background-color:#b0b0b0;color:#505050;padding:10px;">
    #b0b0b0 - rgb(176, 176, 176);
</div>
<div width="50%" height="20px"
    style="background-color:#c0c0c0;color:#404040;padding:10px;">
    #c0c0c0 - rgb(192, 192, 192);
</div>
<div width="50%" height="20px"
    style="background-color:#d0d0d0;color:#303030;padding:10px;">
    #d0d0d0 - rgb(208, 208, 208);
</div>
<div width="50%" height="20px"
    style="background-color:#e0e0e0;color:#202020;padding:10px;">
    #e0e0e0 - rgb(224, 224, 224);
</div>
<div width="50%" height="20px"
    style="background-color:#f0f0f0;color:#101010;padding:10px;">
    #f0f0f0 - rgb(240, 240, 240);
</div>
<div width="50%" height="20px"
    style="background-color:#ffffff;color:#000000;padding:10px;">
    #ffffff - rgb(255, 255, 255);
</div>
</div>


### Complementary Colors

When we start to mix the ratios of red, green, and blue, we come up with the rest of the colors of the spectrum. Some of the first colors we should consider are the complementary colors of red, green, and blue. To get the complementary color for red, we use full green and blue. This creates Cyan.

**Cyan:**

- rgb(0, 255, 255);
- #00ffff;

<div width="50%" height="20px"
    style="background-color:#00ffff;color:#ff0000;padding:10px;font-size:1.5em;">
    Cyan compliments red.
</div>
<div width="50%" height="20px"
    style="background-color:#ff0000;color:#00ffff;padding:10px;font-size:1.5em;">
    Cyan compliments red.
</div>

Likewise, to get the complimentary colors for green and blue, which are magenta and yellow, respectively, we boost the values of the two other colors.

**Magenta:**

- rgb(255, 0, 255);
- #ff00ff;

<div width="50%" height="20px"
    style="background-color:#ff00ff;color:#00ff00;padding:10px;font-size:1.5em;">
    Magenta compliments green.
</div>
<div width="50%" height="20px"
    style="background-color:#00ff00;color:#ff00ff;padding:10px;font-size:1.5em;">
    Magenta compliments green.
</div>

**Yellow:**

- rgb(255, 255, 00);
- #ffff00;

<div width="50%" height="20px"
    style="background-color:#ffff00;color:#0000ff;padding:10px;font-size:1.5em;">
    Yellow compliments Blue.
</div>
<div width="50%" height="20px"
    style="background-color:#0000ff;color:#ffff00;padding:10px;font-size:1.5em;">
    Yellow compliments Blue.
</div>


### Other Colors

Others colors are obviously some combination of these values. The exact ratios depend on the amounts of red, green, and blue in every value.

For more information on RGB colors, please read the corresponding [Wikipedia article](https://en.wikipedia.org/wiki/RGB_color_model).


## Atom Tips:

If you are using atom, there are two packages you may want to consider installing.

1. _[color-picker](https://atom.io/packages/color-picker)_ - The atom color picker lets you inspect colors, as any value type (rgb, hex, hsl, etc.), and navigate a color "picker" so that you can insert any color value. Once, installed, you can pull up this package with the "atom command palette" by typing color.
![Atom Color Picker Demo](https://i.github-camo.com/467c72e686f00893c3d36bf46499e76c10f31787/68747470733a2f2f6769746875622e636f6d2f74686f6d61736c696e647374726f6d2f636f6c6f722d7069636b65722f7261772f6d61737465722f707265766965772e676966 "atom color picker demo")

2. _[pigments](https://atom.io/packages/pigments)_ - The atom pigments package highlights color values in your code. This can make it easier to visually see in atom, while developing the colors that will appear.
![Atom Pigments Package Demo](https://i.github-camo.com/802d8b759d01e70861f95f99495731f19b145b03/687474703a2f2f61626533332e6769746875622e696f2f61746f6d2d7069676d656e74732f7069676d656e74732e6769663f7261773d74727565 "Atom Pigments Package Demo")


#### Going Further

For more information on hexadecimal numbering, visit:
- [Hex Number System](http://homepage.smc.edu/morgan_david/cs40/hex-system.htm)
- [Math is Fun: Hexadecimal Numbers](https://www.mathsisfun.com/hexadecimals.html)
- [Decimal to Hex Converter](http://www.binaryhexconverter.com/decimal-to-hex-converter)


# { TODO: }
1. Read the ["7 Step Guide to Understanding Color Theory"](https://99designs.com/blog/tips/the-7-step-guide-to-understanding-color-theory/).
2. Read pages 246-249 of Chapter 11 in [Duckett](https://github.com/Media-Ed-Online/intro-web-dev/issues/3).
