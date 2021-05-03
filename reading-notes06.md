# Js overview

![sasfsf](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTXbKjWsa3sT8gQuCzab76jHjPKLqXc6eO1Ig&usqp=CAU.jpg)

## Calling functions in JS

![gegg](https://i.stack.imgur.com/x93bg.png)

### What is call function in JavaScript?
>The call() method is a predefined JavaScript method. It can be used to invoke (call) a method with an owner object as an argument (parameter). With call() , an object can use a method belonging to another object


### How do you call a function within a function in JavaScript?
> Nested functions in JavaScript...Approach:
1. Write one function inside another function.
2. Make a call to the inner function in the return statement of the outer function.
3. Call it fun(a)(b) where a is parameter to outer and b is to the inner function.
4. Finally return the combined output from the nested function.


### How do I call a function?

1. Write the name of the function.
2. Add parentheses () after the function's name.
3. Inside the parenthesis, add any parameters that the function requires, separated by commas.

### Js getting a single value out of  functions

> Let’s start with creating a simple multiply function in Vanilla JavaScript.

` function getMultiply(numberParam) { `
   `console.log('Multiply', numberParam * numberParam);`
`}`
> We can call it with:`
`getMultiply(7);`
> So now this function will multiply the number 7. But we can’t do anything with the outcome of it.
> Return a value from the function
> Let’s bring in the return statement.
`function getMultiply(numberParam) {`
   `return numberParam * numberParam;`
`}`
> Now we have to call the function in the console.log to see the outcome.
`console.log(getMultiply(7));`
##### If we put this function into a variable, we have the outcome stored inside of it!With the return statement, you can put anything out of the function.
#### If you want to return true, false or an Object or Array.
#### How do you use the return statement?
#### If you have another way of using the statement return? Please share it in the comments!🙏 But if you have any problems with returning a value out of a JavaScript function? Please let me help you, post your question in the comments!
#### Originally published at Mr Frontend Blog.



#### Summary: in this tutorial, you will learn how to develop JavaScript functions that return multiple values.

#### JavaScript functions can return a single value. To return multiple values from a function, you can pack the return values as elements of an array or as properties of an object.

#### Returning multiple values from a function using an array
#### Suppose that the following getNames() function retrieves the first name and last name from the database or a third-party API and returns them as elements of an array:

`function getNames() {`
    `// get names from the database or API`
    `let firstName = 'John',`
        `lastName = 'Doe';`

   ` // return as an array`
    `return [firstName, lastName];`
`}`
`Code language: JavaScript (javascript)`
`The following shows how to get the return value from the getNames() function:`

`let names = getNames();`
`Code language: JavaScript (javascript)`
#### Because the names variable is an array, you can reference its elements using the square brackets, like this:

`const firstName = names[0],`
`    lastName = names[1];`
`Code language: JavaScript (javascript)`
##### In ES6, you can destructuring assignment syntax to unpack values from an array more intuitively, like this:

`const [firstName, lastName] = getNames();`
`Code language: JavaScript (javascript)`
##### In this code, the firstName and lastName variables will take the first and second elements of the return array.

> Returning multiple values from an function using an object If you want to assign a name to each returned value to make it more readable and easier to maintain, you can use an object:

`function getNames() {`
   ` // get names from the database or API`
    `let firstName = 'John',`
     `   lastName = 'Doe';`

`    // return values`
    `return {`
     `   firstName,`
        `lastName`
    `};`
`}`
##### Code language: JavaScript (javascript)
##### And you can get the return value as an object, like this:

`let names = getNames();`

`let firstName = names.firstName,`
    `lastName = names.lastName;`
`Code language: JavaScript (javascript)`
##### If you want to unpack properties from an object, you can use the object destructuring syntax as follows:

`let { firstName, lastName } = getNames();`
`Code language: JavaScript (javascript)`

### Summary
### JavaScript doesn’t support functions that return multiple values. However, you can wrap multiple values into an array or an object and return the array or the object.
### Use destructuring assignment syntax to unpack values from the array, or properties from objec.


#### ANONYMOUS FUNCTIONS & FUNCTION EXPRESSIONS

#### Expressions produce a value. They can be used where values are expected. If a function is placed where a browser expects to see an expression, (e.g., as an argument to a function), then it gets treated as an expression. 
##### FUNCTION DECLARATION 
#### A function declaration creates a function that you can call later in your code. It is the type of function you have seen so far in this book. 
#### In order to call the function later in your code, you must give it a name, so these are known as named functions. Below, a function called area() is declared, which can then be called using its name. function area (width, height) 
`return width * height; `
`}; `
`var size= area (3, 4) ;`

##### As you will see on p456, the interpreter always looks for variables and function declarations before going through each section of a script, line-by-line. 
> This means that a function created with a function declaration can be called before it has even been 
declared. For more information about how variables and functions are processed first, see the discussion 
about execution context and hoisting on. 

> § FUNCTIONS, METHODS & OBJECTS FUNCTION EXPRESSION If you put a function where the interpreter would expect to see an expression, then it is treated as an expression, and it is known as a function expression. 

###### In function expressions, the name is usually omitted. 
###### A function with no name is called an anonymous function. Below, the function is stored in a variable called area. It can be called like any function created with a function declaration. 
`var ar ea = f unction(width, height) { `
`r eturn width * height; `
`} ;` 
`var size = area (3, 4) ;`

> In a function expression, the function is not processed until the interpreter gets to that statement. This means you cannot call this function before the interpreter has discovered it. It also means that any code that appears up to that point could potentially alter what goes on inside this funct.


## VARIABLE SCOPE 
#### The location where you declare a variable will affect where it can be used within your code. If you declare it within a function, it can only be used within that function This is known as the variable's scope. 

#### LOCAL VARIABLES 
> When a variable is created inside a function using the var keyword, it can only be used in that function. It is called a local variable or function-level variable. 

>It is said to have local scope or function-level scope. It cannot be accessed outside of the function in which it was declared. Below, area is a local variable. 

#### The interpreter creates local variables when the function is run, and removes them as soon as the function has finished its task. This means that: 
* If the function runs twice, the variable can have 
different values each time. 
* Two different functions can use variables with the 
#### same name without any kind of naming conflict. 
#### GLOBAL VARIABLES 
>If you create a variable outside of a function, then it can be used anywhere within the script. It is called a global variable and has global scope. In the example shown, wa 11 Size is a global variable.

>Global variables are stored in memory for as long as the web page is loaded into the web browser. This means they take up more memory than local variables, and it also increases the risk of naming conflicts (see next page). For these reasons, you should use local variables wherever possible. If you forget to declare a variable using the var keyword, the variable will work, but it will be treated as a global variable (this is considered bad practice). 

#### function getArea(width, height) 
`var area = width * height;` 
`return area;` 
`var wallSize = getArea(3, 2);` 
`document. write(wa 11 Si ze);` 
* LOCAL (OR FUNCTION-LEVEL) SCOPE 
* GLOBAL SCOPE



---------------------------------------------------------------------------------------------------------------



## USING WHILE LOOPS

![SFSDGDG](https://www.guru99.com/images/1/020819_0538_CLoopsForW1.png)

 >while loop is used to repeat a section of code an unknown number of times until a specific condition is met For example, say we want to know how many times a given number can be divided by 2 before it is less than or equal to 1.


> while loop in C programming repeatedly executes a target statement as long as a given condition is true. The >syntax is like below.
...
>Output.
-|-
-|-
While Loop|	Do-While Loop
The while loop may run zero or more times|	Do-While may run more than one times but at least once.


#### Can we use && in while loop?
>Suppose in a while loop, you have two conditions, and any one needs to be true to proceed to the body, then in that case you can use the || operator between those two conditions, and in case you want both to be true, you can use && operator.

#### Where do we use while loop and for loop?


1. Use a for loop to iterate over an array.
2. Use a for loop when you know the loop should execute n times.
3. Use a while loop for reading a file into a variable.
4. Use a while loop when asking for user input.
5. Use a while loop when the increment value is nonstandard.


## SUMMARY
* Conditional statements allow your code to make 

* decisions about what to do next. 

* Comparison operators (===, ! ==, ==, ! =, <, >, <=, =>) are used to compare two operands. 

*Logical operators allow you to combine more than one 
* set of comparison operators. 

* if ... else statements allow you to run one set of code 

* if a condition is true, and another if it is false.

* switch statements allow you to compare a value 

* against possible outcomes (and also provides a default option if none match). 

* Data types can be coerced from one type to another. 

* All values evaluate to either truthy or falsy.

* There are three types of loop: for, while, and do ... while. Each repeats a set of statements. 



--------------------------------------------------------------------------------------------------------------------------------------------
## DOM
### THE DOM TREE IS A  MODEL OF A WEB PAGE

![MLKKL](https://upload.wikimedia.org/wikipedia/commons/thumb/5/5a/DOM-model.svg/1200px-DOM-model.svg.png)

## What is Document Object Model (DOM)?

> Document Object Model (DOM) constitutes an integral web interaction tool that creates a virtual map of the web page that loads in the browser. It may also be labeled as a programming interface for both HTML and XML documents. Web programs manipulate the structure of the document, the style and its content due to the DOM, which has nodes and objects that form a document. Without this model, programming languages wouldn't work on a browser page. Usually, a browser contains the DOM, while JavaScript acts as the client-scripting language that completes the essential connection. JavaScript manipulates the DOM in nearly all website operations such as slideshows, providing an error report on submitting an incomplete form or even toggling navigation menus.

##### In simple terms, any web page that you encounter is a document. Viewing the document as an HTML source or in a browser window is just an approach of presenting one thing in different ways. The document object model (DOM) represents a webpage as objects to enable its manipulation. With the document-oriented model, a scripting language such as JavaScript may modify it by targeting the objects.

##### It is noteworthy that browsers have different standards and the most common are the W3C DOM and WHATWG DOM standards. This necessitates a compatibility check across standards.

#### For instance, the standard DOM implementation requires the getElementsByTagName method to show in the below yields <p> elements that are persistent in the document.


### Related Blogs
>Understanding the DOM Tree and Nodes
>This post is written as a guide to some of the concepts and terms related to the DOM tree and nodes.

#### You will often find the DOM (Document Object Model) being referred to as the DOM tree because of its nodes, which are trees of objects. In our short introduction to DOM, we looked at the concept behind the DOM. We were also able to differentiate the DOM from HTML source code and define instances where they are similar and dissimilar.

##### The aim of this post is to review some of the basic HTML terminology and also learn a bit more about DOM nodes. Understanding these concepts will help you when it comes to working on both DOM and JavaScript as well as in identifying common types of nodes. In a later tutorial we will also explore how to use JavaScript to make modifications to the DOM.

### What Are Nodes in DOM?
> We have seen what constitutes an HTML document. In DOM terminology, all elements of an HTML document are nodes, including the entire document and all the HTML tags contained within it. To explain this, text constitutes text nodes, comments make up the comment nodes, while HTML attributes make up the attribute nodes.


### node.
#### Node Design
> In JavaScript, all HTML elements are handled as JavaScript objects, which are then arranged as a tree. Such an arrangement is possible since each node has specific properties or characteristics such as having a parent node, having sibling nodes, or having child nodes. A tree arises from a node's family of nodes.

##### When a node is saved in JavaScript, the family information in the tree is part of its node properties. We can have a property and children, which will have all its child nodes, and that is the logic that enables arranging the child nodes under the node in reference.

### Learn How to Manage Nodes in the DOM?
>  this blog post, you will learn how you can add, change, replace and remove nodes in the DOM.

##### In previous blog posts, we have already explored how you can access DOM elements and handle the DOM, so from what we have learned so far, we can proceed to use classes, tags, ids, and selectors to look for nodes in the DOM. We can also further use the properties of parents, children, and siblings to find relative nodes in the DOM.

> In this part of my tutorial series, you will learn how you can add, change, replace, and remove nodes in the DOM. We will be creating simple JavaScript projects where we can create, modify, and remove elements in the DOM. Our simple programs will be tailored towards the type of changes that are executed on the DOM.

> If you work as a front-end developer, then you'll know that the DOM manipulation is routine business. While HTML is the default method, using JavaScript provides a greater level of flexibility and a larger number of features.



### How do you select an element with ID?

> id of an element is unique within a page, so the id selector is used to select one unique element! To select an element with a specific id, write a hash (#) character, followed by the id of the element.


### What is an ID attribute?
> Definition and Usage. The id attribute specifies a unique id for an HTML element (the value must be unique within the HTML document). The id attribute is most used to point to a style in a style sheet, and by JavaScript (via the HTML DOM) to manipulate the element with the specific id.

### Are ID selectors part of the dom?
The id selectors are part of the DOM.

### What is an element attribute?
> Attributes define additional characteristics or properties of the element such as width and height of an image. Attributes are always specified in the start tag (or opening tag) and usually consists of name/value pairs like name="value" . Attribute values should always be enclosed in quotation marks.


### SELECTING ELEMENTS BY TAG NAME 


##### How do I get element by tag name?

>HTML DOM getElementsByTagName() Method

>The getElementsByTagName() method returns a collection of all elements in the document with the specified tag name, as an HTMLCollection object The HTMLCollection object represents a collection of nodes. The nodes can be accessed by index numbers. The index starts at 0.

#### How do you get all the elements of a specified element by its tag name?

> The Element. getElementsByTagName() method returns a live HTMLCollection of elements with the given tag name. All descendants of the specified element are searched, but not the element itself.



---------------------------------------------------------------------------------------------------------------------------------------



#### ACCESSING TEXT ONLY 
##### How to browse in Text-Only Mode in Chrome
!VDVDG](http://www.gstatic.com/images/icons/material/apps/fonts/1x/catalog/v5/opengraph_color.png)
1. Open Google Chrome browser on your computer.
2. Click the three-dotted icon and select Settings.
3. Go to the Privacy and security tab.
4. Click on Site Settings > Images.
5. Toggle the Show all button.
6. Click on JavaScript.
7. Toggle the Allowed button.
8. Start browsing the internet in text-only mode.
