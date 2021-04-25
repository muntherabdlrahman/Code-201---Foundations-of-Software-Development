# HTML
![SFSFSD](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRfRxCKiS7qkVILEENB6IVCsNH742LMh9buUuZV4REd3iWswQFisYgquJ0qUR8-ped0R2k&usqp=CAU.JPG)
### How the web works?
*When you visit a website,the web server hosting that site could be anywhere in the world. In order for you to find the location of the web server, your browser will first connect to a Domain Name System (DNS) server.*
*The unique number that the  DNS server returns to your computer allows your browser to contact the web server  that hosts the website you  requested. A web server is a  computer that is constantly  connected to the web, and is set  up especially to send web pages to users.*

--------------------------------------------------
### 1: HTML
***HTML Describes the Structure of Pages***
*The rest of this section introduces the tags you have  at your disposal to create web pages, grouped into chapters on: text,lists, links, images,tables,  forms,video audio and flash, and miscellaneous elements*

*should warn that the examples in the first nine chapters are not exciting to look at, yet they are the foundation of every web page. The following chapters on CSS will show you how to make your pages look a lot more interesting.*


### 2: CSS
*Presentation: How to control things like the color of text, the fonts you want to use and the size of those fonts, how to add background colors to pages (or parts of a page), and how to add background images.*

*Layout: How to control where the different elements are positioned on the screen. You will also learn several techniques that professionals use to make  their pages more attractive.*


### 3: Practical
*We end up with some helpful information that will assist you in building better websites*
*Finally, we end up looking at topics that will help you once you have built your site, such as putting it on the web search  engine optimisation (SEO) and using analytics software to track who comes to your site and what 
they are looking at*

#### How Websites are Created?
*All websites use HTML and CSS, but content  management systems, blogging software, and  e-commerce platforms often add a few more technologies into the mix.*

##### 1: What you see
*When you are looking at a  website, it is most likely that  your browser will be receiving  HTML and CSS from the web  server that hosts the site. The  web browser interprets the  HTML and CSS code to create the page that you see. 
Some sites also send JavaScript  or Flash to your browser, and you  will see how to add JavaScript  and Flash in your web pages. Both of these technologies are advanced topics that you can go  on to learn more about once you have mastered HTML and CSS, if you want*


##### 2:How it is Created
*Small websites are often written just using HTML and CSS. Larger websites — in particular  those that are updated regularly  and use a content management  system (CMS), blogging tools.
Or  e-commerce software — often  make use of more complex  technologies on the web server,  but these technologies are  actually used to produce HTML  and CSS that is then sent to the  browser. So, if your site uses  these technologies, you will be  able to use your new HTML and  CSS knowledge to take more  control over how your site looks.*




##### 3:TML5 & CSS3
*Since the web was first created  there have been several versions  of HTML and CSS — each  intended to be an improvement  on the previous version.  At the time of writing this  book, HTML5 & CSS3 were  still being developed. Although  they had not been finalized,  many browsers were already  supporting some features of  these languages and a lot of  people were using the latest  code on their websites. I have  therefore chosen to teach you these latest versions.*




### HTML main continent
#### `<body>`
*You met the <body> element 
in the first example we created. 
Everything inside this element is 
shown inside the main browser 
window.*

#### `<head>`
*Before the <body> element you 
will often see a <head> element. 
This contains information 
about the page (rather than 
information that is shown within 
the main part of the browser 
window that is highlighted in 
blue on the opposite page). 
You will usually find a <title>
element inside the <head>
element.*

