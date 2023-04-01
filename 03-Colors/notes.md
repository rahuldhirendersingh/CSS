# CSS Colors

## Color Names

- In this we just need to write the name of a color. Like:

1. red
2. green
3. pink
4. limegreen
5. aqua

## RGB Value

- In CSS, a color can be specified as an RGB value, using this formula:

> rgb(red, green, blue)

- Each parameter (red, green, and blue) defines the intensity of the color between 0 and 255.

- For example, rgb(255, 0, 0) is displayed as red, because red is set to its highest value (255) and the others are set to 0.

- To display black, set all color parameters to 0, like this: rgb(0, 0, 0).

- To display white, set all color parameters to 255, like this: rgb(255, 255, 255).

**Example**

```
rgb(255, 0, 0)

rgb(0, 0, 255)

rgb(60, 179, 113)

rgb(238, 130, 238)
```

> Shades of gray are often defined using equal values for all the 3 light sources:

**Example**

```
rgb(60, 60, 60)

rgb(90, 90, 90)
```

## RGBA Value

- RGBA color values are an extension of RGB color values with an alpha channel - which specifies the opacity for a color.

- An RGBA color value is specified with:

> rgba(red, green, blue, alpha)

- The alpha parameter is a number between 0.0 (fully transparent) and 1.0 (not transparent at all):

**Example**

```
rgba(255, 99, 71, 0.6)

rgba(255, 99, 71, 0.8)

rgba(255, 99, 71, 1)
```

## HEX Colors

- A hexadecimal color is specified with: #RRGGBB, where the RR (red), GG (green) and BB (blue) hexadecimal integers specify the components of the color.

### HEX Value

- In CSS, a color can be specified using a hexadecimal value in the form:

> #rrggbb

- Where rr (red), gg (green) and bb (blue) are hexadecimal values between 00 and ff (same as decimal 0-255).

- For example, #ff0000 is displayed as red, because red is set to its highest value (ff) and the others are set to the lowest value (00).

- To display black, set all values to 00, like this: #000000.

- To display white, set all values to ff, like this: #ffffff.

**Example**

```
#ff0000

#0000ff
```

> Shades of gray are often defined using equal values for all the 3 light sources:

**Example**

```
#3c3c3c

#616161
```

### 3 Digit HEX Value

- Sometimes you will see a 3-digit hex code in the CSS source.

- The 3-digit hex code is a shorthand for some 6-digit hex codes.

> #rgb

- Where r, g, and b represent the red, green, and blue components with values between 0 and f.

- The 3-digit hex code can only be used when both the values (RR, GG, and BB) are the same for each component. So, if we have #ff00cc, it can be written like this: #f0c.

**Example**

```
p {
  color: #b58; /* same as #bb5588 */
}
```

## HSL Colors

- HSL stands for hue, saturation, and lightness.

### HSL Value

- In CSS, a color can be specified using hue, saturation, and lightness (HSL) in the form:

> hsl(hue, saturation, lightness)

- Hue is a degree on the color wheel from 0 to 360. 0 is red, 120 is green, and 240 is blue.

- Saturation is a percentage value. 0% means a shade of gray, and 100% is the full color.

- Lightness is also a percentage. 0% is black, 50% is neither light or dark, 100% is white

_Example_

> hsl(147, 50%, 47%)

**Saturation**

- Saturation can be described as the intensity of a color.

- 100% is pure color, no shades of gray.

- 50% is 50% gray, but you can still see the color.

- 0% is completely gray; you can no longer see the color.

_Example_

> hsl(0, 100%, 50%)

**Lightness**

- The lightness of a color can be described as how much light you want to give the color, where 0% means no light (black), 50% means 50% light (neither dark nor light) and 100% means full lightness (white).

_Example_

> hsl(0, 100%, 0%)

### HSLA Value

- HSLA color values are an extension of HSL color values with an alpha channel - which specifies the opacity for a color.

- An HSLA color value is specified with:

- hsla(hue, saturation, lightness, alpha)

- The alpha parameter is a number between 0.0 (fully transparent) and 1.0 (not transparent at all):

_Example_

> hsla(0, 100%, 50%, 0.5)
