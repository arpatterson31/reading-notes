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


### Floating Elements
  - takes it out of its normal position and moves it to the far right or far left