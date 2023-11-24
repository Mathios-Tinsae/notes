# CSS INTRO

CSS is the language we use to style an HTML document.

CSS describes how HTML elements should be displayed.

This tutorial will teach you CSS from basic to advanced.

**CSS Syntax**

![Untitled](CSS%20INTRO%20c80840d893e14ea88cbe0e3ea906e5dd/CSS%20intro%20e4865ddd35a047fc8c7bc8fa8c2d9e3b/Untitled.png)

The selector points to the HTML element you want to style.

The declaration block contains one or more declarations separated by semicolons.

Each declaration includes a CSS property name and a value, separated by a colon.

Multiple CSS declarations are separated with semicolons, and declaration blocks are surrounded by curly braces.

**CSS Selectors**

We can divide CSS selectors into five categories:

- Simple selectors (select elements based on name, id, class)
- [Combinator selectors](https://www.w3schools.com/css/css_combinators.asp) (select elements based on a specific relationship between them)
- [Pseudo-class selectors](https://www.w3schools.com/css/css_pseudo_classes.asp) (select elements based on a certain state)
- [Pseudo-elements selectors](https://www.w3schools.com/css/css_pseudo_elements.asp) (select and style a part of an element)
- [Attribute selectors](https://www.w3schools.com/css/css_attribute_selectors.asp) (select elements based on an attribute or attribute value)

**How To Add CSS**

# Three Ways to Insert CSS

There are three ways of inserting a style sheet:

- External CSS
- Internal CSS
- Inline CSS

**CSS Colors**

Colors are specified using predefined color names, or RGB, HEX, HSL, RGBA, HSLA values.

**CSS RGB Colors**

An RGB color value represents RED, GREEN, and BLUE light sources.

# RGB Value

In CSS, a color can be specified as an RGB value, using this formula:

**rgb(*red,* *green*, *blue*)**

Each parameter (red, green, and blue) defines the intensity of the color between 0 and 255.

For example, rgb(255, 0, 0) is displayed as red, because red is set to its highest value (255) and the others are set to 0.

# RGBA Value

RGBA color values are an extension of RGB color values with an alpha channel - which specifies the opacity for a color.

An RGBA color value is specified with:

**rgba(*red,* *green*, *blue, alpha*)**

The alpha parameter is a number between 0.0 (fully transparent) and 1.0 (not transparent at all)

**CSS HEX Colors**

A hexadecimal color is specified with: #RRGGBB, where the RR (red), GG (green) and BB (blue) hexadecimal integers specify the components of the color.

# HEX Value

In CSS, a color can be specified using a hexadecimal value in the form:

**#*rrggbb***

Where rr (red), gg (green) and bb (blue) are hexadecimal values between 00 and ff (same as decimal 0-255).

For example, #ff0000 is displayed as red, because red is set to its highest value (ff) and the others are set to the lowest value (00).

To display black, set all values to 00, like this: #000000.

To display white, set all values to ff, like this: #ffffff.

# 3 Digit HEX Value

Sometimes you will see a 3-digit hex code in the CSS source.

The 3-digit hex code is a shorthand for some 6-digit hex codes.

The 3-digit hex code has the following form:

**#*rgb***

Where r, g, and b represent the red, green, and blue components with values between 0 and f.

The 3-digit hex code can only be used when both the values (RR, GG, and BB) are the same for each component. So, if we have #ff00cc, it can be written like this: #f0c.

**CSS HSL Colors**

# HSL Value

In CSS, a color can be specified using hue, saturation, and lightness (HSL) in the form:

**hsl(*hue*, *saturation*, *lightness*)**

Hue is a degree on the color wheel from 0 to 360. 0 is red, 120 is green, and 240 is blue.

Saturation is a percentage value. 0% means a shade of gray, and 100% is the full color.

Lightness is also a percentage. 0% is black, 50% is neither light or dark, 100% is white

# Saturation

Saturation can be described as the intensity of a color.

100% is pure color, no shades of gray.

50% is 50% gray, but you can still see the color.

0% is completely gray; you can no longer see the color.

# Lightness

The lightness of a color can be described as how much light you want to give the color, where 0% means no light (black), 50% means 50% light (neither dark nor light) and 100% means full lightness (white).

# Shades of Gray

Shades of gray are often defined by setting the hue and saturation to 0, and adjust the lightness from 0% to 100% to get darker/lighter shades:

# HSLA Value

HSLA color values are an extension of HSL color values with an alpha channel - which specifies the opacity for a color.

An HSLA color value is specified with:

**hsla(*hue,* *saturation*, *lightness, alpha*)**

The alpha parameter is a number between 0.0 (fully transparent) and 1.0 (not transparent at all):

**CSS Backgrounds**

The CSS background properties are used to add background effects for elements.

# CSS background-image

The `background-image` property specifies an image to use as the background of an element.

By default, the image is repeated so it covers the entire element.

**CSS Background Image Repeat**

# CSS background-repeat

By default, the `background-image` property repeats an image both horizontally and vertically.

Some images should be repeated only horizontally or vertically, or they will look strange, like this:

```css
body {
  background-image: url("gradient_bg.png");
}
```

If the image above is repeated only horizontally (`background-repeat: repeat-x;`), the background will look better

```css
body {
  background-image: url("gradient_bg.png");
  background-repeat: repeat-x;
	}
```

**CSS background-repeat: no-repeat**

Showing the background image only once is also specified by the `background-repeat` property:

```css
body {
  background-image: url("img_tree.png");
  background-repeat: no-repeat;
}
```

# CSS background-position

The `background-position` property is used to specify the position of the background image.

```css
body {
  background-image: url("img_tree.png");
  background-repeat: no-repeat;
  background-position: right top;
}
```

# CSS background-attachment

The `background-attachment` property specifies whether the background image should scroll or be fixed (will not scroll with the rest of the page):

```css
body {
  background-image: url("img_tree.png");
  background-repeat: no-repeat;
  background-position: right top;
  background-attachment: fixed;
}
```

# CSS Outline

An outline is a line that is drawn around elements, OUTSIDE the borders, to make the element "stand out".

CSS has the following outline properties:

- `outline-style`
- `outline-color`
- `outline-width`
- `outline-offset`
- `outline`

# CSS Outline Style

The `outline-style` property specifies the style of the outline, and can have one of the following values:

- `dotted` - Defines a dotted outline
- `dashed` - Defines a dashed outline
- `solid` - Defines a solid outline
- `double` - Defines a double outline
- `groove` - Defines a 3D grooved outline
- `ridge` - Defines a 3D ridged outline
- `inset` - Defines a 3D inset outline
- `outset` - Defines a 3D outset outline
- `none` - Defines no outline
- `hidden` - Defines a hidden outline

```css
p.dotted {outline-style: dotted;}
p.dashed {outline-style: dashed;}
p.solid {outline-style: solid;}
p.double {outline-style: double;}
p.groove {outline-style: groove;}
p.ridge {outline-style: ridge;}
p.inset {outline-style: inset;}
p.outset {outline-style: outset;}
```

# Text Alignment and Text Direction

In this chapter you will learn about the following properties:

- `text-align`
- `text-align-last`
- `direction`
- `unicode-bidi`
- `vertical-align`

---

# Text Alignment

The `text-align` property is used to set the horizontal alignment of a text.

A text can be left or right aligned, centered, or justified.

The following example shows center aligned, and left and right aligned text (left alignment is default if text direction is left-to-right, and right alignment is default if text direction is right-to-left):

```css
h1 {
  text-align: center;
}

h2 {
  text-align: left;
}

h3 {
  text-align: right;
}
```

When the `text-align` property is set to "justify", each line is stretched so that every line has equal width, and the left and right margins are straight (like in magazines and newspapers):

```css
div {
  text-align: justify;
}
```

# Text Align Last

The `text-align-last` property specifies how to align the last line of a text.

```css
p.a {
  text-align-last: right;
}

p.b {
  text-align-last: center;
}

p.c {
  text-align-last: justify;
}
```

# Text Direction

The `direction` and `unicode-bidi` properties can be used to change the text direction of an element:

```css
p {
  direction: rtl;
  unicode-bidi: bidi-override;
}
```

# Vertical Alignment

The `vertical-align` property sets the vertical alignment of an element.

```css
img.a {  vertical-align: baseline;}
img.b {  vertical-align: text-top;}
img.c {  vertical-align: text-bottom;}
img.d {  vertical-align: sub;}
img.e {  vertical-align: super;}
```

# The CSS Text Alignment/Direction Properties

| Property | Description |
| --- | --- |
| https://www.w3schools.com/cssref/pr_text_direction.asp | Specifies the text direction/writing direction |
| https://www.w3schools.com/cssref/pr_text_text-align.asp | Specifies the horizontal alignment of text |
| https://www.w3schools.com/cssref/css3_pr_text-align-last.asp | Specifies how to align the last line of a text |
| https://www.w3schools.com/cssref/pr_text_unicode-bidi.asp | Used together with the https://www.w3schools.com/cssref/pr_text_direction.asp property to set or return whether the text should be overridden to support multiple languages in the same document |
| https://www.w3schools.com/cssref/pr_pos_vertical-align.asp | Sets the vertical alignment of an element |

# Grid Layout

The CSS Grid Layout Module offers a grid-based layout system, with rows and columns, making it easier to design web pages without having to use floats and positioning.

# Grid Elements

A grid layout consists of a parent element, with one or more child elements.

# Example

```html
<div class="grid-container">  <div class="grid-item">1</div>  <div class="grid-item">2</div>  <div class="grid-item">3</div>  <div class="grid-item">4</div>  <div class="grid-item">5</div>  <div class="grid-item">6</div>  <div class="grid-item">7</div>  <div class="grid-item">8</div>  <div class="grid-item">9</div></div>
```

# Display Property

An HTML element becomes a grid container when its `display` property is set to `grid` or `inline-grid`.

# Example

```css
.grid-container {  display: grid;}
```

# Example

```css
.grid-container {  display: inline-grid;}
```

# Grid Columns

The vertical lines of grid items are called *columns*.

![https://www.w3schools.com/css/grid_columns.png](https://www.w3schools.com/css/grid_columns.png)

---

# Grid Rows

The horizontal lines of grid items are called *rows*.

![https://www.w3schools.com/css/grid_rows.png](https://www.w3schools.com/css/grid_rows.png)

---

# Grid Gaps

The spaces between each column/row are called *gaps*.

![https://www.w3schools.com/css/grid_gaps.png](https://www.w3schools.com/css/grid_gaps.png)

You can adjust the gap size by using one of the following properties:

- `column-gap`
- `row-gap`
- `gap`

# Example

The `column-gap` property sets the gap between the columns:

```css
.grid-container {  display: grid;  **column-gap: 50px;**}
```

# Example

The `row-gap` property sets the gap between the rows:

```css
.grid-container {  display: grid;  **row-gap: 50px;**}
```

# Example

The `gap` property is a shorthand property for the `row-gap` and the `column-gap` properties:

```css
.grid-container {  display: grid;  **gap: 50px 100px;**}
```

# Example

The `gap` property can also be used to set both the row gap and the column gap in one value:

```css
.grid-container {  display: grid;  **gap: 50px;**}
```

# Grid Lines

The lines between columns are called *column lines*.

The lines between rows are called *row lines*.

![https://www.w3schools.com/css/grid_lines.png](https://www.w3schools.com/css/grid_lines.png)

Refer to line numbers when placing a grid item in a grid container:

# Example

Place a grid item at column line 1, and let it end on column line 3:

```css
.item1 {  ****grid-column-start: 1;  grid-column-end: 3;}
```

# Example

Place a grid item at row line 1, and let it end on row line 3:

```css
.item1 {  ****grid-row-start: 1;  grid-row-end: 3;}
```

# All CSS Grid Properties

| Property | Description |
| --- | --- |
| https://www.w3schools.com/cssref/css3_pr_column-gap.asp | Specifies the gap between the columns |
| https://www.w3schools.com/cssref/css3_pr_gap.asp | A shorthand property for the row-gap and the column-gap properties |
| https://www.w3schools.com/cssref/pr_grid.asp | A shorthand property for the grid-template-rows, grid-template-columns, grid-template-areas, grid-auto-rows, grid-auto-columns, and the grid-auto-flow properties |
| https://www.w3schools.com/cssref/pr_grid-area.asp | Either specifies a name for the grid item, or this property is a shorthand property for the grid-row-start, grid-column-start, grid-row-end, and grid-column-end properties |
| https://www.w3schools.com/cssref/pr_grid-auto-columns.asp | Specifies a default column size |
| https://www.w3schools.com/cssref/pr_grid-auto-flow.asp | Specifies how auto-placed items are inserted in the grid |
| https://www.w3schools.com/cssref/pr_grid-auto-rows.asp | Specifies a default row size |
| https://www.w3schools.com/cssref/pr_grid-column.asp | A shorthand property for the grid-column-start and the grid-column-end properties |
| https://www.w3schools.com/cssref/pr_grid-column-end.asp | Specifies where to end the grid item |
| https://www.w3schools.com/cssref/pr_grid-column-gap.asp | Specifies the size of the gap between columns |
| https://www.w3schools.com/cssref/pr_grid-column-start.asp | Specifies where to start the grid item |
| https://www.w3schools.com/cssref/pr_grid-gap.asp | A shorthand property for the grid-row-gap and grid-column-gap properties |
| https://www.w3schools.com/cssref/pr_grid-row.asp | A shorthand property for the grid-row-start and the grid-row-end properties |
| https://www.w3schools.com/cssref/pr_grid-row-end.asp | Specifies where to end the grid item |
| https://www.w3schools.com/cssref/pr_grid-row-gap.asp | Specifies the size of the gap between rows |
| https://www.w3schools.com/cssref/pr_grid-row-start.asp | Specifies where to start the grid item |
| https://www.w3schools.com/cssref/pr_grid-template.asp | A shorthand property for the grid-template-rows, grid-template-columns and grid-areas properties |
| https://www.w3schools.com/cssref/pr_grid-template-areas.asp | Specifies how to display columns and rows, using named grid items |
| https://www.w3schools.com/cssref/pr_grid-template-columns.asp | Specifies the size of the columns, and how many columns in a grid layout |
| https://www.w3schools.com/cssref/pr_grid-template-rows.asp | Specifies the size of the rows in a grid layout |
| https://www.w3schools.com/cssref/css3_pr_row-gap.asp | Specifies the gap between the grid rows |