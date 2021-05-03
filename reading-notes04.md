# Reading-notes04

## Html
![fhf](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRxWPA0bLvRLyIEVJRem3iJ3Ik5yv9YUyeo9A&usqp=CAU.jpg)

### Unordered Lists
>An unordered list is a collection of related items that have no special order or sequence. This list is created by using HTML <ul> tag. Each item in the list is marked with a bulle.

`<ul>`
*The unordered list is created with the `<ul>` element.*

`<li>`
*Each item in the list is placed between an opening `<li>` tag and a closing `</li>` tag. (The `li` stands for list item.)*


### Definition Lists

`<dl>`
*The definition list is created with the `<dl>` element and usually consists of a series of terms and their definitions.*

*Inside the `<dl>` element you will usually see pairs of `<dt>` and  `<dd>` elements.*

`<dt>`
*This is used to contain the term being defined (the definition term).*

`<dd>`
*This is used to contain the  definition.*


### NESTED LISTS 68
*You can put a second list inside an `<li>` element to create a sublist or nested list.*

### Links

#### How to do links in html:
no|steps
-|-
1|Use the `<a>` element to define a link.
2|Use the href attribute to define the link address.
3|Use the target attribute to define where to open the linked document.
4|Use the `<img>` element (inside `<a>` ) to use an image as a link.

