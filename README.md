# Simple Grid

Simple lightweight grid system. Provides a 2, 3, 4, 5, 6, 8, 9, and 12 column based grid system with full compliment of *spanning* columns at each grid size. This is a flexible (percentage based) grid system so columns will resize with the browser window, within any pre-set contraints of any wrapper elements.

Inspiration from [Chris Coyier's post on grids] (http://css-tricks.com/dont-overthink-it-grids/). Implementation jumpstarted by @ThisIsDallas (see: http://thisisdallas.github.com/Simple-Grid/).

## Usage

As with any grid system, you need to wrap your grid rows in a div class named <code>grid</code>. If you want a 20px padding around your grid, add the class <code>grid-pad</code> to the div wrapper. 

Choosing column sizes is through the use of the `col-x-y` classes where `x` is the number of columns to be spanned in a `y` based grid. For instance, to create a page with 2 sidebars placed left and right along with a 50% width central column, something like the following could be used:

```html
<div class="grid">
  <div class="col-1-4">
    <div class="content" />
  </div>
  <div class="col-2-4">
    <div class="content" />
  </div>
  <div class="col-1-4">
    <div class="content" />
  </div>
</div>
```

Columns by default are floated left to right. If you wish to pull a column out of order and push it to the right, use the `push-right` class.