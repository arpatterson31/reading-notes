# Class 14a Reading Notes - CSS Tranforms, Transitions, and Animation

## CSS Transforms Article

- CSS3 has new ways to size, position, and change elements
  - these new techniques can happen by the **transform** property

- **Transform** property comes in 2 settings: 2D and 3D

- Syntax
  - transform property followed by the value
  - value specifies the transform type followed by a specific amount inside parentheses



## CSS Transitions & Animations Article

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