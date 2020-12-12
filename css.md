# CSS learning notes

CSS adds style!

## CSS Rules
 - Contains 2 parts
   - selector or the element -- like h1, p, body
   - declaration - how it will be styled -- font, color, size
     - declarations are broken out into a property and a value
        - the property is the name of the style -- font, color, size

** Selectors - many kinds - can help to target specific elements to style

Example of how CSS looks:
``` p {```   
            ```color: red;}```    


### External CSS & Internal CSS
 - External is linked using ``` <link href="css/style.css" type="text/css" rel="stylesheet">```
    - Advantage: less code and smaller html pages, all pages can share the same stylesheet - preferred
 - Internal is using ``` <style> ``` html tag 
    - Advantage: everything is in one place, could work best when creating only page 
 


## Color!
Ways to specify color
- RGB Values -- red, green, blue - expressed as numbers between 0 and 255 : ``` rgb(123,123,123) ```
- HEX Codes -- red, green, blue - hexadecimal code : ``` #87cdae ```
- Color Name  
Contrast is key
CSS3 introduces opacity and hue, saturation, lightness values 



