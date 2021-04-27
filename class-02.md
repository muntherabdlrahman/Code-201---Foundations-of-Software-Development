# Readings notes of class-02
## HTML summiries
![sum](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSK05JKrfhOFjMdS5DQLKu1GAxxCdfLZ2Ky6pZgaDsgywwMOLF6_R4EVdoiSUTsoX01VMk&usqp=CAU.jpg)

## Code in a Content Management System
![dffs](https://code-websites.com/wp-content/uploads/2016/09/Content-Management-System-1030x736.jpg)

*content management system (CMS) is a computer software used to manage the creation and modification of digital content.
ECM typically supports multiple users in a collaborative environment by integrating document management, digital asset management, and record retention*

#####  Acontent management system, blogging platform, or e-commerce application, you will probably log into a special administration section of the website to control it. The tools provided in the administration sections of these sites usually allow you to edit parts of the page rather than the entire page, which means you will rarely see the `<html>`, `<head>`, or <body> elements.

##  How other sites are Built
*Each page will have its own text, images and other elements. All web pages and elements are then placed in a folder and stored on your web host server. Each web page is written in codes and these codes describe the layout, format and content on the page. The most common coding language used to create web pages is HTML. *


##### How do websites work?
*Before you begin creating your own website and launch it to the Internet, it’s important to know how websites work.
Here are some basic terms:* 

*A website is simply a collection of web pages of codes – codes that describes the layout, format and content on a page. 
The web server is a internet-connected computer that receives the request for a web page sent by your browser.
The browser connects your computer to the server through an IP address. The IP address is obtained by translating the domain name. (Don’t worry, this part is all done automatically by your browser so you don’t have to look up the IP addresses yourself.)
In other words, in order to display your website on the Internet, you will need:*

-|-
-|-
1|A website
2|A domain name
3|A server
###### INFORMATION IS FROM
[Domain Email and Website Hosting Articles](https://www.doteasy.com/domain-email-and-website-hosting-articles/how-do-websites-work)

>Once you have opened this page, you can look for the View menu in your browser, and select the option that says Source or View source. (The title changes depending on what browser you are using.

## Text
*HTML has six "levels" of headings:`<h1>` is used for main headings `<h2>` is used for subheadings If there are further sections under the subheadings then the `<h3>` element is used, and so on...*

## Bold & Italic
###### <b>
*By enclosing words in the tags `<b>` and `</b>` we can make characters appear bold.The <b> element also represents a section of text that would be presented in a visually different way (for example key words in a paragraph) although the use of the <b> element does not imply any additional meaning.*
###### <i>
*By enclosing words in the tags `<i>` and `</i>` we can make* 
*characters appear italic.*
*The `<i>` element also represents a section of text that would be said in a different way from surrounding content — such as technical terms, names of ships, foreign words, thoughts, or other terms that would usually be italicized*

## Superscript & Subscript
###### `<sup>`
*The `<sup>` element is used to contain characters that should be superscript such as the suffixes of dates or mathematical concepts like raising a number to a power such as 22*

###### `<sub>`
*The `<sub>` element is used to contain characters that should be subscript. It is commonly used with foot notes or chemical formulas such as H20.*


## Line Breaks & Horizontal Rules
###### `<br />`
*As you have already seen, the browser will automatically show each new paragraph or heading on a new line. But if you wanted to add a line break inside the middle of a paragraph you can use the line break tag <br />*

###### `<hr />`
*To create a break between themes — such as a change of topic in a book or a new scene in a play — you can add a horizontal rule between sections using the <hr /> tag.*


## Visual Editors & Their Code views
![hhj] (https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRb6ji6XCLJGe9GlBuXe5KWKvkraxA7rQa-mQ&usqp=CAU.jpg)

> isual editors often resemble word processors. Although each editor will differ slightly, there are some features that are common to most editors that allow you to control the presentation of text.

* Headings are created by highlighting text then using a drop-down box to select a heading.
* Bold and italic text are created by highlighting some text and pressing a b or ibutton.
* New paragraphs are created using the return or the enter key.
* Line breaks are created by pressing the shift key and the return key at the same time.
* Horizontal rules are created using a button with a straight line on it.

## Strong & Emphasis
![fsffs](https://www.dummies.com/wp-content/uploads/412474.image0.jpg)
###### <strong>
*The use of the `<strong>`element indicates that its content has strong importance. For example, the words contained in this element might be said with strong emphasis.By default, browsers will show the contents of a <strong> element in bold.*

###### `<em>`
*The <em> element indicates emphasis that subtly changes the meaning of a sentence.By default browsers will show the contents of an `<em>` element in italic*

-------------------------------------------------------------------------------------------------------------------------------------------------

## : Adding HTML5 Audio to Your Pages


>How to Embed Audio Files in an HTML5 Document:
-|-
-|-
1|Create an HTML5 document in Dreamweaver or your favorite HTML editor.
2|Switch to your HTML editor's Code view.
3|Position your cursor in the body of the document. That would be anywhere after the tag.
4|Enter the following code: ...
5|Save the document and test it in each browser used by your target audience.

###### `<audio>`
*HTML5 introduced the `<audio>` element to include audio files in your pages. As with HTML5 video, browsers expect different formats for the audio.*

*The `<audio>` element has a number of attributes which allow you to control audio playback: src This attribute specifies the path to the audio file* 

###### controls.
*This attribute indicates whether the player should display controls. If you do not use this attribute, no controls will be shown by default. You can also specify your own controls using JavaScrip*


###### autoplay
*The presence of this attribute indicates that the audio should start playing automatically. (It is considered better practice to let visitors choose to play audio.) HTML5: Adding HTML5 Audio to Your Pages*

##### preload
*This attribute indicates what the browser should do if the player is not set to autoplay. It can have the same values  for the `<video>` element.*

###### loop
*This attribute specifies that the audio track should play again once it has finished.*

---------------------------------------------------------------------------------------------------------------------------------------------------

## CSS
![dfsdfd](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRFAJ1dCa79KVB_qn9L2JVflatBSJuO6hTkp2vXEOu6-HxtELwoG8rU4GGu3FmLo-Cq2Rc&usqp=CAU.jpg)

###### What is CSS?
*Cascading Style Sheets (CSS) is a language for specifying the style and appearance of web pages. For example, CSS is used to specify:*

1. Fonts
2. Colors
3. Arrangement of elements on the page
*The key to understanding how CSS works is to imagine that there is an invisible box around every HTML element (Figure 2.1). CSS allows us to create rules that control the way that each individual box, and the contents of that box, is presented. CSS is run when it is linked to HTML code, while that HTML code is processed and visually presented by the browser*

## Using External CSS
![fsfsf](https://slideplayer.com/slide/9224209/27/images/5/External+CSS+External+styles+are+defined+in+an+external+CSS+file%2C+and+then+linked+to+in+the+%3Chead%3E+section+of+an+HTML+page%3A.jpg)

>How do I use an external CSS file?
-|-
-|-
1|How to Create a CSS External Style Sheet
2|Start with an HTML file that contains an embedded style sheet, such as this one. ...
3|Create a new file and save it as StyleSheet. ...
4|Move all the CSS rules from the HTML file to the StyleSheet. ...
5|Remove the style block from the HTML file.
6|In the HTML file, add a link tag after the closing title tag that points to StyleSheet.
 ###### information is from
 [dummies](https://www.dummies.com/web-design-development/html5-and-css3/how-to-use-an-external-style-sheet-for-html5-and-css3-programming/)

###### <link> 

*The `<link>` element can be used in an HTML document to tell the browser where to find the CSS file used to style the page. It is an empty element (meaning it does not need a closing tag), and it lives inside the `<head>` element.* 

>It should use three attributes:

###### `<href>`
*This specifies the path to the CSS file (which is often placed in a folder called css or styles). type This attribute specifies the type of document being linked to. The value should be text/css.*

###### `<rel>`
*This specifies the relationship between the HTML page and the file it is linked to. The value should be stylesheet when linking to a CSS file.*



###### `<style>`
*You can also include CSS rules within an HTML page by placing them inside a `<style>` element, which usually sits inside the `<head>` element of the page. The `<style>` `element` should `use` the type attribute to indicate that the styles are specified in CSS. The value should be text/css.When building a site with more than one page,* 

>you should use 
>an external CSS style sheet. This:
* Allows all pages to use the same style rules (rather than repeating them in each page).
* Keeps the content separate from how the page looks.
* Means you can change the styles used across all pages by altering just one file (rather than each individual page).*


*here are many different types of CSS selector that allow you to target rules to specific elements in an HTML document. The table on the opposite page introduces the most commonly used CSS selectors.On this page, there is an HTML file to demonstrate which elements these CSS selectors would apply to.*

*CSS selectors are case sensitive, so they must match element names and attribute values exactly.There are some more advanced selectors which allow you to select elements based on attributes and their values* 


---------------------------------------------------------------------------------------------------------------------------------------------------

## Js
![vdvd](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRidvQ2qNaTGeNrYi6ZHiNL9QwMFwkfjHCGBeBCwlcHGZE2UfFKhT-0uiLf1vzp3pIg2d4&usqp=CAU.jpg)


>JavaScript is a text-based programming language used both on the client-side and server-side that allows you to make web pages interactive. Where HTML and CSS are languages that give structure and style to web pages, JavaScript gives web pages interactive elements 

>What is JavaScript used for? 
>JavaScript is mainly used for web-based applications and web browsers. But JavaScript is also used beyond the Web in software, servers and embedded hardware controls. Here are some basic things JavaScript is used for:

 

1. Adding interactive behavior to web pages JavaScript allows users to interact with web pages. There are almost no limits to the things you can do with JavaScript on a web page
>these are just a few examples:

-|-
-|-
1|Show or hide more information with the click of a button

2|Change the color of a button when the mouse hovers over it

3|Slide through a carousel of images on the homepage

4|Zooming in or zooming out on an image

5|Displaying a timer or count-down on a website

6|Playing audio and video in a web page

7|Displaying animations

8|Using a drop-down hamburger menu

 

2. Creating web and mobile apps Developers can use various JavaScript frameworks for developing and building web and mobile apps. JavaScript frameworks are collections of JavaScript code libraries that provide developers with pre-written code to use for routine programming features and tasks—literally a framework to build websites or web applications around. 

###### Popular JavaScript front-end frameworks include React, React Native, Angular, and Vue. Many companies use Node.js, a JavaScript runtime environment built on Google Chrome’s JavaScript V8 engine. A few famous examples include Paypal, LinkedIn, Netflix, and Uber!

 

3. Building web servers and developing server applications Beyond websites and apps, developers can also use JavaScript to build simple web servers and develop the back-end infrastructure using Node.js. 

 

4. Game developmentOf course, you can also use JavaScript to create browser games. These are a great way for beginning developers to practice their JavaScript skills. 

 

###### Why use JavaScript over other programming languages? 
>Aside from the unlimited possibilities, there are many reasons for web developers to use JavaScript over other programming languages:
-|-
-|-
1|JavaScript is the only programming language native to the web browser

2|JavaScript is the most popular language

3|There’s a low threshold to get started

4|It’s a fun language to learn




COMMENTS `//`
