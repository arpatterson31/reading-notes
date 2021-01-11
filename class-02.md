# Class 2 Read Notes - HTML Text, CSS Intro, and Basic JavaScript Instructions

## HTML Text

**Tags or markup provide meaning and provides structure to the page for browsers to read** 

### Structural Tags 
|**tag** | **name** | **additional notes on use** |
|-------------------|-----------------------|---------------|
|`<h1>` `<h2>` | headings | there are 6 levels of headings in HTML |
|`<p>`| paragraphs | creates a paragraph on the page |
|`<b>` | bold | characters appear bold between opening and closing tag |
|`<i>`| italic| characters appear italic between opening and closing tag |
|`<sup>`| superscript | superscripts characters like in suffixes of dates or math concepts - to a power| 
|`<sub>`| subscript| subscript characters used in footnotes or chemical formulas | 
|`<br />`| line break | can add a line break in middle of paragraph |
|`<hr />`| horizontal rule | can be used to add a break between themes |


### Semantic Tags - does not affect the structure but adds extra info to pages
|**tag** | **name** | **additional notes on use** |
|-------------------|-----------------------|---------------|
|`<strong>` | strong | indicates that content is strong importance |
|`<em>`| emphasis | indicates emphasis |
|`<blockquote>` | block quote | long quotes that take up a whole paragraph |
|`<q>`| quote | used for shorter quotes |
|`<abbr>`| abbreviations & acronyms | include title attribute to specify full term| 
|`<cite>`| citation | use when referencing a piece of work like a book or film | 
|`<dfn>`| definitions | explaining new terminology |
|`<address>`| author detail | contains contact info for author of the page |
|`<ins>`| insterted | content has been inserted into a document |
|`<del>`| deleted | content has been deleted from document |
|`<s>`| strike-out | content is no longer accurate or relevant but should not be deleted |


## CSS Intro

**CSS styles elements and tell the page how they should appear**

**CSS 

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

