# flex-grid
Flexbox grid system

## Usage
Include `grid.css` in your main CSS file or bring it straight into your `index.html`.

## Structure
The grid has columns that are wrapped in rows. By default, columns are all the same width and grow/shrink accordingly to fit the screen.

Add a class of `grid-row` to an element and put as many `grid-col` elements inside of that.

```html
<div class="grid-row">
  <div class="grid-col"></div>
  <div class="grid-col"></div>
  <div class="grid-col"></div>
</div>
```

For mobile-first grid layouts, add the class `grid-mobile` to the `grid-row`.

```html
<div class="grid-row grid-mobile">
  <div class="grid-col"></div>
  <div class="grid-col"></div>
  <div class="grid-col"></div>
</div>
```

For spacing between the columns, add the class `with-gutters` to the `grid-row`.

```html
<div class="grid-row with-gutters">
  <div class="grid-col"></div>
  <div class="grid-col"></div>
  <div class="grid-col"></div>
</div>
```

## Modifiers
Since we are using flexbox, we can add some modifiers for the columns and rows to do some easy alignment tweaks. When columns within a row are unequal heights, you can align them by adding the classes `row-top`, `row-middle`, or `row-bottom` to have all columns within the row align top/middle/bottom respectively.

```html
<div class="grid-row row-top">
  <div class="grid-col"></div>
  <div class="grid-col"></div>
  <div class="grid-col"></div>
</div>
```

If you want to align a single column within a row, you can add `col-top`, `col-middle`, or `col-bottom` to a `grid-col` and it will align itself at the top/middle/bottom of the row, regardless of where the columns within the row are aligned.

```html
<div class="grid-row">
  <div class="grid-col col-bottom"></div>
  <div class="grid-col col-top"></div>
  <div class="grid-col"></div>
</div>
```

There are also modifiers for fixed-width columns at intervals of thirds and fourths. For example, if you want a side nav menu as the first column in your grid and you want it to take up one fourth of the row and the next column to fill the remaining space, you could do something like this:

```html
<div class="grid-row row-top with-gutters">
  <div class="grid-col col-one-fourth"></div>
  <div class="grid-col"></div>
</div>
```

> In this example, you could add the class `col-three-fourths` to the second column, but if you leave it off it will grow to fill the remaining space.

## License
Copyright (c) 2015 Mike McBride

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
