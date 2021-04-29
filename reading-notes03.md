# Readings-notes03

# Html-notes
![dsvfvsds](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTkYS7oc8ae0GC8zHwuF35oJJIWOFxTH2LfGw&usqp=CAU.jpg)

## Other content

`<address>` 

*The `<address>` element has quite a specific use: to contain contact details for the author of the page.It can contain a physical address, but it does not have to. For example, it may also contain a phone number or email address*



`<s>`

*The `<s>` element indicates something that is no longer accurate or relevant (but that should not be deleted).Visually the content of an `<s>`element will usually be displayed with a line through the center*

`<ins>`
`<del>`

*The `<ins>` element can be used to show content that has been inserted into a document, while the `<del>` element can show text that has been deleted from it.The content of a `<ins>` element is usually underlined, while the content of a `<del>` element usually has a line through it*


1.  HTML elements are used to describe the structure of 
the page (e.g. headings, subheadings, paragraphs).

2.  They also provide semantic information (e.g. where 
emphasis should be placed, the definition of any 
acronyms used, when given text is a quotation).


## LISTS

### How many list types in HTML:
1. unordered list — used to group a set of related items in no particular order.
2. ordered list — used to group a set of related items in a specific order.
3. description list — used to display name/value pairs such as terms and definitions

### Ordered list
`<ol>`
>The ordered list is created with the `<ol>` element.

`<li>`
>Each item in the list is placed between an opening <li> tag and a closing </li> tag
(The listands for list item.)


### Unordered list
`<ul>`
> The unordered list is created with the `<ul>` element.

`<li>`
>Each item in the list is placed between an opening `<li>` tag and a closing `</li>` tag
(The listands for list item.)



--------------------------------------------------------------------------

### Summary
* There are properties to control the choice of font, size, 
weight, style, and spacing.
* There is a limited choice of fonts that you can assume 
most people will have installed.
* If you want to use a wider range of typefaces there are 
several options, but you need to have the right license 
to use them.
* You can control the space between lines of text, 
individual letters, and words. Text can also be aligned 
to the left, right, center, or justified. It can also be 
indented.
* You can use pseudo-classes to change the style of an 
element when a user hovers over or clicks on text, or 
when they have visited a link.


----------------------------------------------------------------------------------



## BOXES
### How do you insert a box in HTML?
>Using CSS to Draw a Border Around Your Block of Text and Pictures

No|StePs
-|-
1|Create the HTML for the block. For this tutorial, I shall use a DIV block to enclose the text/pictures. `<div class="boxed">` ...
2|Next, you will need to style the DIV box by adding a border. In your CSS section, or external CSS file, add the following code:


### How do you make a box in HTML?
> Using CSS to Draw a Border Around Your Block of Text and Pictures
1. Create the HTML for the block. For this tutorial, I shall use a DIV block to enclose the text/pictures. `<div class="boxed">` ...
2. Next, you will need to style the DIV box by adding a border. In your CSS section, orexternal CSS file.

1. Create the HTML for the block. For this tutorial, I shall use a DIV block to enclose the text/pictures.

`<div class="boxed">`
  >This text is enclosed in a box.
`</div>`



##### I gave the DIV block a class of "boxed" but you can of course use some other valid CSS class name. Replace my dummy content with your actual text and/or images.

2. you will need to style the DIV box by adding a border. In your CSS section, or external CSS file, add the following code:

`.boxed {`
  `border: 1px solid green ;`
`}`


`width, height`

*The most popular ways to specify the size of a box are to use pixels, percentages, or ems. Traditionally, pixels have been the most popular method because they allow designers to accurately control their size.*

*When you use percentages, the size of the box is relative to the size of the browser window or, if the box is encased within another box, it is a percentage of  the size of the containing box.*

`min-width, max-width`

*home page designs expand and shrink to fit the size of the user'sscreen. In such designs, the min-width property specifies the smallest size a box can be displayed at when the browser window is narrow, and the max-width property indicates the maximum width a box can stretch to when the browser window is wide.*

`min-height, max-height`

*In the same way that you might want to limit the width of a box on a page, you may also want to limit the height of it. This is achieved using the min-heightand max-height properties.The example on this page demonstrates these properties in action. It also shows you what happens when the content of the box takes up more space than the size specified for the box*

## White space & Vertical Margin
>like this
###### Designers refer to the space between items on a page as 
###### white space. Imagine you had 
###### a border around a box. You 
###### would not want the text to touch 
###### this border or it would become harder to read.

###### Or, imagine you had two boxes 
###### sitting side by side (each with 
###### a black border). You would not 
###### necessarily want the boxes to 
###### touch edges as this would make 
###### the line look twice as thick on 
###### the facing sides.


## Border Width

##### The border-width property is used to control the width of a border. The value of this property can either be given in pixels or using one of the following values:
`thin`
`medium`
`thick`
##### (You cannot use percentages with this property.)
>You can control the individual size of borders using four separate properties:

`border-top-width`
`border-right-width`
`border-bottom-width`
`border-left-width`

>You can also specify different widths for the four border values in one property, like so:border-width: `2px 1px 1px 2px;`

*The values here appear in clockwise order: top, right, bottom, left.*

## Border Style

##### You can control the style of a border using the border-style property. 


>This property can take the following values:solid a single solid line dotted a series of square dots (if your border is 2px wide, then the dots are 2px squared with a 2px gap between each dot)


