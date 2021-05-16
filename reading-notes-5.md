# HTML & CSS Reviwe 
![HTML&CSS](https://www.lambdatest.com/blog/wp-content/uploads/2018/11/JPG-2.jpg)

# images
![Images](https://i.ytimg.com/vi/G6jZUJcOmgI/maxresdefault.jpg)

##  Choosing Images for Your Site

Images can be used to set the 
tone for a site in less time than 
it takes to read a description. If 
you do not have photographs 
to use on your website, there 
are companies who sell stock 
images; these are images you 
pay to use (there is a list of stock 
photography websites below). 
Remember that all images are 
subject to copyright, and you 
can get in trouble for simply 
taking photographs from 
another website.


If you have a page that shows 
several images (such as product 
photographs or members of a 
team) then putting them on a 
simple, consistent background 
helps them look better as 
a group.

Images should...

* Be relevant
* Convey information
* Convey the right mood 
* Be instantly recognisable 
* Fit the color palette

## Storing Images on Your Site


As a website grows, keeping 
images in a separate folder 
helps you understand how the 
site is organized. Here you can 
see an example of the files for 
a website; all of the images are 
stored in a folder called images.


On a big site you might like to 
add subfolders inside the images
folder. For example, images such 
as logos and buttons might sit in 
a folder called interface, product 
photographs might sit in a page 
called products, and images 
related to news might live in a 
folder called news.


If you are using a content 
management system or blogging 
platform, there are usually tools 
built into the admin site that 
allow you to upload images, 
and the program will probably 
already have a separate folder 
for image files and any 
other uploads

## Adding Images

### `<img>` 


To add an image into the page 
you need to use an <img>
element. This is an empty 
element (which means there is 
no closing tag). It must carry the 
following two attributes:

* src :

This tells the browser where 
it can find the image file. This 
will usually be a relative URL 
pointing to an image on your 
own site. (Here you can see that 
the images are in a child folder 
called images — relative URLs 
were covered on pages 83-84). 

* alt :

This provides a text description 
of the image which describes the 
image if you cannot see it.

* title :

You can also use the title
attribute with the <img> element 
to provide additional information 
about the image. Most browsers 
will display the content of this 
attribute in a tootip when the 
user hovers over the image.

## Height & Width of Images

You will also often see an `<img>`
element use two other attributes 
that specify its size:

* height :

This specifies the height of the 
image in pixels.

* width :

This specifies the width of the image in pixels.
Images often take longer to 
load than the HTML code that 
makes up the rest of the page. 
It is, therefore, a good idea to 
specify the size of the image 
so that the browser can render 
the rest of the text on the page 
while leaving the right amount of 
space for the image that is still 
loading.

## Where to Place Images in Your Code

Where an image is placed 
in the code will affect how it 
is displayed. Here are three 
examples of image placement 
that produce different results:

1. before a paragraph The paragraph starts on a new line after the image.

2. inside the start of a paragraph The first row of text aligns with the bottom of the image.

3. in the middle of a paragraph The image is placed between the words of the paragraph that it appears in.

Where you place the image in 
the code is important because 
browsers show HTML elements 
in one of two ways:

Block elements always appear 
on a new line. Examples of block 
elements include the `<h1>` and 
`<p>` elements.

If the `<img>` is followed by a 
block level element (such as a 
paragraph) then the block level 
element will sit on a new line 
after the imageas shown in the 
first example on this page.
Inline elements sit within a 
block level element and do not 
start on a new line. Examples of 
inline elements include the `<b>`, 
`<em>`, and `<img>` elements.

## Old Code: Aligning Images Horizontally

* align :

The align attribute was 
commonly used to indicate how 
the other parts of a page should 
flow around an image. It has 
been removed from HTML5 
and new websites should use 
CSS to control the alignment of 
images .

I have discussed it here because 
you are likely to come across 
it if you look at older code, and 
because some visual editors still 
insert this attribute when you 
indicate how an image should be 
aligned.

The align attribute can take 
these horizontal values:

1. left :

This aligns the image to the left 
(allowing text to flow around its 
right-hand side).

2. right : 

This aligns the image to the right 
(allowing text to flow around its 
left-hand side).

## Old Code: Aligning Images Vertically

As you saw on the last page, the 
align attribute is no longer used 
in HTML5, but it is covered here 
because you may see it used in 
older websites and it is still used 
in the code created by some 
visual editors.

There are three values that the 
align attribute can take that 
control how the image should 
align vertically with the text that 
surrounds it:

* top :

This aligns the first line of the 
surrounding text with the top of 
the image.

* middle :

This aligns the first line of the 
surrounding text with the middle 
of the image.

* bottom :

This aligns the first line of the 
surrounding text with the bottom 
of the image.

## Three Rules for Creating Images

1.  Save images in the right format
Websites mainly use images in jpeg, gif, or png format. If you choose the wrong image format then your image might not look as sharp as it should and can make the web page slower to load.


2. Save images at the right size You should save the image at the same width and height it will appear on the website. If the image is smaller than the width or height that you have specified, the image can be distorted and stretched. If the image is larger than the width and height if you have specified, the image will take longer to display on the page.


3. Use the correct resolution Computer screens are made up of dots known as pixels. Images used on the web are also made up of tiny dots. Resolution refers to the number of dots per inch, and most computer screens only show web pages at 72 pixels per inch.So saving images at a higher resolution results in images that are larger than necessary and take longer to download

## Image Formats: JPEG 

Whenever you have many different 
colors in a picture you should use a JPEG. 
A photograph that features snow or an 
overcast sky might look like it has large 
areas that are just white or gray, but the 
picture is usually made up of many different 
colors that are subtly different.

## Image Formats: GIF 

Use GIF or PNG format 
when saving images 
with few colors or large 
areas of the same color.

When a picture has an area that is filled 
with exactly the same color, it is known as 
flat color. Logos, illustrations, and diagrams 
often use flat colors.

## Image Dimensions 

The images you use on your website should be 
saved at the same width and height that you 
want them to appear on the page.

For example, if you have 
designed a page to include an 
image that is 300 pixels wide by 
150 pixels tall, the image you use 
should be 300 x 150 pixels. You 
may need to use image editing 
tools to resize and crop the image. 

When sourcing images, it 
is important to understand how 
you can alter the dimensions of 
an image; imagine that you had 
designed a web page to include 
an image that is 300 pixels wide 
by 150 pixels tall:

* REDUCING IMAGE SIZE

You can reduce the size of 
images to create a smaller 
version of the image.

Example: If your image is 600 
pixels wide and 300 pixels tall, 
you can reduce the size of the 
image by 50%.


* INCREASING IMAGE SIZE

You can't increase the size of 
photos significantly without 
affecting the image quality.

Example: If your image is only 
100 pixels wide by 50 pixels tall, 
increasing the size by 300% 
would result in poor quality.

* CHANGING SHAPE

Only some images can be 
cropped without losing valuable 
information .

Example: If your image is 300 
pixels square, you can remove 
parts of it, but in doing so you 
might lose valuable information.

## Cropping Images

When cropping images it is important not to 
lose valuable information. It is best to source 
images that are the correct shape if possible.

## Image Resolution

Images created for the web should be saved at 
a resolution of 72 ppi. The higher the resolution 
of the image, the larger the size of the file.

JPGs, GIFs, and PNGs belong to 
a type of image format known 
as bitmap. They are made up of 
lots of miniature squares. The 
resolution of an image is the 
number of squares that fit within 
a 1 inch x 1 inch square area.

Images appearing on computer
screens are made of tiny squares 
called pixels. A small segment 
of this photograph has been 
magnified to show how it is 
made up of pixels. The web 
browsers on most desktop 
computers display images at a 
resolution of 72 pixels per inch 
(ppi). 

Images in print materials 
(such as books and magazines) 
are made up of tiny circles called 
dots. These images are usually 
printed at a resolution of 300
dots per inch (dpi).

## Vector Images

Vector images differ from bitmap images and 
are resolution-independent. Vector images are 
commonly created in programs such as Adobe 
Illustrator.

When an image is a line drawing 
(such as a logo, illustration, or 
diagram), designers will often 
create it in vector format.
Vector formatted images are 
very different to bitmap images.

Vector images are created by 
placing points on a grid, and 
drawing lines between those 
points. A color can then be 
added to "fill in" the lines that 
have been created.

The advantage of creating line 
drawings in vector format is that 
you can increase the dimensions 
of the image without affecting 
the quality of it.

## Animated GIFs 

Animated GIFs show several frames of an 
image in sequence and therefore can be used to 
create simple animations.

## Transparency

Creating an image that is partially transparent 
(or "see-through") for the web involves 
selecting one of two formats:

* Transparent GIF :

If the transparent part of the 
image has straight edges and 
it is 100% transparent (that is, 
not semi-opaque), you can save 
the image as a GIF (with the 
transparency option selected).

* PNG :

If the transparent part of the image has diagonal or rounded 
edges or if you want a semiopaque transparency or a dropshadow,then you will need to save it as a PNG

## Examining Images on the Web

* Checking the Size of Images

If you are updating a website, you might need to check the size of an existing image before creating a new one to replace it. This can be achieved by right-clicking on the image and making a selection from the pop-up menu that appears.

* Downloading Images

If you want to download images from a website, you can do so by 
accessing the same pop-up menu.

## HTML5: Figure and Figure Caption

### `<figure>`

Images often come with 
captions. HTML5 has introduced 
a new `<figure>` element to 
contain images and their caption 
so that the two are associated. 

You can have more than one 
image inside the `<figure>`
element as long as they all share 
the same caption.

### `<figcaption>`

The `<figcaption>` element has 
been added to HTML5 in order 
to allow web page authors to add 
a caption to an image.
Before these elements were 
created there was no way to 
associate an `<img>` element with 
its caption

## Summary 


* The `<img>` element is used to add images to a 
web page.


* You must always specify a src attribute to indicate the 
source of an image and an alt attribute to describe the 
content of an image.


* You should save images at the size you will be using 
them on the web page and in the appropriate format.


* Photographs are best saved as JPEGs; illustrations or 
logos that use flat colors are better saved as GIFs.


# color

![color](https://html.com/wp-content/uploads/html-color.png)

## Foreground Color

The color property allows you 
to specify the color of text inside 
an element. You can specify any 
color in CSS in one of three ways:

* rgb values

These express colors in terms 
of how much red, green and 
blue are used to make it up. For 
example: rgb(100,100,90)

* hex codes

These are six-digit codes that 
represent the amount of red, 
green and blue in a color, 
preceded by a pound or hash # 
sign. For example: #ee3e80

* color names

There are 147 predefined color 
names that are recognized 
by browsers. For example: 
DarkCyan

We look at these three different 
ways of specifying colors on the 
next double-page spread

## Background Color

CSS treats each HTML element 
as if it appears in a box, and the 
background-color property 
sets the color of the background 
for that box.

You can specify your choice of 
background color in the same 
three ways you can specify 
foreground colors: RGB values, 
hex codes, and color names.

If you do not specify a 
background color, then the 
background is transparent.

By default, most browser 
windows have a white 
background, but browser users 
can set a background color for 
their windows, so if you want 
to be sure that the background 
is white you can use the 
background-color property on 
the `<body>` element.

## Understanding Color

Every color on a computer screen is created by mixing amounts of red, green, and blue. To find the color you want, you can use a color picker.

Computer monitors are made 
up of thousands of tiny squares 
called pixels (if you look very 
closely at your monitor you 
should be able to see them).

When the screen is not turned 
on, it's black because it's not 
emitting any light. When it's 
on, each pixel can be a different 
color, creating a picture.

The color of every pixel on the 
screen is expressed in terms of 
a mix of red, green, and blue
just like on a television screen.

* RGB Values

Values for red, green, and blue 
are expressed as numbers 
between 0 and 255. 

* Hex Codes

Hex values represent values 
for red, green, and blue in 
hexadecimal code.

* Color Names

Colors are represented by 
predefined names. However, 
they are very limited in number.

* Hue

Hue is near to the colloquial idea 
of color. Technically speaking 
however, a color can also have 
saturation and brightness as 
well as hue.

* Saturation

Saturation refers to the amount 
of gray in a color. At maximum 
saturation, there would be no 
gray in the color. At minimum 
saturation, the color would be 
mostly gray.

* Brightness

Brightness (or "value") refers 
to how much black is in a color. 
At maximum brightness, there 
would be no black in the color. 
At minimum brightness, the 
color would be very dark

## Contrast

When picking foreground and background 
colors, it is important to ensure that there is 
enough contrast for the text to be legible.

* Low Contrast

Text is harder to read when 
there is low contrast between 
background and foreground 
colors. 

A lack of contrast is particularly 
a problem for those with 
visual impairments and color 
blindness.

It also affects those with poor 
monitors and sunlight on their 
screens (which is increasingly 
common as people use handheld 
devices outdoors).

* High Contrast

Text is easier to read when 
there is higher contrast between 
background and foreground 
colors.

If you want people to read a lot 
of text on your page, however, 
then too much contrast can 
make it harder to read, too. 

* Medium Contrast

For long spans of text, reducing 
the contrast a little bit improves 
readability.


You can reduce contrast by 
using dark gray text on a white 
background or an off-white text 
on a dark background.

## CSS3: Opacity

CSS3 introduces the opacity
property which allows you to 
specify the opacity of an element 
and any of its child elements. 
The value is a number between 
0.0 and 1.0 (so a value of 0.5
is 50% opacity and 0.15 is 15% 
opacity).

The CSS3 rgba property allows 
you to specify a color, just like 
you would with an RGB value, 
but adds a fourth value to 
indicate opacity. This value is 
known as an alpha value and is 
a number between 0.0 and 1.0
(so a value of 0.5 is 50% opacity 
and 0.15 is 15% opacity). The 
rgba value will only affect the 
element on which it is applied 
(not child elements).

Because some browsers will 
not recognize RGBA colors, you 
can offer a fallback so that they 
display a solid color. If there are 
two rules that apply to the same 
element, the latter of the two 
will take priority. To create the 
fallback, you can specify a color 
as a hex code, color name or 
RGB value, followed by the rule 
that specifies an RGBA value. If 
the browser understands RGBA 
colors it will use that rule. If it 
doesn't, it will use the RGB value.

## CSS3: HSL Colors

CSS3 introduces an entirely new and intuitive 
way to specify colors using hue, saturation, 
and lightness values.

* hue

Hue is the colloquial idea of 
color. In HSL colors, hue is often 
represented as a color circle 
where the angle represents the 
color, although it may also be 
shown as a slider with values 
from 0 to 360.

* saturation

Saturation is the amount of 
gray in a color. Saturation is 
represented as a percentage. 
100% is full saturation and 0% 
is a shade of gray.

* lightness

Lightness is the amount of 
white (lightness) or black 
(darkness) in a color. Lightness 
is represented as a percentage. 
0% lightness is black, 100% 
lightness is white, and 50% 
lightness is normal. Lightness 
is sometimes referred to as 
luminosity.

## CSS3: HSL & HSLA

The hsl color property has 
been introduced in CSS3 as an 
alternative way to specify colors. 
The value of the property starts 
with the letters hsl, followed 
by individual values inside 
parentheses for:

* hue

This is expressed as an angle 
(between 0 and 360 degrees).
saturation
This is expressed as a 
percentage.

* lightness

This is expressed as a 
percentage with 0% being white, 
50% being normal, and 100% 
being black.

The hsla color property allows 
you to specify color properties 
using hue, saturation, and 
lightness as above, and adds a 
fourth value which represents 
transparency (just like the rgba
property). The a stands for:

* alpha

This is expressed as a 
number between 0 and 1.0. 
For example, 0.5 represents 
50% transparency, and 0.75
represents 75% transparency.

## Summary


* Color not only brings your site to life, but also helps convey the mood and evokes reactions.


* There are three ways to specify colors in CSS: 
RGB values, hex codes, and color names.


* Color pickers can help you find the color you want.


* It is important to ensure that there is enough contrast between any text and the background color (otherwise people will not be able to read your content).


* CSS3 has introduced an extra value for RGB colors to indicate opacity. It is known as RGBA.


* CSS3 also allows you to specify colors as HSL values, with an optional opacity value. It is known as HSLA.


# Text 
![text](https://flaviocopes.com/html-text-tags/various.png)

## Typeface Terminology

* Serif 

Serif fonts have extra details on 
the ends of the main strokes of 
the letters. These details are 
known as serifs.

In print, serif fonts were 
traditionally used for long 
passages of text because they 
were considered easier to read.

* Sans-Serif

Sans-serif fonts have straight 
ends to letters, and therefore 
have a much cleaner design.

Screens have a lower resolution 
than print. So, if the text is small, 
sans-serif fonts can be clearer 
to read.

* Monospace

Every letter in a monospace (or 
fixed-width) font is the same 
width. (Non-monospace fonts 
have different widths.)

Monospace fonts are commonly 
used for code because they align 
nicely, making the text easier to 
follow.

## Choosing a Typeface for your Website

When choosing 
a typeface, it 
is important to 
understand that a 
browser will usually 
only display it if it's 
installed on that 
user's computer.

* Serif

Serif fonts have extra details on 
the end of the main strokes of 
the letters.

* Sans-Serif

Sans-serif fonts have straight 
ends to letters and therefore 
have a much cleaner design.

* Monospace

Every letter in a monospace 
typeface is the same width. 
(Non-monospace fonts have 
different widths.)

* Cursive

Cursive fonts either have 
joining strokes or other cursive 
characteristics, such as 
handwriting styles.

* Fantasy

Fantasy fonts are usually 
decorative fonts and are often 
used for titles. They're not 
designed for long bodies of text.

## Techniques That Offer a Wider Choice of Typefaces

There are several ways to use fonts other than those listed on the previous page. However, typefaces are subject to copyright, so the techniques you can choose from are limited by their respective licenses.

font-family |font-face |Service-based Font-Face
-|-|-
The user's computer needs the typeface installed. CSS is used to specify the typeface.|CSS specifies where a font can be downloaded from if it is not installed on the computer.|Commercial services give users access to a wider range of fonts using @font-face.
Issues|
There is a limited choice of typefaces that most users have installed.|The user has to download the font file, which can slow down loading of the web page.|There is an ongoing fee to cover licenses paid to font foundries.
Licensing|
You are not distributing the typeface, so there is no licensing issue.|The license to use the font must permit its distribution using @font-face.|The service takes care of the licensing issues with the people who made the font.
Choice of Typefaces|
There is a limited choice because the font needs to be installed on users' computers.|Choice is limited because few typefaces can be freely distributed this way.|Each service offers a different choice of fonts based on their agreements with font foundries.

## Specifying Typefaces 

The font-family property 
allows you to specify the 
typeface that should be used for 
any text inside the element(s) to 
which a CSS rule applies.

The value of this property is the 
name of the typeface you want 
to use.

The people who are visiting 
your site need the typeface you 
have specified installed on their 
computer in order for it to be 
displayed. 

You can specify a list of fonts 
separated by commas so that, 
if the user does not have your 
first choice of typeface installed, 
the browser can try to use an 
alternative font from the list.

It is also common to end with a 
generic font name for that type 
of font (which you saw on pages 
269-270).

If a font name is made up of 
more than one word, it should be 
put in double quotes.

Designers suggest pages usually 
look better if they use no more 
than three typefaces on a page.

## Size Of Type 

The font-size property enables 
you to specify a size for the 
font. There are several ways to 
specify the size of a font. The 
most common are:

* pixels

Pixels are commonly used 
because they allow web 
designers very precise control 
over how much space their text 
takes up. The number of pixels is 
followed by the letters px.

* percentages

The default size of text in 
browsers is 16px. So a size of 
75% would be the equivalent of 
12px, and 200% would be 32px.

If you create a rule to make all 
text inside the `<body>` element 
to be 75% of the default size (to 
make it 12px), and then specify 
another rule that indicates the 
content of an element inside the 
`<body>` element should be 75% 
size, it will be 9px (75% of the 
12px font size).

* ems

An em is equivalent to the width 
of a letter m.

## Understanding Font Format

Different browsers support 
different formats for fonts 
(in the same way that they 
support different audio and 
video formats), so you will need 
to supply the font in several 
variations to reach all browsers.

If you do not have all of these 
formats for your font, you can 
upload the font to a website 
called FontSquirrel where they 
will convert it for you: 

www.fontsquirrel.com/

fontface/generator

Font Squirrel also provides you 
with the CSS code for the 
@font-face rule. This is very 
helpful because, when you 
are dealing with multiple font 
formats, the src and format
properties of the @font-face
rule can get rather complicated.

You can see an example of a 
more complicated @font-face 
rule on the left.

## Bold 

The font-weight property 
allows you to create bold text. 
There are two values that this 
property commonly takes:

* normal

This causes text to appear at a 
normal weight.

* bold

This causes text to appear bold.

In this example, you can see 
that the element whose class
attribute has a value of credits
has been bolded.

## Italic

If you want to create italic text, 
you can use the font-style
property. There are three values 
this property can take:

* normal

This causes text to appear in a 
normal style (as opposed to italic 
or oblique).

* italic

This causes text to appear italic.

* oblique

This causes text to appear 
oblique.

## UpperCase & LowerCase

The text-transform property 
is used to change the case of 
text giving it one of the following 
values:

* uppercase

This causes the text to appear 
uppercase.

* lowercase

This causes the text to appear 
lowercase.

* capitalize

This causes the first letter of 
each word to appear capitalized.

## Underline & Strike 

The text-decoration property 
allows you to specify the 
following values:

* none

This removes any decoration 
already applied to the text.

* underline

This adds a line underneath the 
text.

* overline

This adds a line over the top of 
the text.

* line-through

This adds a line through words.

* blink

This animates the text to make it 
flash on and off (however this is 
generally frowned upon, as it is 
considered rather annoying).

## Leading

Leading  is a term typographers use for the 
vertical space between lines of 
text. In a typeface, the part of 
a letter that drops beneath the 
baseline is called a descender, 
while the highest point of a letter 
is called the ascender. Leading 
is measured from the bottom of 
the descender on one line to the 
top of the ascender on the next.

In CSS, the line-height
property sets the height of 
an entire line of text, so the 
difference between the fontsize 
and the line-height is 
equivalent to the leading (as 
shown in the diagram above).

Increasing the line-height
makes the vertical gap between 
lines of text larger.

## Letter & Word Spacing 

Kerning is the term 
typographers use for the space 
between each letter. You can 
control the space between each 
letter with the letter-spacing
property.

It is particularly helpful to 
increase the kerning when 
your heading or sentence is 
all in uppercase. If your text is 
in sentence (or normal) case, 
increasing or decreasing the 
kerning can make it harder to 
read.

You can also control the gap 
between words using the 
word-spacing property. 

When you specify a value for 
these properties, it should 
be given in ems, and it will be 
added on top of the default value 
specified by the font.

The default gap between 
words is set by the typeface 
(often around 0.25em), and 
it is unlikely that you would 
need to change this property 
regularly. If the typeface is bold 
or you have increased the space 
between letters, then a larger 
gap between words can increase 
readability.

## Alignment

The text-align property allows 
you to control the alignment of 
text. The property can take one 
of four values:

* left

This indicates that the text 
should be left-aligned.

* right

This indicates that the text 
should be right-aligned.

* center

This allows you to center text.

* justify

This indicates that every line in 
a paragraph, except the last line, 
should be set to take up the full 
width of the containing box.

## Summary


* There are properties to control the choice of font, size, weight, style, and spacing.


* There is a limited choice of fonts that you can assume most people will have installed.


* If you want to use a wider range of typefaces there are several options, but you need to have the right license to use them.


* You can control the space between lines of text, individual letters, and words. Text can also be aligned to the left, right, center, or justified. It can also be indented.


* You can use pseudo-classes to change the style of an element when a user hovers over or clicks on text,or when they have visited a link.