![vdvv](https://www.wikihow.com/images/6/6c/Add-a-Hyperlink-with-HTML-Step-6-Version-2.jpg)

## Directory Structure
### tructure
*The diagram on the right shows the directory structure for a fictional entertainment listings website called ExampleArts. The top-level folder is known as the root folder. (In this example, the root folder is called examplearts.) The root folder contains all of the other files and folders for a website. Each section of the site is placed in a separate folder; this helps organize the files.*

### Relationships
*The relationship between files and folders on a website is described using the same terminology as a family tree. In the diagram on the right, you can see some relationships have been drawn in.*

### Homepages
*The main homepage of a site written in HTML (and the homepages of each section in a child folder) is called index.html.Web servers are usually set up to return the index.html file if no file name is specified. Therefore, if you enter examplearts.com it will return examplearts.com/index.html, and examplearts.com/music will return examplearts.com/music/index.html.*

![dvdg](https://i.stack.imgur.com/qTP6u.png)


### Email Links

`mailto:`
*To create a link that starts up the user's email program and addresses an email to a specified email address, you use the `<a>`element. However, this time the value of the href attribute starts with `mailto:` and is followed by the email address you want the email to be sent to.*


### pening Links ina New Window
### How to open a link in a new window or new tab?
no|steps
-|-
1|Open a link in a new window or tab. In order to open a link in a new window / tab, add target="_blank" inside the <a> tag: ...
2|New window or new tab. You can't set whether the link will be opened in a new window or new tab. ...
3|Open a link in a new window with specified size.

`target`

*If you want a link to open in a new window, you can use the target attribute on the opening `<a>` tag. The value of this attribute should be `_blank`.One of the most common reasons a web page author might want a link to be opened in a new window is if it points to another website.*




----------------------------------------------------------------------------------------
## Layout
![dsfsg](https://media.geeksforgeeks.org/wp-content/uploads/layout.png)


### What is layout of HTML?
>HTML layouts provide a way to arrange web pages in well-mannered, well-structured, and in responsive form or we can say that HTML layout specifies a way in which the web pages can be arranged. Web-page layout works with arrangement of visual elements of an HTML .

### What is Building Blocks
>CSS treats each HTML element as if it is in its own box. This box will either be a block-level box or an inline box.


### lock-level elements
#### start on a new line
###### Examples include:`<h1>` `<p>` `<ul>` `<li>`

### Inline elements
#### flow in between surrounding text
###### Examples include:`<img>` `<b>` `<i>`



### Controlling the Position of Elements



*Lorem Ipsum CSS has the following positioning schemes that allow you to control the layout of a page: normal flow, relative positioning, and absolute positioning. You specify the positioning scheme using the position property in CSS. You can also float elements using the float property.*

### Normal flow
*Every block-level element appears on a new line, causing each item to appear lower down the page than the previous one. Even if you specify the width of the boxes and there is space for two elements to sit side-byside, they will not appear next to each other. This is the default behavior (unless you tell the browser to do something else).*

### Relative Positioning
*This moves an element from the position it would be in normal flow, shifting it to the top, right, bottom, or left of where it would have been placed. This does not affect the position of surrounding elements; they stay in the position they would be in in normal flow.*

Absolute positioning
*This positions the element in relation to its containing element. It is taken out of normal flow, meaning that it does not affect the position of any surrounding elements (as they simply ignore the space it would have taken up). Absolutely positioned elements move as users scroll up and down the page.*

## Normal Flow
## position:static
>In normal flow, each block-level element sits on top of the next one. Since this is the default way in which browsers treat HTML elements, you do not need a CSS property to indicate that elements should appear in normal flow, but the syntax would be:

### position: static; 
*I have not specified a width property for the heading element, so you can see how it stretches the width of the entire browser window by default.*


>The paragraphs are restricted to 450 pixels wide. This shows how the elements in normal flow start on a new line even if they do not take up the full width of the browser window

## Relative Positioning
## position:relative
*Relative positioning moves an element in relation to where it would have been in normal flow.For example, you can move it 10 pixels lower than it would have been in normal flow or 20% to the right.*
*You can indicate that an element should be relatively positioned using the position property with a value of relative.*



>When the position property is given a value of absolute, the box is taken out of normal flow and no longer affects the position of other elements on the page. (They act like it is not there.) The box offset properties (top or bottom and left or right) specify where the element should appear in relation to its containing element.

Fixed Positioning
position:fixed
>Fixed positioning is a type of absolute positioning that requires the position property to have a value of fixed.

*The `<p>` elements are in normal flow and ignore the space that the `<h1>` element would have taken up. Therefore, the margin-top property has been used to push the first `<p>`element below where the fixed position `<h1>` element is sitting.*


## Clearing Floats
`clear`

>The clear property allows you to say that no element (within the same containing element) should touch the left or righthand sides of a box. It can take the following values:

`left`
*The left-hand side of the box should not touch any other elements appearing in the same containing element.*

`right`
*The right-hand side of the box will not touch elements appearing in the same containing element.*

`both`
*Neither the left nor right-hand sides of the box will touch elements appearing in the same containing element.*

`none`
*Elements can touch either side.the fourth paragraph has a class called clear. The CSS rule for this class uses the clear property to indicate that nothing should touch the left-hand side of it. The fourth paragraph is therefore moved further down the page so no other element touches its left-hand side.*



## A Liquid Layout
![ggggg](https://cloud.netlifyusercontent.com/assets/344dbf88-fdf9-42bb-adb4-46f01eedd629/6bfc16df-3bb6-42b2-9076-7a8f4daef4d2/fluid.jpg)

>fluid layout is a type of webpage design in which layout of the page resizes as the window size is changed. This is accomplished by defining areas of the page using percentages instead of fixed pixel widths , The CSS classes in the examples could each be assigned to a div within a page's HTML where the 




## Layout Grids

![ggggd](https://miro.medium.com/max/1024/1*XCZZZmhQN4rHLw2dW14BZQ.png)


>while a grid might seem like a restriction, in actual fact it:

* Creates a continuity between 
different pages which may 
use different designs
* Helps users predict where to 
find information on various 
pages
* Makes it easier to add new 
content to the site in a 
consistent way
* Helps people collaborate 
on the design of a site in a 
consistent way

## Layout Using 960.
![ffdfsf](https://images4.arabicprogrammer.com/807/c0/c054867a6b3342605d809a965991b037.JPEG)

>The `960_12_col.css` stylesheet contains all of the rules we need to control the grid layout. The HTML uses the class names:`container_12` to act as a container for the whole page and indicate that we are using a 12 column grid



##### The `960.gs` style sheet 
>has taken care of the layout, creating the correct width for the columns and setting the spaces between them. Therefore, the only rules we needed to add are shown on this page. These rules:
* Control the font and the 
position of the text in the 
boxes
* Set the background colors for 
the boxes
* Set the height of the feature 
and article boxes
* Add a margin to the top and 
bottom of each bo

## Multiple Style Sheets
## @import

Some web page authors split 
*up their CSS style rules into separate style sheets. For example, they might use one style sheet to control the layout and another to control fonts, colors and so on.*

>Some authors take an even more modular approach to stylesheets, creating separate stylesheets to control typography, layout, forms, tables, even different styles for each sub-section of a site.There are two ways to add :

>multiple style sheets to a page:
1. Your HTML page can link to one style sheet and that stylesheet can use the @import rule to import other style sheets.
2. In the HTML you can use a separate <link> element for each style sheet*



## Multiple Style Sheets
## link
*the contents of site.css are identical to styles.css on the left hand page, except the code does not contain @import rules.As with all style sheets, if two rules apply to the same element then rules that appear later in a document will take precedence over previous rules.* 


--------------------------------------------------------------------------------

#JS
![DDDSFS](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQmf0qiGBPZPrbc9jfghWdJCmis3Gx1Q1P6Qw&usqp=CAU.JPG)

* A script is made up of a series of statements. Each 
 statement is like a step in a recipe. 

* Scripts contain very precise instructions. For example, 

* you might specify that a value must be remembered 
before creating a calculation using that value. 

* Variables are used to temporarily store pieces of 
information used in the script. 

* Arrays are special types of variables that store more 
than one piece of related information. 


* JavaScript distinguishes between numbers (0-9), 

* strings (text), and Boolean values (true or false). 

* Expressions evaluate into a single value. 

* Expressions rely on operators to calculate a value. 


* A script is made up of a series of statements. Each 
statement is like a step in a recipe. 

* Scripts contain very precise instructions. For example, 
you might specify that a value must be remembered 
before creating a calculation using that value. 

* Variables are used to temporarily store pieces of 
information used in the script. 

* Arrays are special types of variables that store more 
than one piece of related information. 

* JavaScript distinguishes between numbers (0-9), 
strings (text), and Boolean values (true or false). 

* Expressions evaluate into a single value. 

* Expressions rely on operators to calculate a value. 

-------------------------------------------------------------------------------------

## FUNCTIONS
### WHAT IS A FUNCTION? 
>Functions let you group a series of statements together to perform a 
specific task. If different parts of a script repeat the same task, you can 
reuse the function (rather than repeating the same set of statements). 

## DECLARING FUNCTIONS
![VDVDVSD](https://s3-ap-southeast-1.amazonaws.com/djamblog/article-040420082711.png)

## EXPLANITION FUNCTION
![DVSVS](https://www.fatalerrors.org/images/blog/cbbaf0ee49c4b43577c3a4f0e4f5fb68.jpg)




* Scripts contain very precise instructions. For example, 
you might specify that a value must be remembered 
before creating a calculation using that value. 

* Variables are used to temporarily store pieces of 
information used in the script. 

* Arrays are special types of variables that store more 
than one piece of related information. 

* JavaScript distinguishes between numbers (0-9), 
strings (text), and Boolean values (true or false). 

* Expressions evaluate into a single value. 

* Expressions rely on operators to calculate a value
