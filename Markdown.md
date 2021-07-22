# 1. Title
> ### Two format 
> > Use = or -  

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
use <del>  <*del*> </*del*></del>  
use ~~two wavy lines~~  `~~two wavy lines~~`    

---  
# 3. List  
>### Unordered list  
`use * or + or - (notice space)`  
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
`Use number + . (notice space)`  
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
`Use >`  
#### Example:  
    >one
    >>two
    >>>three
#### Effects:  
>one
>>two
>>>three  
`Use lists in the block`  
#### Example:  
    >block1
    >1. one
    >2. two
#### Effects:  
>block1
>1. one
>2. two  
`Use blocks in the list(four spaces forward >)`
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
Use ` `
```
#### Example:  
```
Use `reboot` in terminal to reboot!
```
#### Effects:  
Use `reboot` in terminal to reboot!  
>### Code block  
1. Use four space or a Tab  
#### Example:  
```
    int main()
    {
        return 0;
    }
```
#### Effects:  
    int main()
    {
        return 0;
    }   
2. Use ` ``` `  
#### Example:  
    ```  
    int main()
    {
        return 0;
    }
    ```   
#### Effects:  
```
int main()
{
    return 0;
}
```  
---  
# 5. Links  
>### Name + link  
#### Example:  
```
[github](https://github.com/cloudres97)
```
#### Effects:  
[github](https://github.com/cloudres97)  
>### only link  
#### Example:  
```
<https://github.com/cloudres97>
```
#### Effects:  
<https://github.com/cloudres97>  
>### link at the end  
#### Example:  
```
My github name is [cloudres97][1]  
...  
[1]: https://github.com/cloudres97
```
#### Effects:  
My github name is [cloudres97][1]  
...  
[1]: https://github.com/cloudres97  
===   
# 6. Picture  
>### single picture(like links)  
#### Example:  
```
![My logo](https://avatars.githubusercontent.com/u/81032093?v=4 "可愛い猫")
```
#### Effects:  
![My logo](https://avatars.githubusercontent.com/u/81032093?v=4 "可愛い猫")  
>### give the picture a name  
#### Example:  
```
It's my github [logo][My logo]
...
[My logo](https://avatars.githubusercontent.com/u/81032093?v=4)
```
#### Effects:  
It's my github [logo][My logo]  
...  
[My logo](https://avatars.githubusercontent.com/u/81032093?v=4)  
>### change the size  
#### Example:  
```
<img src="https://avatars.githubusercontent.com/u/81032093?v=4" width="50%" height="50%">
```
#### Effects:  
<img src="https://avatars.githubusercontent.com/u/81032093?v=4" width="10%" height="10%">  

------  
# 7. Form  
>### Use `|`  
#### Example:  
```
|title|title|
|-|-|
|content1|content2|
|content3|content4|
```
#### Effects:  
|title|title|
|-|-|
|content1|content2|
|content3|content4|  
>### Alignment  
#### Example:  
```
|title|title|title|
|:-|-:|:-:|
|content1|content2|content3|
|content4|content5|content6|
```
#### Effects:  
|title|title|title|
|:-|-:|:-:|
|content1|content2|content3|
|content4|content5|content6|   
---  
# 8. Other tips  
>### HTML   
|`<kbd>`|`<b>`|`<i>`|`<em>`|`<sup>`|`<sub>`|`<br>`|
|-|-|-|-|-|-|-|

