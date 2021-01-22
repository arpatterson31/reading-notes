# Class 5 Reading Notes - HTML Images; CSS Color & Text

## Images

Images can either make your site look average or really engaging so choosing the right ones are key!


Images should:
- be relevant
- convey information
- convey the right mood
- be instantly recognizable
- fit the color palette

**All images are subject to copyright so don't steal other people's work!**

Adding an image:
- use `<img>` tag - no need for closing tag
- `src` tells the browser where the file is located
- `alt` provides a text description
- `title` provides additional information about the image
- `width` & `height` can be added to size images in pixels

example:

`<img src="images/image.jpg" alt="This is a picture"/>`


HTML5: Figure and Figure Caption

- `<figure>` element to contain images and their caption
- `<figcaption>` allows a caption to be tied to an image


### Rules for creating images

- Save images in the right format
- Save images at the right size
- Measure images in pixels


Types of images:
- JPEG - use when you have many different colors in a picture
- GIF or PNG - use when you have images with few colors or large areas of the same color


## CSS Color

Ways to specify color
- RGB Values -- red, green, blue - expressed as numbers between 0 and 255 : `rgb(123,123,123)`
- HEX Codes -- red, green, blue - hexadecimal code : `#87cdae`
- Color Name 


Hue - a color or shade
Saturation - the amount of gray in the color - max would be no gray
Brightness - how much black is in the color - max would be no black


## CSS Text 

TYPEFACE TERMINOLOGY
- SERIF - extra details on the end of the letters
- SANS-SERIF - no details on the end of the letters
- MONOSPACE - every letter is the same width
- WEIGHT - adds emphasis and affects the amount of whitespace
- STYLE - normal, italic
- STRETCH


Specifying typeface
- font-family
- font-size
- font-weight
- font-style
- text-decoration
  - none
  - underline
  - overline
  - line-through
  - blink
- text-align
  - left
  - right
  - center
  - justify
