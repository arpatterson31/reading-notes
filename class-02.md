# Class 2 Read Notes - HTML Text, CSS Intro, and Basic JavaScript Instructions

## HTML Text

**Tags or markup provide meaning and provides structure to the page for browsers to read** 

### Structural Tags 

|**Tag** | **Name** | **Additional notes on use** |
|-------------------|-----------------------|---------------|
| `<h1>` `<h2>` | headings | there are 6 levels of headings in HTML |
| `<p>` | paragraphs | creates a paragraph on the page |
| `<b>` | bold | characters appear bold between opening and closing tag |
| `<i>` | italic| characters appear italic between opening and closing tag |
| `<sup>` | superscript | superscripts characters like in suffixes of dates or math concepts - to a power| 
| `<sub>` | subscript| subscript characters used in footnotes or chemical formulas | 
| `<br />` | line break | can add a line break in middle of paragraph |
| `<hr />` | horizontal rule | can be used to add a break between themes |


### Semantic Tags - does not affect the structure but adds extra info to pages

|**Tag** | **Name** | **Additional notes on use** |
|-------------------|-----------------------|---------------|
| `<strong>` | strong | indicates that content is strong importance |
| `<em>` | emphasis | indicates emphasis |
| `<blockquote>` | block quote | long quotes that take up a whole paragraph |
| `<q>` | quote | used for shorter quotes |
| `<abbr>` | abbreviations & acronyms | include title attribute to specify full term| 
| `<cite>` | citation | use when referencing a piece of work like a book or film | 
| `<dfn>` | definitions | explaining new terminology |
| `<address>` | author detail | contains contact info for author of the page |
| `<ins>` | insterted | content has been inserted into a document |
| `<del>` | deleted | content has been deleted from document |
| `<s>` | strike-out | content is no longer accurate or relevant but should not be deleted |


## CSS Intro

**CSS styles elements and tell the page how they should appear**

- Contains 2 parts
   - selector or the element -- like h1, p, body
   - declaration - how it will be styled -- font, color, size
     - declarations are broken out into a property and a value
        - the property is the name of the style -- font, color, size

Example of how CSS looks:
``` h1 {```   
            ```color: red;}```    

### External CSS & Internal CSS
 - External is linked using ``` <link href="css/style.css" type="text/css" rel="stylesheet">```
    - Advantage: less code and smaller html pages, all pages can share the same stylesheet - preferred
 - Internal is using ``` <style> ``` html tag 
    - Advantage: everything is in one place, could work best when creating only page 


**Selectors - many kinds - can help to target specific elements to style**

|**Selector** | **Meaning** | **How to write it** |
|-------------------|-----------------------|---------------|
| Universal | applies to all elements | `* {}` |
| Type | matches element names | `p {}` `h1, h2, h3 {}` |
| Class | matches to a class attribute | `.className {}` |
| ID | matches to an ID attribute | `#IDName {}` |


## Basic JavaScript Instructions

|**Vocab Term** | **Definition** | **Additional Info** |
|-------------------|-----------------------|---------------|
| statement | individual step in the script | Always end with a `;` |
| comment | use comments to explain your code | single line comment use: `//` multi-line use: `/* comment */` |
| Variables | stored information from the statement | declare a variable by using ` var variableName` |
| Array | special type of variable - stores a list of values | declare by using var then name of array |
| Expressions | results in single value | expressions can just assign a value to a variable  or use 2 or more values to return single value |
| Operators | helps create a single value from one or more | see detailed operator explaination below |


### Arrays
- Values assigned in an array are enclosed in square brackets `[]`
- Values in an array are also given an number called an index - index values start at 0


### Operators
- Assignment Operators - assign value to variable using ` = `
- Arithmetic Operators - preform basic math 
- String Operators - combine 2 or more strings using ` + `
- Comparison Operators - compare 2 values to return true or false
- Logical operators - combine expresions and return true or false 

## Decisions and loops

### Comparison
- comparing value to what you expect to be true
- Result will be boolean: true or false


|**operator** | **meaning** | **examples** 
|-------------------|-----------------------|---------------|
|`==` | is equal to | 'black' == 'white' - false; 'black' == 'black' - true|
|`!=`| is not equal to | 'black' != 'white' - true; 'black' != 'black' - false |
|`===` | strict equal to | 'two' === 2 - false; 2 === 2 - true |
|`!==`| strict not equal to| 'two' !== 2 - true; 2 !== 2 - false |
|`>`| greater than | 5 > 2 - true; 2 > 5 - false| 
|`<`| less than|  5 < 2 - false; 2 < 5 - true| 
|`>=`| greater than or equal to | 5 >= 2 - true; 5 >= 5 - true; 2 >= 5 - false|
|`<=`| less than or equal to| 5 <= 2 - false; 5 <= 2 - false; 2 <= 5 - true|

### Logical Operators
- allows you to compare results of more than one comparison operator

``` && ``` - logical and 
``` || ``` - logical or
``` ! ``` - logical not - single boolean value and inverts it