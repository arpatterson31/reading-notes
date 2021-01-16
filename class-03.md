# Class 3 Read Notes - HTML Lists, Control Flow with JS, and the CSS Box Model

## Lists

Types of Lists

- Ordered Lists
  - each item in the list numbered
- Unordered Lists
  - bullet points rather than numbered 
- Definition Lists
  - made up of a set of terms and definitions for each terms


|**Tag** | **Name** | **Additional notes on use** |
|-------------------|-----------------------|---------------|
| `<ol>` | ordered lists | this creates the ordered list in HTML |
| `<ul>` | unordered list | this creates the unordered list in HTML |
| `<li>` | list item | creates list item in HTML - used for ordered and unordered |
| `<dl>` | definition list | creates the definition list in HTML |
| `<dt>` | definition term | used to contain the term being defined | 
| `<dd>` | definition | contains the definition in a definition list | 


## Boxes

HTML elements live in their own box per CSS

### Controlling Dimensions

- Height & Width
  - can be specified using pixels, percentages, and ems(based on the size of text)
  - min-width; max-width (specifies the smallest or largest the width of a box can be)
  - min-height; max-height

### **Border** - every box has one!

Style Elements for border

- border-width
- border-style
- border-color


### **Margin** - sits outside the edge of the border

- margin: auto: sets the box in the middle of the page

### **Padding** - space between the border of the box and content within it

### CSS3

- border-image
- box-shadow
- border-radius for rounded corners or elliptical shapes