# HTML Layout
![sdasdad](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTXlJasL34NfbfmVHj_BANsBQh7ZyZObB3JzA&usqp=CAU.jpg)


### What is layout of HTML?

>HTML layouts provide a way to arrange web pages in well-mannered, well-structured, and in responsive form or we can say that HTML layout specifies a way in which the web pages can be arranged. Web-page layout works with arrangement of visual elements of an HTML document.

### How do you create a layout in HTML?
>HTML Layout Elements
1. `<header>` - Defines a header for a document or a section.
2. `<nav>` - Defines a set of navigation links.
3. `<section>` - Defines a section in a document.
4. `<article>` - Defines an independent self-contained content.
5. `<aside>` - Defines content aside from the content (like a sidebar)
 
###  What is layout techniques?

> CSS layout techniques allow us to define the placement of elements on a web page, that is to control where they are positioned with respect to their default position as per normal flow, the other elements around them, their parent container, or the main viewport/window.

1. position:static
 ### In normal flow, each block-level element sits on top of the next one. Since this is the default way in which browsers treat HTML elements, you do not need a CSS property to indicate that elements should appear in normal flow, but the syntax.

 2. position:relative
 > Relative positioning moves an element in relation to where it would have been in normal flow.For example, you can move it 10 pixels lower than it would have been in normal flow or 20% to the right.
> You can indicate that an element should be relatively positioned using the position property with a value of relative.You then use the offset properties (top or bottom and left or right) to indicate how far to move the element from where it would have been in normal flow


3. position:absolute
> An element with position: absolute; is positioned relative to the nearest positioned ancestor (instead of positioned relative to the viewport, like fixed). However; if an absolute positioned element has no positioned ancestors, it uses the document body, and moves along with page scrolling.

### What is position relative and absolute?
> position: relative places an element relative to its current position without changing the layout around it, whereas position: absolute places an element relative to its parent's position and changing the layout around it.

##### Relative - the element is positioned relative to its normal position. Absolute - the element is positioned absolutely to its first positioned parent. Fixed - the element is positioned related to the browser window. Sticky - the element is positioned based on the user's scroll position.

>Properties of CSS: Inline CSS has the highest priority, then comes Internal/Embedded followed by External CSS which has the least priority.

4. position:fixed
>A fixed position element is positioned relative to the viewport, or the browser window itself. The viewport doesn't change when the window is scrolled, so a fixed positioned element will stay right where it is when the page is scroll‏.

### What is the difference between position fixed and absolute?

>Whereas the position and dimensions of an element with position:absolute are relative to its containing block, the position and dimensions of an element with position:fixed are always relative to the initial containing block.

### How do you make a fixed position responsive?

1. “how to make fixed position responsive” Code Answer
2. responsive-div {
3. position: fixed;
4. width: 70vw; // vw being viewport-width, so 70% of the width of the viewport.
5. height: 50vh; // vh being viewport-height, so 50% of the height of the viewport.
6. /*works well for SVG's specifically*/
7. }

5. z-index
#### Definition and Usage
> The z-index property specifies the stack order of an element.

> An element with greater stack order is always in front of an element with a lower stack order.

> Note: z-index only works on positioned elements (position: absolute, position: relative, position: fixed, or position: sticky) and flex items (elements that are direct children of display:flex elements).


### Using z-index
> The first part of this article, Stacking without the z-index property, explains how stacking is arranged by default. If you want to create a custom stacking order, you can use the z-index property on a positioned element.

##### The z-index property can be specified with an integer value (positive, zero, or negative), which represents the position of the element along the z-axis. If you are not familiar with the z-axis, imagine the page as a stack of layers, each one having a number. Layers are rendered in numerical order, with larger numbers above smaller numbers.

bottom layer (farthest from the observer)
...
Layer -3
Layer -2
Layer -1
Layer 0 (default rendering layer)
Layer 1
Layer 2
Layer 3
...
top layer (closest to the observer)

-----------------------------------------------------




6. float
> The float CSS property places an element on the left or right side of its container, allowing text and inline elements to wrap around it. The element is removed from the normal flow of the page, though still remaining a part of the flow (in contrast to absolute positioning).

### How do you add a float in HTML?
1. Let an image float to the righ
2. Let an image float to the left
3. Let image be displayed just where it occurs in the text (float: none)
4. Let the first letter of a paragraph float to the left and style the letter
6. Use float with a list of hyperlinks to create a horizontal menu

### Clearing Floats clear

> The clear property is directly related to the float property. It specifies if an element should be next to the floated elements or if it should move below them. This property applies to both floated and non-floated elements. If an element can fit in the horizontal space next to the floated elements, it will.

### How do you clear a float in CSS?
###### Both is most commonly used, which clears floats coming from either direction. Left and Right can be used to only clear the float from one direction respectively. None is the default, which is typically unnecessary unless removing a clear value from a cascade.


### width
> This sets the width of the columns.
### float
> This positions the columns next to each other.
### margin
> This creates a gap


8. Screen Sizes html
### How do you change the screen size in HTML?

1. Add this viewport meta tag inside the `<head>` tag: `<meta name="viewport"content="width=device-width">` This should make the page render at a reasonable size.

2. Add this `<style> tag inside the <head> tag: <style> img { max-width: 100%; } </style>`