#### `<title>`
*The contents of the <title>
element are either shown in the 
top of the browser, above where 
you usually type in the URL of 
the page you want to visit, or 
on the tab for that page (if your 
browser uses tabs to allow you 
to view multiple pages at the 
same time*

`<form>`
*Element uses the action attribute to indicate the page that 
the data is being sent to. Each of the form controls sits inside the <form> element.
 Different types of form control are suited to collecting different types of data. 
The <fieldset> element is used to group related questions together. The <label> element indicates the purpose of each form control.*

----------------------------------------------------
## The Evolution of HTML
>Each new version was designed  to be an improvement on the last (with new elements and  attributes added and older code  removed). 
There have also been several  versions of each browser used to view web pages, each of which implements new code. Not all  web users, however, have the  latest browsers installed on  their computers, which means that not everyone will be able to  view all of the latest features and markup.

#### HTML 4
*With the exception of a few  elements added in HTML5 
(which have been highlighted),  the elements you have seen in  this book were all available in .
Although HTML 4 had some presentational elements to  control the appearance of pages,  authors are not recommended to  use them any more. (Examples include the <center> element  for centering content on a page, <font> for controlling  the appearance of text, and  <strike> to put a line through  the text — all of these can be achieved with CSS instead.)* 



#### XHTML 1.0

*In 1998, a language called XML  was published. Its purpose  was to allow people to write  new markup languages. Since  HTML was the most widely used  markup language around, it was  decided that HTML 4 should be reformulated to follow the rules  of XML and it was renamed  XHTML. This meant that  authors had to follow some new,  more strict rules about writing markup. For example:*


* Every element needed a closing tag (except for empty elements such as <img />).
* Attribute names had to be in lowercase.
* All attributes required a value, and all values were to be placed in double quotes.
* Deprecated elements should no longer be used.
* Every element that was opened inside another element should be closed inside that same element. 

#### HTML5
*web page authors do not need to close all tags, and new elements and attributes will be introduced. 
At the time of writing, the HTML5 specification had not been completed, but the major browser makers had started to implement many of the new features, and web page authors were rapidly adopting the new markup.Despite the fact that HTML5 is not yet completed, you can safely take advantage of the new features of the language as long as you endeavour to ensure that users with older browsers will be able to view your pages (even though some of the extra features will not be visible to them)*

#### some of contents of Html5 codes
`<!-- -->`
*If you want to add a comment 
to your code that will not be 
visible in the user's browser, you 
can add the text between these 
characters:*
`<!-- comment goes here -->`




`<div>`
*The <div> element allows you to 
group a set of elements together 
in one block-level box.*

`<span>`
*The <span> element acts like 
an inline equivalent of the <div>
element. It is used to either*

-|contains
-|-
1|Contain a section of text where there is no other suitable element to differentiate it from its surrounding text
2|Contain a number of inline elements


`<iframe>` 
*An iframe is like a little window 
that has been cut into your 
page — and in that window you 
can see another page. The term 
iframe is an abbreviation of inline 
frame*


`src`
*The src attribute specifies the 
URL of the page to show in the 
frame.*
`height`
*The height attribute specifies 
the height of the iframe in pixels.*
`width`
*The width attribute specifies 
the width of the iframe in pixels.*


`crolling`

*The scrolling attribute will 
not be supported in HTML5. In 
HTML 4 and XHTML, it indicates 
whether the iframe should 
have scrollbars or not. This is 
important if the page inside the 
iframe is larger than the space 
you have allowed for it (using the 
height and width attributes). 

`Scrollbars`

*allow the user to move 
around the frame to see more 
content. It can take one of three 
values: yes (to show scrollbars), 
no (to hide scrollbars) and auto
(to show them only if needed).*

`frameborder`

*The frameborder attribute will 
not be supported in HTML5. In 
HTML 4 and XHTML, it indicates 
whether the frame should have 
a border or not. A value of 0
indicates that no border should 
be shown. A value of 1 indicates 
that a border should be shown.*

`seamless`

*In HTML5, a new attribute 
called seamless can be applied 
to an iframe where scrollbars 
are not desired. The seamless
attribute (like some other new 
HTML5 attributes) does not 
need a value, but you will often 
see authors give it a value of 
seamless. Older browsers 
do not support the seamless
attribute.*

`<meta>`
*The <meta> element lives 
inside the <head> element and 
contains information about that 
web page*

-------------------------------
## Traditional HTML Layouts
![SFSF](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSA5CahAwdOWNlETTPhdwfijpYmO2jLVDj3RQ&usqp=CAU.JPG)

>For a long time, web page authors used <div> elements to group together related elements on the page (such as the elements that form a header, an article, footer or sidebar). Authors used class or id attributes to indicate the role of the <div> element in the structure of the page.

1.  `<header>` and `<footer>`

elements can be used for:
* The main header or footer 
that appears at the top or 
bottom of every page on the 
site.
* A header or footer for an 
individual <article> or 
<section> within the page.

2. `<nav>`

*element is used to  contain the major navigational 
blocks on the site such as the primary site navigation. Going back to our blog example, 
if you wanted to finish an article 
with links to related blog posts, 
these would not be counted as major navigational blocks and therefore should not sit inside a <nav> element.* 

`<article>`

*element acts as a container for any section of a page that could stand alone and potentially be syndicated*


`<aside>`

*element has two 
purposes, depending on whether 
it is inside an <article>
element or not.*

`<section>`

*element groups 
related content together, and 
typically each section would 
have its own heading.*

`<hgroup>`

*element is to group together a 
set of one or more <h1> through 
<h6> elements so that they are 
treated as one single heading.*

`<figure>`

*element in Chapter 5 when we 
looked at images. It can be used 
to contain any content that is 
referenced from the main flow of 
an article (not just images).*


~~~~~~
Older browsers that do not know the new HTML5 elements will automatically treat them as inline elements. Therefore, to help older browsers, you should include the line of CSS on the left which states which new elements should be rendered as block-level elements.Also, IE9 was the first version of Internet Explorer to allow CSS rules to be associated with these new HTML5 layout elements. In order to style these elements using earlier versions of IE, you need to use a simple JavaScript known as the HTML5 shiv or  HTML5 shim. 
~~~~~~~~~


### Summary
>The new HTML5 elements indicate the purpose of 
different parts of a web page and help to describe 
its structure.
* The new elements provide clearer code (compared 
with using multiple <div> elements).
* Older browsers that do not understand HTML5 
elements need to be told which elements are 
block-level elements.
* To make HTML5 elements work in Internet Explorer 8 
(and older versions of IE), extra JavaScript is needed, 
which is available free from Google.


-------------------------------------

## Why People Visit YOUR Website?
![HFTH](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSTDDBb5yTpG_RSH-4PC9Pp_g_5OJ7CK8Tr7Q&usqp=CAU.JPG)
>Your content and design should 
be influenced by the goals of 
your users. 
To help determine why people 
are coming to your website, 
there are two basic categories of 
questions you can ask:

***1: The first attempts to discover 
the underlying motivations for 
why visitors come to the site.***

***2: The second examines the 
specific goals of the visitors. 
These are the triggers making 
them come to the site now.***


so

#### Key Motivations
* Are they looking for general 
entertainment or do they 
need to achieve a specific 
goal? 
* If there is a specific goal, is 
it a personal or professional 
one?
* Do they see spending time on 
this activity as essential or a 
luxury?..

#### pecific Goals
* Do they want general 
information / research (such 
as background on a topic / 
company), or are they after 
something specific (such as a 
particular fact or information 
on a product)?
* Are they already familiar with 
the service or product that 
you offer or do they need to 
be introduced to it?
* Are they looking for time 
sensitive information, such as 
the latest news or updates on 
a particular topic?



#### Key Information
* Will visitors be familiar with 
your subject area / brand 
or do you need to introduce 
yourself?
* Will they be familiar with 
the product / service / 
information you are covering 
or do they need background 
information on it?
* What are the most important 
features of what you are 
offering?
* What is special about what 
you offer that differentiates 
you from other sites that offer 
something similar?
* Once people have achieved 
the goal that sent them to 
your site, are there common 
questions people ask about 
this subject area?


#### Goods / Services
* How often do the same 
people return to purchase 
from you?
* How often is your stock 
updated or your service 
changed?
Information
* How often is the subject 
updated?
* What percentage of your 
visitors would return for 
regular updates on the 
subject, compared with 
those who will just need the 
information once?...

### Example Site Map
![HH](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRDKnEvd8DbxW-XI6lY1XsMAlHax6ywAD7KhrBFgmeeXFZytEVPhAUB9igFHNSv8p1-qcE&usqp=CAU.JPG)


>At the end I hope this page be helpful for you guys and for any kind of assistance please ask me to provide more information that should be so helpful as i can sheerd with you my personal notes written on by my hands on real perpor.

<<<<<<< HEAD
Thank you 
=======

>>>>>>> d808ae8aa1e8aaa14aef82f37d0beec139c72bbd
