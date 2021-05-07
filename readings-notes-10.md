
# JS REVIEW 
![javascript](https://safeonline.najah.edu/media/filer_public_thumbnails/filer_public/fa/05/fa05716d-b124-4264-ba5b-2519f3ef2581/shhr_wqw_nw_lkhtrqt_n_tryq_ljf_skrbt_javascript.jpg__1200x675_q85_crop_subsampling-2_upscale.jpg)

# ERROR HANDLING & DEBUGGING 

## ORDER OF EXECUTION

 > To find the source of an error, it helps to know how  scripts  are processed. The order in which statements are executed can be complex; some tasks cannot complete until another statement or function has been run.

 ##  EXECUTION CONTEXTS

 > The JavaScript interpreter uses the concept of execution contexts. There is one global execution context; plus, each function creates a new new execution context. They correspond to variable scope. 

### EXECUTION CONTEXT 
##### Every statement in a script lives in one of three execution contexts:

* ##### GLOBAL CONTEXT 
##### Code that is in the script, but not in a function. 
##### There is only one global context in any page. 
* ##### FUNCTION CONTEXT 
##### Code that is being run within a function. 
##### Each function has its own function context. 
* ##### EVAL CONTEXT (NOT SHOWN)    
##### Text is executed like code in an internal function 
##### called eva l {) (which is not covered in this book). 

### VARIABLE SCOPE 
##### The first two execution contexts correspond with the notion of scope : 
* ##### GLOBAL SCOPE 
##### If a variable is declared outside a function, it can 
##### be used anywhere because it has global scope. 
##### If you do not use the var keyword when creating 
##### a variable, it is placed in global scope. 
* ##### FUNCTION-LEVEL SCOPE 
##### When a variable is declared within a function, 
##### it can only be used within that function. This is 
##### because it has function-level scope. 

##  EXECUTION CONTEXT & HOISTING

> Each time a script enters a new execution context, there are two phases of activity:

### 1. Prepare
##### • The new scope is created 
##### • Variables, functions, and arguments are created 
##### • The value of the this keyword is determined 
### 2. Execute 
##### • Now it can assign values to variables 
##### • Reference functions and run their code 
##### • Execute statements 


* ##### Understanding that these two phases happen helps with understanding a concept called hoisting. You may have seen that you can: 
##### • Call functions before they have been declared (if they were created using function declarations - not function expressions, see p96) 
##### • Assign a value to a variable that has not yet been declared 
##### This is because any variables and functions within each execution context are created before they are executed. 
##### The preparation phase is often described as taking all of the variables and functions and hoisting them to the top of the execution context. Or you can think of them as having been prepared. 
##### Each execution context also creates its own vari ab 1 es object. This object contains details of all of the variables, functions, and parameters for that execution context. 

## UNDERSTANDING SCOPE

![understanding](https://i1.wp.com/www.welovejs.com/wp-content/uploads/2020/05/chris-ried-ieic5Tq8YMk-unsplash-1.jpg?resize=950%2C500&ssl=1.jpg)

 ### In the interpreter, each execution context has its own variables object. 
> It holds the variables, functions, and parameters available within it. 
>Each execution context can also access its parent's variables object. 
 
 ##### Functions in JavaScript are said to have lexical scope. They are linked to the object they were defined within. So, for each execution context, the scope is the current execution context's variables object, plus the variables object for each parent execution context. Imagine that each function is a nesting doll. The children can ask the parents for information in their variables. But the parents cannot get variables from their children. Each child will get the same answer from the same parent. 

##### If a variable is not found in the variables object for the current execution context, it can look in the variables object of the parent execution context. But it is worth knowing that looking further up the stack can affect performance, so ideally you create variables inside the functions that use them. 
##### If you look at the example on the left, the inner functions can access the outer functions and their variables. For example, the greetUser() function can access the time variable that was declared in the outer greeting() function. 
##### Each time a function is called, it gets its own execution context and variables object. 
##### Each time an outer function calls an inner function, the inner function can have a new variables object. But variables in the outer function remain the same. 

##  UNDERSTANDING ERRORS

> If a JavaScript statement generates an error, then it throws an exception. At that point, the interpreter stops and looks for exception-handl ing code. 

##### If you are anticipating that something in your code may cause an error, you can use a set of statements to handle the error. This is important because if the error is not handled, the script will just stop processing and the user will not know why. So exception-handling code should inform users when there is a problem. 

## ERROR OBJECTS 

> Error objects can help you find where your mistakes are and browsers have tools to help you read them.

##### there are seven types of built-in error objects in JavaScript.

Object | Descrition 
-|-
Error | Generic error - the other errors are all based upon this error
Syntax Error | Syntax has not been followed
Reference Error | Tried to reference a variable that is not declared/within scope
TypeError | An unexpected data type that cannot be coerced 
Range Error | Numbers not in acceptable range 
URI Error | encodeURI ().decodeURI(),and similar methods used incorrectly 
EvalError | eva l () function used incorrectly 


##  HOW TO DEAL WITH ERRORS
> Now that you know what an error is and how the browser treats them, there are two things you can do with the errors. 
### 1: DEBUG THE SCRIPT TO FIX ERRORS 
#### If you come across an error while writing a script (or when someone reports a bug), you will need to debug the code, track down the source of the error, and fix it. 
#### You will find that the developer tools available in every major modern browser will help you with this task. In this chapter, you will learn about the developer tools in Chrome and Firefox. (The tools in Chrome are identical to those in Opera.) 
#### IE and Safari also have their own tools (but there is not space to cover them all).  
### 2: HANDLE ERRORS GRACEFULLY 
#### You can handle errors gracefully using try, catch, throw, and finally statements. 
#### Sometimes, an error may occur in the script for a reason beyond your control. For example, you might request data from a third party, and their server may not respond. In such cases, it is particularly important to write error-handling code. 
 #### In the latter part of the chapter, you will learn how to gracefully check whether something will work, and offer an alternative option if it fails.  

## A DEBUGGING WORKFLOW

> Debugging is about deduction: eliminating potential causes of an error. 
Here is a workflow for techniques you will meet over the next 20 pages. 
Try to narrow down where the problem might be, then look for clues.

### WHERE IS THE PROBLEM? 
 #### First, should try to can narrow down the area where the problem seems to be. In a long script, this is especially important. 
#### 1. Look at the error message, it tells you: 
#### • The relevant script that caused the problem. 
#### • The line number where it became a problem for the interpreter. (As you will see, the cause of the error may be earlier in a script; but this is the point at which the script could not continue.) 
#### • The type of error (although the underlying cause of the error may be different). 
#### 2. Check how far the script is running. Use tools to write messages to the console to tell how far your script has executed. 
#### 3. Use breakpoints where things are going wrong. They let you pause execution and inspect the values that are stored in variables. 
#### If you are stuck on an error, many programmers 
#### suggest that you try to describe the situation (talking out loud) to another programmer. Explain what should be happening and where the error appears to be happening. This seems to be an effective way of finding errors in all programming languages. (If nobody else is available, try describing it to yourself.) 


### WHAT EXACTLY IS THE PROBLEM? 
#### Once you think that you might know the rough area in which your problem is located, you can then try to find the actual line of code that is causing the error. 
#### 1. When you have set breakpoints, you can see if the variables around them have the values you would expect them to. If not, look earlier in the script. 
#### 2. Break down I break out parts of the code to test smaller pieces of the functionality. 
#### • Write values of variables into the console. 
#### • Calrfunctions from the console to check if they are returning what you would expect them to. 
#### • Check if objects exist and have the methods I properties that you think they do. 
#### 3. Check the number of parameters for a function, or the number of items in an array. 
#### And be prepared to repeat the whole process if the above solved one error just to uncover another .. 
- ####  If the problem is hard to find, it is easy to lose track of what you have and have not tested. Therefore, when you start debugging, keep notes of what you have tested and what the result was. No matter how stressful the circumstances  are, if you can, stay calm and methodical, the problem will feel less overwhelming and you will solve it faster.


## BROWSER DEV TOOLS & JAVASCRIPT CONSOLE 

> The JavaScript console will tell you when there is a problem with a script, 
where to look for the problem, and what kind of issue it seems to be. 

### CHROME/ OPERA 
#### On a PC, press the F12 key or: 
#### 1. Go to the options menu (or three line menu icon) 
#### 2. Select Toots or More tools. 
#### 3. Select JavaScript Console or Developer Tools 
#### On a Mac press Alt + Cmd + J. Or: 
#### 4. Go to the View menu. 
#### 5. Select Developer. 
#### 6. Open the JavaScript Console or Developer Tools option and select Console. 
### INTERNET EXPLORER 
#### Press the F12 key or: 
#### 1. Go to the settings menu in the top-right. 
#### 2. Select developer tools.

### FIREFOX 
### On a PC, press Ctrl + Shift + Kor: 
#### 1. Go to the Firefox menu. 
#### 2. Select Web Developer. 
#### 3. Open the Web Console. 
#### On a Mac press Alt + Cmd + K. Or: 
#### 1. Go to the Tools menu. 
#### 2. Select Web Developer. 
#### 3. Open the Web Console. 
### SAFARI 
#### Press Alt + Cmd + C or: 
#### 1. Go to the Develop menu. 
#### 2. Select Show Error Console. 
#### If the Develop menu is not shown: 
#### 1. Go to the Safari menu. 
#### 2. Select Preferences. 
#### 3. Select Advanced. 
#### 4. Check the box that says "Show Develop menu in menu bar." 
 
## HOW TO LOOK AT ERRORS IN FIREFOX

> 1. The Console option is selected. 
> 2. Only the JavaScript and 
Logging options need to be 
turned on. The Net, CSS, and 
Security options show other 
information. 
> 3. The type of error and the error 
message are shown on the left. 
> 4. On the right-hand side of the 
console, you can see the name 
of the JavaScript file and the line 
number of the error. 


