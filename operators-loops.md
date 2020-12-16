# Operators

## Comparison
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
|`>=`| greater than or equal to | |
|`<=`| less than or equal to| |


## Logical Operators
- allows you to compare results of more than one comparison operator

``` && ``` - logical and 
``` || ``` - logical or
``` ! ``` - logical not - single boolean value and inverts it



# Loops
Check conditions 

If true - code will run and continue in a loop until false returned

### Types of loops
-For - used if you need it to run for a specific number of times

- create variable then set it to 0
- set condition or how many times you need it to run;  i < 10
- update - i++ adds one to the counter every time loop runs


- While - if you don't know how many times it needs to run
    - while (i < 10) -- will run as long as the condition in the parentheses is true