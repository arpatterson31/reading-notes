# Class 8 Reading Notes - CSS Layout

## CSS Positioning

### Relative Positioning
  - shifts element to Top, Left, Right, or bottom of where it was originally placed

To write it in CSS:

`position: relative;`

then use the offset properties (top or bottom & left or right) to indicate how far to move the element from where it would have been in normal flow

`top: 10px;`

`left: 100px;`


### Absolute Positioning
  - positions the element in relation to its containing element
  - the box is taken out of normal flow and no longer affects the position of other elements on the page

To write it in CSS:

`position: absolute;`

then use the offset properties (top or bottom & left or right) to specify where the element should appear in relation to its containing element

`top: 0px;`

`left: 500px;`


### Fixed Positioning
  - positions the element in relation to the browser window

To write it in CSS:

`position: fixed;`

then use the offset properties (top or bottom & left or right) to control where the fixed position box appears in relation to the browser window

`top: 0px;`

`left: 0px;`


### z-index
- when using relative, fixed, or absolute positioning, boxes can overlap.. you can control which elements sit on top using the z-index property
- Its value is a number
- the higher the value, the closer that element is to the front

To write it in CSS:

`z-index: 15`


### Floating Elements
  - takes it out of its normal position and moves it to the far right or far left

To write it in CSS:

`float: right`

or

`float: left`

### Clearing Floats
- allows you to say that no element should touch the left or right-hand sides of a box

To write it in CSS:

`clear:left`  -- left hand side of box should not touch

`clear:right` -- right hand side of box should not touch

`clear:both` -- neither the left nor right

`clear:none` -- elements can touch either side



## Screen Size & Resolution

- Because screen sizes and resolution vary, web designers often try to create pages of around **960-1000 pixels** wide


## Page Layouts

- Fixed width layout - does not change size as the user increases or decreases the size of their browser window. (uses pixel)
  - advantages: pixel values are accurate, designer has far greater control over appearance and position
  - disadvantages: end up with gaps around the edge of a page, user resolution higher than designer's the page will look smaller

- Liquid Layout - stretch and contrast as user increases or descreases the size of their browser window (use percentages)
  - advantages: pages expand to fill the entire window on large screens and in a small screen, it can fit without having to scroll to the side
  - disadvantages: if width isn't controlled, pages can look very different than what was intended



## Layout Grids

- 960 pixel grid is widely used by web designers