##### dashed a series of short lines double two solid lines (the value of the border-width property creates the sum of the two lines) groove appears to be carved into the pageridge appears to stick out from the page inset appears embedded into the pageoutset looks like it is coming out of the screen hidden / none no border is shown

>You can individually change the styles of different borders using:
`border-top-style`
`border-left-style`
`border-right-style`
`border-bottom-style`


## Short hand border
 ![vfsds](https://s3.amazonaws.com/webucator-how-tos/2366.png)
>The border property allows you to specify the width, style and color of a border in one property (and the values should be coded in that specific order)



## IE6 Box Model
![DSFSFS](https://crypt.codemancers.com/images/boxmodel/BoxModelDefault.f05f124a77b1950f2e16ff518613155149e83d9b97cb6fb99831b829d85406ed.png)

*When you specify the width of a box, any padding or margin should be added to the width of it. Internet Explorer 6, however, has a quirk whereby it includes the padding and margins in the width of the box.*

*The way around this is to ensure that you provide a `DOCTYPE` declaration for the HTML page. You can use either the `HTML5`, `HTML` `4 strict`, or HTML 4 transitional `DOCTYPE` declarations to ensure that IE6 follows the correct box model.*

## Change Inline/Block

>The display property allows you to turn an inline element into a block-level element or vice versa, and can also be used to hide an element from the page.The values this property can take are:

* inline
*This causes a block-level element to act like an inline element.*

* block
*This causes an inline element to act like a block-level element.*

* inline-block
*This causes a block-level element to flow like an inline element, while retaining other features of a block-level element.*

## CSS3: Rounded Corners

*CSS3 introduces the ability to create rounded corners on any box, using a property called border-radius. The value indicates the size of the radius in pixels.*

*Older browsers that do not support this property will show a box with right-angled corners.*

*The -moz-border-radius and -webkit-border-radius properties are not in the CSS specification. However, they are used in some versions of Chrome, Firefox, and Safari to offer early support for this styl (and therefore can be used to achieve this effect in more browsers).*

>You can specify individual values 
>for each corner of a box using:

`border-top-right-radius`
`border-bottom-right-radius`
`border-bottom-left-radius`
`border-top-left-radius`

*You can also use a shorthand of these four properties (in clockwise order: top, right, 
bottom, left). For example:border-radius:* `5px, 10px, 5px, 10px;`



----------------------------------------------------------------------------------------

# JS OVERVIWE
![XVXDVX](https://www.vitoshacademy.com/wp-content/uploads/2015/04/JS.png)

## USING QUOTES INSIDE A STRING

>Sometimes you will want to use a double or single quote mark within a string. 

*Because strings can live in single or double quotes, if you just want to use double quotes in the string, you could surround the entire string in single quotes.*

*If you just want to use single quotes in the string, you could surround the string in double quotes (as shown in the third line of this code example).* 

*You can also use a technique called escaping the quotation characters. This is done by using a backwards slash (or `"backslash"`) before any type of uote mark that appears within a string (as shown on the fourth line of this code sample). The backwards slash tells the interpreter that the following character is part of the string, rather than the end of it.* 

## USING A VARIABLE TO STORE A BOOLEAN

*A Boolean variable can only have a value of true or fa 1 se, but this data type is very helpful. In the example on the right, the values true or fa 1 se are used in the cl ass attributes of HTML elements.* 

*These values trigger different CSS class rules: true shows a check, fa 1 se shows a cross. (You learn how the class attribute is set in Chapter 5.) *

*It is rare that you would want to write the words true or false into the page for the user to read, but this data type does have two very popular uses:* 

* First, Booleans are used when the value can only be true/ `fa` `1` `se`.

* You could also think of these values as `on/off` or `0/1:` true is equivalent to on or `1`, `fa` 1 `se` is equivalent to `off` or `0`* 

## CREATING VARIABLES 

>Programmers sometimes use shorthand to create variables. Here are three variations of how to declare variables and assign them values: 

1. Variables are declared and 
values assigned in the same 
statement. 

2. Three variables are declared 
on the same line, then values 
assigned to each. 

3. Two variables are declared 
and assigned values on the same 
line. Then one is declared and 
assigned a value on the next line. 
(The third example shows two 
numbers, but you can declare 
variables that hold different 
types of data on the same line, 
e.g., a string and a number.) 

4. Here, a variable is used to 
hold a reference to an element in 
the HTML page. This allows you 
to work directly with the element 
stored in that variable.

## CHANGING THE VALUE OF A VARIABLE

>Once you have assigned a value to a variable, you can then change what is stored in the variable later in the same script. Once the variable has been created, you do not need to use the var keyword to assign it a new value. You just use the variable name, the equals sign (also known as the assignment operator), and the new value for that attribute. 

>For example, the value of a shipping variable might start out as being false.* 

*Then something in the code might change the ability to ship the item and you could therefore change the value to true. In this code example, the values of the two variables are both swapped from being true to false and vice versa.* 


## LOOPS
![SCSASSA](https://data-flair.training/blogs/wp-content/uploads/sites/2/2019/08/Difference-between-for-and-while-loop.jpg)

![DVSDVSDVSD](https://miro.medium.com/max/1024/0*L0CgDXGMGpXL53Ud.png)

## IF STATMENT
![DSFSDFSFDE](https://www.guru99.com/images/JavaScript/javascript5_1.png)
![DSSDSSSSSA](https://image.slidesharecdn.com/javascriptconditionalstatements-140806034702-phpapp02/95/javascript-conditional-statements-1-638.jpg?cb=1407296892.JPG)


