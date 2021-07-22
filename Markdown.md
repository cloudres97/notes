# 1. Title
> ### Two format 
> > Using = or -  

 #### Example:  
 ```
 This is the first level title!
 =
 This is the secondary title!
 -
 ```
 #### Effects:  
 This is the first level title!
 =
 This is the secondary title!
 -  

> Using #  

The number of "#" represents the level of the title(notice space)  
#### Example:  
```
# First level
## Second level   
...
###### Five level
```
#### Effects:  
# First level
## Second level   
...  
##### Five level  
---  
# 2. Paragraph and font
> ### Newline  
> > two spaces + enter  
> > empty line  

>### Font  
#### Example:
```
*Italics*    
_Italics_    
**Bold**    
__Bold__     
***Italics and bold***    
___Italics and bold___   
```
#### Effects:  
*Italics*    
_Italics_    
**Bold**    
__Bold__     
***Italics and bold***    
___Italics and bold___   
>### Separator  
*more than three * or - or _, without other symbols except space*  
#### Example:
```
**  *
- - -
_ _   _ 
```
#### Effects:  
**  *
- - -
_ _   _  
>### Delete line  
using <del>  <*del*> </*del*></del>  
using ~~two wavy lines~~  `~~two wavy lines~~`    

---  
# 3. List  
>### Unordered list  
`using * or + or - (notice space)`  
#### Example:  
```
* one
* two
* three

* one
+ two
+ three

- one
* two
+ three
```  
#### Effects:  
* one
* two
* three

* one
- two
+ three

- one
* two
+ three  
>### Ordered list  
`Using number + . (notice space)`  
#### Example:  
```
1. one
2. two
3. three
```  
#### Effects:  
1. one
2. two
3. three  
>### Nested list  
`Four spaces`
#### Example:
```
1. one
    + one
    - two
2. two
    1. one
    2. two
```  
#### Effects:  
1. one
    + one
    - two
2. two  
    1. one
    2. two  

---  
# 4. Block  
`Using >`  
#### Example:  
    >one
    >>two
    >>>three
#### Effects:  
>one
>>two
>>>three  
`Using lists in the block`  
#### Example:  
    >block1
    >1. one
    >2. two
#### Effects:  
>block1
>1. one
>2. two  
`Using blocks in the list(four spaces forward >)`
#### Example:  
```
1. one
    >one
    >>two
2. two
```
#### Effects:  
1. one
    >one
    >>two
2. two  
---  
# 5. Code  
>### In Sentence 
```
Using ` `
```
#### Example:  
```
Using `reboot` in terminal to reboot!
```
#### Effects:  
Using `reboot` in terminal to reboot!  
>### Code block
