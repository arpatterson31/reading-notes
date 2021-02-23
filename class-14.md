# Class 14a Reading Notes - CSS Tranforms, Transitions, and Animation

## CSS Transforms Article

- CSS3 has new ways to size, position, and change elements
  - these new techniques can happen by the **transform** property

- **Transform** property comes in 2 settings: 2D and 3D

- Syntax
  - transform property followed by the value
  - value specifies the transform type followed by a specific amount inside parentheses

- Examples:

- 2D Rotate - rotate an element from 0 to 360 degrees
  - `transform: rotate(20deg)`

- 2D Scale - change the appeared size of element
  - default scale value is 1
  - `scaleX` will scale the width
  - `scaleY` will scale the height
  - `transform: scale(1.25)`

- 2D Translate - pushes and pulls element in different directions without interrupting the normal flow 
  - `transform: translate(-10px, 25%)`
  - `translateX` will change position on the horizontal axis
  - `translateY` will change position on the vertical axis

- 2D Skew - distorts on the horizontal, vertical axis or both
  - `transform: skewX(5deg)`

- 3D uses perspective and the z axis

## CSS Transitions & Animations Article

### Transitions

- allow you to alter the apperance/behavior or an element when it is hovered over, focused on, active, or targeted

- Transition uses pseudo-classes
  - `:hover`
  - `:focus`
  - `:active`
  - `:target`

- There are 4 transition related properties
  - `transition-property`
  - `transition-duration`
  - `transition-timing-function`
  - `transition-delay`

### Animations

- Animations help pick up where transitions leave off 

- Animation Properties
  - `animation-name:`
  - `animation-duration:`
  - `animation-timing-function:`
  - `animation-delay:`
  - `animation-iteration-count:`
  - `animation-direction:`
  - `animation-play-state:`
  - `animation-fill-mode:`
  
  
## 8 Simple CSS3 transitions that will wow your users Article

- Fade In - emphasizes functionality or draws attention
  - first set the intial state then the change like hover

````css
.fade
{
        opacity:0.5;
}
.fade:hover
{
        opacity:1;
}
````

- Change Color
  - animating a change of color

```` css
.color:hover
{
        background:#53a7ea;
}
````

- Grow
  - to grow, use it's width and height or its padding:

```` css
.grow:hover
{
        -webkit-transform: scale(1.3);
        -ms-transform: scale(1.3);
        transform: scale(1.3);
}
````

- Shrink
  - shrinking is the same except we specify a value less than 1

```` css
.shrink:hover
{
        -webkit-transform: scale(0.8);
        -ms-transform: scale(0.8);
        transform: scale(0.8);
}
````

- Rotate element

```` css 
.rotate:hover
{
        -webkit-transform: rotateZ(-30deg);
        -ms-transform: rotateZ(-30deg);
        transform: rotateZ(-30deg);
}
````

- Square to circle

```` css
.circle:hover
{
        border-radius:50%;
}
````

- 3D Shadow

```` css
.threed:hover
{
        box-shadow:
                1px 1px #53a7ea,
                2px 2px #53a7ea,
                3px 3px #53a7ea;
        -webkit-transform: translateX(-3px);
        transform: translateX(-3px);
}
````

- Swing

````css
.swing:hover
{
        -webkit-animation: swing 1s ease;
        animation: swing 1s ease;
        -webkit-animation-iteration-count: 1;
        animation-iteration-count: 1;
}
````

- Inset border

````css 
.border:hover
{
        box-shadow: inset 0 0 0 25px #53a7ea;
}
````

# Class 14b Reading Notes - What Google Learned About Teams