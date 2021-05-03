# Js overview






## What is array of objects in Javascript?
> JAVA ARRAY OF OBJECT, as defined by its name, stores an array of objects. Unlike a traditional array that store values like string, integer, Boolean, etc an array of objects stores OBJECTS. The array elements store the location of the reference variables of the object.

### What is an array object?
> Arrays of Objects. An array of objects, all of whose elements are of the same class, can be declared just as an array of any built-in type. Each element of the array is an object of that class. Being able to declare arrays of objects in this way underscores the fact that a class is similar to a type.

### Can you have an array of objects in Java?
> Answer: Yes. Java can have an array of objects just like how it can have an array of primitive types. ... Answer: In Java, an array is a dynamically created object that can have elements that are primitive data types or objects. The array may be assigned variables that are of type object.

### How do you create an array of objects in Java?
1. public class ArrayOfObjects. {
2. public static void main(String args[]) {
3. //create an array of product object.
4. Product[] obj = new Product[5] ;
5. //create & initialize actual product objects using constructor.
6. obj[0] = new Product(23907,"Dell Laptop")
dvsdss

### THE BROWSER OBJECT MODEL: THE WINDOW OBJECT


### What is browser window object?
> The window object represents an open window in a browser. If a document contain frames (`<iframe>` tags), the browser creates one window object for the HTML document, and one additional window object for each frame.

### What is the window object in JavaScript?
> The window object is a global object that has the properties pertaining to the current DOM document, which is what's in the tab of a browser. The document property of the window object has the DOM document and associated nodes and methods that we can use to manipulate the DOM nodes and listen to events for each node.

### What is BOM and Dom?
> The BOM (Browser Object Model) consists of the objects navigator , history , screen , location and document which are children of window . In the document node is the DOM (Document Object Model), the document object model, which represents the contents of the page.

### What are different types of window objects?
> that are different types of window objects? The javascript objects are string, array, date etc..
‏



### How can document object be used to access form elements?
> The Form Object in HTML DOM is used to represent the HTML < form > element. This tag is used to set or get the properties of < form > element. This element can be accessed by using getElementById() method.

### What is meant by document object model?
> Introduction. The Document Object Model (DOM) is a programming API for HTML and XML documents. It defines the logical structure of documents and the way a document is accessed and manipulated. ... The Document Object Model can be used with any programming language. HTML: `<object>` tag. This HTML tutorial explains how to use the HTML element called the `<object>` tag with syntax and examples.

## GLOBAL OBJECTS:


### What is a global object?
> A global object is an object that always exists in the global scope. ... The global object's interface depends on the execution context in which the script is running. For example: In a web browser, any code which the script doesn't specifically start up as a background task has a Window as its global object.

### Is console a global object?
> According the the Node documentation, the console object is a global that has a few methods allowing developers to do things such as printing a log or an error. Digging deeper into the docs we can see that console is really a global instance that is configured to write to process. stdout and process. stderr .



### Why code written in node JS is pretty fast?
> Being built on Google Chrome's V8 JavaScript Engine, Node. js library is very fast in code execution. ... B - Node based server uses a single threaded model and can services much larger number of requests than traditional server like Apache HTTP Server.

### How node JS overcomes the problem of blocking of I O operations?
> By putting the event-based model at its core and using an event loop instead of threads, Node. js overcomes the problem of blocking I/O operations.

### CREATING A DATE OBJECT
#### How do you create a date object?

> To create a date, we can use the datetime() class (constructor) of the datetime module. The datetime() class requires three parameters to create a date: year, month, day.

What is Type Date?
<input type="date"> <input> elements of type="date" create input fields that let the user enter a date, either with a textbox that validates the input or a special date picker interface. ... The time and datetime-local input types support time and date+time input

What is date and time called?
Loading when this answer was accepted… Though perhaps awkward in some contexts, timestamp does fit your desired meaning. The date and time at which an event occurs or occurred, usually indicated in human-readable form, especially when used in a log to track events.

HOW MEMORY & VARIABLES WORK
In JavaScript, when we create variables, functions, or anything you can think of, the JS engine allocates memory for this and releases it once it's not needed anymore. Allocating memory is the process of reserving space in memory, while releasing memory frees up space, ready to be used for another purpose.

How are variables stored in memory?
dsfddsgdg

Most variables stored in the array (i.e., in main memory) are larger than one byte, so the address of each variable is the index of the first byte of that variable. Viewing main memory as an array of bytes. ... An address is equivalent to an index into the memory array. Most C++ data types span multiple bytes of memory.

A Memory leak can be defined as a piece of memory that is no longer being used or required by an application but for some reason is not returned back to the OS and is still being occupied needlessly. ... A Javascript memory leak occurs when you may no longer need an object but the JS runtime still thinks you do.
In JavaScript, memory is automatically allocated each time you create, for instance, an object, an array, a string, or a DOM element. ... A sawtooth pattern with these vertical drops coinciding with garbage collection may also indicate a memory leak. Memory leaks can assume many shapes and forms, though.
How does JavaScript memory management work?
These primitives are used by the developer to explicitly allocate and free memory from and to the operating system. At the same time, JavaScript allocates memory when things (objects, strings, etc.) are created and “automatically” frees it up when they are not used anymore, a process called garbage collection.

How are variables stored in memory JavaScript?
Variables in JavaScript (and most other programming languages) are stored in two places: stack and heap. A stack is usually a continuous region of memory allocating local context for each executing function. ... Even if a function calls itself recursively, each frame has its own copy of all local variables.

CREATING· OBJECTS USING LITERAL NOTATION
What is object literal notation of JavaScript?
The Object literal notation is basically an array of key:value pairs, with a colon separating the keys and values, and a comma after every key:value pair, except for the last, just like a regular array. Values created with anonymous functions are methods of your object.

How do you make an object literal?
Object literals are defined using the following syntax rules:

A colon separates property name[1] from value.
A comma separates each name-value pair from the next.
A comma after the last name-value pair is optional. [2]
Do we have classes in JavaScript?
In JavaScript, there are no classes in the class-based OOP sense of the word. JavaScript works with objects. If you want to encapsulate a few functions and properties together, you would create an object containing functions and properties, and not a class. ... JavaScript doesn't have blueprints, it only has houses.

Computed properties allow you to dynamically choose what property in your object gets updated. It's important to give your input element a name attribute. The name attribute that you specify should match the property that you wish to update within the object. Retrieve the name and value from even‏.
Object Types (Blueprints) (Classes)
They only create single objects. Sometimes we need a "blueprint" for creating many objects of the same "type". The way to create an "object type", is to use an object constructor function. In the example above, function Person() is an object constructor function.

## What is array of objects in Javascript?

> JAVA ARRAY OF OBJECT, as defined by its name, stores an array of objects. Unlike a traditional array that store values like string, integer, Boolean, etc an array of objects stores OBJECTS. The array elements store the location of the reference variables of the object.

### What is an array object?

> Arrays of Objects. An array of objects, all of whose elements are of the same class, can be declared just as an array of any built-in type. Each element of the array is an object of that class. Being able to declare arrays of objects in this way underscores the fact that a class is similar to a type.

### Can you have an array of objects in Java?

> Answer: Yes. Java can have an array of objects just like how it can have an array of primitive types. ... Answer: In Java, an array is a dynamically created object that can have elements that are primitive data types or objects. The array may be assigned variables that are of type object.




### How do you create an array of objects in Java?

1. public class ArrayOfObjects.
`{`
2. public static void `main(String args[])`
`{`
3. //create an array of product object.
4. `Product[]` `obj = new Product[5]` ;
5. //create & initialize actual product objects using constructor.
6. obj`[0]` = new Product(23907,"Dell Laptop")


![dvsdss](https://i2.wp.com/javaconceptoftheday.com/wp-content/uploads/2014/11/ArrayOfObjects.png?w=1200.jpg)



------------------------------------------------------------------------------------------------------------------------------------------------




## THE BROWSER OBJECT MODEL: THE WINDOW OBJECT
![dffdgdg](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSUMDMetAHhXisNoGYNTMA9YBDXAu7L63yPtPzk52lfA5bZk9kJS3xUr5UcHkfmFhujzTA&usqp=CAU.jpg)



### What is browser window object?
>The window object represents an open window in a browser. If a document contain frames (`<iframe> tags`), the browser creates one window object for the HTML document, and one additional window object for each frame.

### What is the window object in JavaScript?

The window object is a global object that has the properties pertaining to the current DOM document, which is what's in the tab of a browser. The document property of the window object has the DOM document and associated nodes and methods that we can use to manipulate the DOM nodes and listen to events for each node.

### What is BOM and Dom?

>The BOM (Browser Object Model) consists of the objects navigator , history , screen , location and document which are children of window . In the document node is the DOM (Document Object Model), the document object model, which represents the contents of the page.١١‏/١٢‏/٢٠١٠



### What are different types of window objects?
> that are different types of window objects?
> The javascript objects are string, array, date etc..

### Methods of window object.
-|-
-|-
Method|	Description
confirm()|	displays the confirm dialog box containing message with ok and cancel button.
prompt()|	displays a dialog box to get input from the user.
open()|	opens the new window.
close()|	closes the current window.

### What is alert () method?
#### The alert() method displays an alert box with a specified message and an OK button. An alert box is often used if you want to make sure information comes through to the user. ... Do not overuse this method, as it prevents the user from accessing other parts of the page until the box is closed.


------------------------------------------------------------------------------------------------------------------------------------------------

## USING THE DOCUMENT  OBJECT


### What does document object mean?

>The Document Object Model (DOM) is a programming interface for HTML and XML documents. ... The Document Object Model (DOM) represents that same document so it can be manipulated. The DOM is an object-oriented representation of the web page, which can be modified with a scripting language such as JavaScript.‏


### What is the use of document object in JavaScript?

>A Document object represents the HTML document that is displayed in that window. The Document object has various properties that refer to other objects which allow access to and modification of document content. The way a document content is accessed and modified is called the Document Object Model, or DOM.

### What are the valid methods of document object?
> Document Object Properties and Methods
-|-
-|-
PropertyMethod	| Description
title |	Sets or returns the title of the document
URL |	Returns the full URL of the HTML document
write() |	Writes HTML expressions or JavaScript code to a document
writeln() |	Same as write(), but adds a newline character after each statement


### How can document object be used to access form elements?

> The Form Object in HTML DOM is used to represent the HTML < form > element. This tag is used to set or get the properties of < form > element. This element can be accessed by using `getElementById() method`.


### What is meant by document object model?
>Introduction. The Document Object Model (DOM) is a programming API for HTML and XML documents. It defines the logical structure of documents and the way a document is accessed and manipulated. ... The Document Object Model can be used with any programming language.
>HTML: `<object>` tag. This HTML tutorial explains how to use the HTML element called the `<object>` tag with syntax and examples.


## GLOBAL OBJECTS: 
![dfsdfssf](https://res.cloudinary.com/practicaldev/image/fetch/s--jRLu_Z5j--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://dev-to-uploads.s3.amazonaws.com/i/q6pyi9z2qpt9iai9foqx.png)

## What is a global object?

> A global object is an object that always exists in the global scope. ... The global object's interface depends on the execution context in which the script is running. For example: In a web browser, any code which the script doesn't specifically start up as a background task has a Window as its global object.

## Is console a global object?

> According the the Node documentation, the console object is a global that has a few methods allowing developers to do things such as printing a log or an error. Digging deeper into the docs we can see that console is really a global instance that is configured to write to process. stdout and process. stderr .

## What is the global object in client side JavaScript?

> The global object in JavaScript is an always defined object that provides variables and functions, and is available anywhere. In a web browser, the global object is the window object, while it is named global in Node. js. The global object can be accessed using the this operator in the global scope.

## Why code written in node JS is pretty fast?

> Being built on Google Chrome's V8 JavaScript Engine, Node. js library is very fast in code execution. ... B - Node based server uses a single threaded model and can services much larger number of requests than traditional server like Apache HTTP Server.

## How node JS overcomes the problem of blocking of I O operations?

> A. By putting the event-based model at its core and using an event loop instead of threads, Node. js overcomes the problem of blocking I/O operations.

## CREATING A DATE OBJECT 

### How do you create a date object?

> To create a date, we can use the datetime() class (constructor) of the datetime module. The datetime() class requires three parameters to create a date: year, month, day.

### What is Type Date?

> <`input type="date">` `<input>` elements of type="date" create input fields that let the user enter a date, either with a textbox that validates the input or a special date picker interface. ... The time and datetime-local input types support time and date+time input

### What is date and time called?

>  Loading when this answer was accepted… Though perhaps awkward in some contexts, timestamp does fit your desired meaning. The date and time at which an event occurs or occurred, usually indicated in human-readable form, especially when used in a log to track events.


-----------------------------------------------------


## HOW MEMORY & VARIABLES WORK
> In JavaScript, when we create variables, functions, or anything you can think of, the JS engine allocates memory for this and releases it once it's not needed anymore. Allocating memory is the process of reserving space in memory, while releasing memory frees up space, ready to be used for another purpose.


### How are variables stored in memory?
![dsfddsgdg](https://miro.medium.com/max/2048/1*qY-yRQWGI-DLS3zRHYHm9A.png)

> Most variables stored in the array (i.e., in main memory) are larger than one byte, so the address of each variable is the index of the first byte of that variable. Viewing main memory as an array of bytes. ... An address is equivalent to an index into the memory array. Most C++ data types span multiple bytes of memory.


##### A Memory leak can be defined as a piece of memory that is no longer being used or required by an application but for some reason is not returned back to the OS and is still being occupied needlessly. ... A Javascript memory leak occurs when you may no longer need an object but the JS runtime still thinks you do.

##### In JavaScript, memory is automatically allocated each time you create, for instance, an object, an array, a string, or a DOM element. ... A sawtooth pattern with these vertical drops coinciding with garbage collection may also indicate a memory leak. Memory leaks can assume many shapes and forms, though.

### How does JavaScript memory management work?

> These primitives are used by the developer to explicitly allocate and free memory from and to the operating system. At the same time, JavaScript allocates memory when things (objects, strings, etc.) are created and “automatically” frees it up when they are not used anymore, a process called garbage collection.

### How are variables stored in memory JavaScript?


> Variables in JavaScript (and most other programming languages) are stored in two places: stack and heap. A stack is usually a continuous region of memory allocating local context for each executing function. ... Even if a function calls itself recursively, each frame has its own copy of all local variables.




-----------------------------------------------------



## CREATING· OBJECTS USING LITERAL NOTATION 


### What is object literal notation of JavaScript?


> The Object literal notation is basically an array of key:value pairs, with a colon separating the keys and values, and a comma after every key:value pair, except for the last, just like a regular array. Values created with anonymous functions are methods of your object.



### How do you make an object literal?

> Object literals are defined using the following syntax rules:

1. A colon separates property name`[1]` from value.
2. A comma separates each name-value pair from the next.
3. A comma after the last name-value pair is optional. `[2]`


### Do we have classes in JavaScript?


> In JavaScript, there are no classes in the class-based OOP sense of the word. JavaScript works with objects. If you want to encapsulate a few functions and properties together, you would create an object containing functions and properties, and not a class. ... JavaScript doesn't have blueprints, it only has houses.


###### Computed properties allow you to dynamically choose what property in your object gets updated. It's important to give your input element a name attribute. The name attribute that you specify should match the property that you wish to update within the object. Retrieve the name and value from even‏.


#### Object Types (Blueprints) (Classes)
> They only create single objects. Sometimes we need a "blueprint" for creating many objects of the same "type". The way to create an "object type", is to use an object constructor function. In the example above, function Person() is an object constructor function.


-------------------------------------------------------------------------------------------------------------------------------------------------

## ADDING AND REMOVING PROPERTIES 
#### Remove Property from an Object
>The delete operator deletes a property from an object:

### Example
<!-- ~var person = {
  firstName:"John",
  lastName:"Doe",
  age:50,
  eyeColor:"blue"
};~ -->

> delete person.age;  // or delete person["age"];

> // Before deletion: person.age = 50, after deletion, >person.age = undefined
#### The delete operator deletes both the value of the property and the property itself.

#### After deletion, the property cannot be used before it is added back again.

#### The delete operator is designed to be used on object properties. It has no effect on variables or functions.

> Note: The delete operator should not be used on predefined JavaScript object properties. It can crash your application

## RECAP: WAYS TO CREATE OBJECTS


#### In JS there are two main ways in which you can create an object:

1. Object Literal Notation
2. Object Constructor Notation

### Object Literal Notation (OLN)

> Literal notation is the easiest and most popular way to create objects.



 

### Object Constructor Notation (OCN)



> Sometimes you will want several objects to represent similar things. As shown above, object constructors can use a function as a template for creating objects First, you have to create the template with the object’s properties and methods.

##### You can then create instances of the object using the constructor function, as shown above. The new keyword followed by a call to the function creates a new object. The properties of each object are given as arguments to the function.

And that’s how you create objects in JavaScript!



-----------------------------------------------------


## MATH OBJECT TO CREATE RANDOM NUMBERS

### What is used to generate random digits?

> To generate “true” random numbers, random number generators gather “entropy,” or seemingly random data from the physical world around them. For random numbers that don't really need to be random, they may just use an algorithm and a seed value.

### Is it possible to generate a random number?


> Even though a computer is absolutely unable to create a random number, it is good at introducing too many variables to predict! Generating truly random numbers in software is indeed not possible as others have pointed out, however it is possible with hardware to build a device which can generate truly random numbers*.

### How do you create a random number in JavaScript?

> In JavaScript, to get a random number between 0 and 1, use the Math. random() function. If you want a random number between 1 and 10, multiply the results of Math. random by 10, then round up or down.

### Is random math random JavaScript?

> JavaScript doesn't decide how Math. ... [Math. random] Returns a Number value with positive sign, greater than or equal to 0 but less than 1, chosen randomly or pseudo randomly with approximately uniform distribution over that range, using an implementation-dependent algorithm or strategy. This function takes no arguments.


## CREATING A DATE OBJECT 

#### how will you create a new date object in JavaScript?

> No Argument − With no arguments, the Date() constructor creates a Date object set to the current date and time.
> milliseconds − When one numeric argument is passed, it is taken as the internal numeric representation of the date in milliseconds, as returned by the `getTime()`



### how do I format a date in JavaScript?
> The date-string method
1. YYYY : 4-digit year.
2. MM : 2-digit month (where January is 01 and December is 12)
3. DD : 2-digit date (0 to 31)
4. - : Date delimiters.
5. T : Indicates the start of time.
6. HH : 24-digit hour (0 to 23)
7. mm : Minutes (0 to 59)

![ssdfsdfs](https://www.w3resource.com/w3r_images/js-date-object-setseconds.gif)




