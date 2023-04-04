# CSS Box Model

- every html element is a box.

- the box contains:

> content + padding + border + margin

**total width of a element(box):**

- content width + padding right + padding left + border right + border left + margin right + margin left.

**total height of a element(box):**

- content height + padding top + padding bottom + border top + border bottom + margin top + margin bottom.

## Default CSS

- every box have some default css styles attached to it.

- like a h1 element have margin top & margin bottom set to 0.67em.

- if the font-size is 3rem.

- the margin top & margin bottom on h1 will be 32.160.

- How ?

**html default font-size is 16px**

> h1 font-size is 3rem

> 16 X 3 = 48px.

> 48 X 0.67 = 32.160 approx.

## Box Sizing

- The box-sizing property defines how the width and height of an element are calculated: should they include padding and borders, or not.

**content-box**

- Default. The width and height properties (and min/max properties) includes only the content. Border and padding are not included.

**border-box**

- The width and height properties (and min/max properties) includes content, padding and border.

**initial**

- Sets this property to its default value.

**inherit**

- Inherits this property from its parent element.
