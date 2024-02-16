# Class 3 CSS(continued)

## Table of contents:
1. Links
2. Combining CSS Selectors
3. CSS Positioning
4. CSS Display
5. Float
6. Media Queries
7.  Notes

## 1. Links
NONE


## 2. Combining CSS Selectors
You can combine different CSS selectors using certain operators, to apply your CSS rules more specifically and more generally.
### List of operators  
1. Comma operator ',': You can combine CSS selectors using a comma, which will apply your rules(attribute values) to all the css selectors. Example: h1, h2, p {color: green}, all h1,h2 and p tags will have the font color green. 
2. Child operator '\>': You can modify all tags that satisfy the 'parent \> child' relationship. Example: ul \> li{color: blue}, will change the font color of all li elements that are children of the ul elements to blue. 
3. Descendant operator ' '(denoted with a space between selectors), is the more general case of the child operator and specifies whether the lefthand selector is an ancestor of the righthand selector 'ancestor descendant'. Example: .box li{color: yellow} turns all li elements who have an ancestor with the .box class to the font color yellow. 
4. Chaining selectors works a bit different and does not use an explicit operator. Instead it places selectors adjacently with no spaces in between. If you are using an element selector it must be placed at the beginning of the chained selector. Chaining selectors are used to find very specific tags. Example: p.class1{color: orange}, chains the paragraph element selector with a class selector, to change the font to orange for all tags that have their element as p and have a class of "class1".
5. You are also allowed to combine all the above! Example: ul > p.obtained{font-size: 2rem} 

[Class Example](./combining_css_selectors/index.html)

## 3. CSS Positioning
* Static Positioning - Defaults to the next slot to put the item(can't be moved).
* Relative Positioning - Relative to default position.
* Absolute Positioning - Position relative to nearest positioned ancestor(parent) or top left corner of webpage
* Fixed Positioning - Position relative to top left corner of browser window(not webpage).

[Class Example](./css_positioning/index.html)

## 4. CSS Display
* inline: Used to place items on the same line(box is as small as possible)(p{display:inline;})
* block: Uses the box-model to place boxes vertically on webpage(Usually default)(p{display:block;})
* inline-block: Allows boxes to be placed on same line(p{display:inline-block;})

[Class Example](./css_display/index.html)

## 5. Float
Float is used to have text wrap around images as shown in [Example](./float/index.html)

## 6. Media Queries
Media queries is our first example of website responsiveness. It allows us to to modify our website based on its window size.
* @media (max-width: 400px){...} is the syntax that works for modifying the css code of a window size between 0-400px.
* @media (min-width: 300px){...} is the syntax that works for modifying the css code of a window size between 300px-max window size.
* @media (min-width: 300px) and (max-width: 500px){...} is the syntax that works for modifying the css code of a window size between 300px-500px.
* @media (max-width: 300px) and (min-width: 500px){...} is the syntax that works for modifying the css code of a window size between from 0px-300px and 500px-max window size.

See [Example](./media_queries/index.html)


## 7. Notes
* Next class flex, Grid, bootstrap, and javascript
* Play with box-model on chrome
* Homework: None
* Note that class="first second" is how you assign two classes to the same tag.