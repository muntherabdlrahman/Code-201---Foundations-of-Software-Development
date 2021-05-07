# HTML CSS REVIEW

## TABLES
## Old Code : Width & Spacing


* There are some outdated 
attributes which you should not 
use on new websites. You may, 
however, come across some 
of them when looking at older 
code, so I will mention them 
here. All of these attributes have 
been replaced by the use of CSS.

* The width attribute was used 
on the opening `<table>` tag to 
indicate how wide that table 
should be and on some opening 
`<th>` and `<td>` tags to specify 
the width of individual cells. 
The value of this attribute is 
the width of the table or cell in 
pixels.

* The columns in a table need to 
form a straight line, so you often 
only see the width attribute on 
the first row (and all subsequent 
rows would use that setting).

* The opening `<table>` tag could 
also use the cellpadding
attribute to add space inside 
each cell of the table, and the 
cellspacing attribute to create 
space between each cell of 
the table. The values for these 
attributes were given in pixels.

## Old Code : Border & Background

* The border attribute was used 
on both the `<table>` and `<td>`
elements to indicate the width of 
the border in pixels.

* The bgcolor attribute was used 
to indicate background colors 
of either the entire table or 
individual table cells. The value 
is usually a hex code.
 
* When building a new website 
you should use CSS to control 
the appearance of the table 
rather than these attributes. 
They are only covered here 
because you may come across 
them if you look at the code of 
older websites

## Summary :

> * The `<table>` element is used to add tables to a web 
page.
>* A table is drawn out row by row. Each row is created 
with the `<tr>` element.
>* Inside each row there are a number of cells 
represented by the `<td>` element (or `<th>` if it is a 
header).
>* You can make cells of a table span more than one row 
or column using the rowspan and colspan attributes.
>* For long tables you can split the table into a `<thead>`, 
`<tbody>`, and `<tfoot>`.

## FORMS :

### Why Forms?

form is a structured document with a fixed arrangement. Forms are used to collect the required information in a logical, meaningful fashion for communication and pass to another entity. When you picture what a form is, you can conjure many different types of documents


## Form Controls :

There are several types of form controls that 
you can use to collect information from visitors to your site.

* ADDING TEXT :

• Text input (single-line)
Used for a single line of text such 
as email addresses and names.
 
• Password input :
Like a single line text box but it 
masks the characters entered.

• Text area (multi-line) :
For longer areas of text, such as 
messages and comments.

* Making Choices:

• Radio buttons :
For use when a user must select 
one of a number of options.

• Checkboxes :
When a user can select and 
unselect one or more options.

• Drop-down boxes :
When a user must pick one of a 
number of options from a list.

* Submitting Forms:

• Submit buttons :
To submit data from your form 
to another web page.

• Image buttons :
Similar to submit buttons but 
they allow you to use an image.

* Uploading Files:

• File upload :
Allows users to upload files 
(e.g. images) to a website.


## How Forms Work

> * A user fills in a form and then presses a button to submit the information to the server.
> * The name of each form control is sent to the server along with the value the user enters or selects.
> * The server processes the information using a programming language such as PHP, C#, or Java. It may also store the information in a database.
> * The server creates a new page to send back to the browser based on the information received.

• A form may have several form controls, each 
gathering different information. The server 
needs to know which piece of inputted data 
corresponds with which form element.


## Form Structure :

## `<form>` :

• Form controls live inside a 
`<form>` element. This element 
should always carry the action
attribute and will usually have a 
method and id attribute too.

* action :

• Every `<form>` element requires 
an action attribute. Its value
is the URL for the page on the 
server that will receive the 
information in the form when it 
is submitted.

* method :

• Forms can be sent using one of 
two methods: get or post.

• With the get method, the values 
from the form are added to 
the end of the URL specified in 
the action attribute. The get
method is ideal for:

1. short forms (such as search 
boxes) 

2. when you are just retrieving 
data from the web server 
(not sending information that 
should be added to or deleted 
from a database)


• With the post method the 
values are sent in what are 
known as HTTP headers. As a 
rule of thumb you should use the 
post method if your form:

1. allows users to upload a file

2. is very long

3. contains sensitive data 
(e.g. passwords)

4. adds information to, or 
deletes information from, a 
database

## Text Input :

## `<input>` :

> The `<input>` element is used 
to create several different form 
controls. The value of the type
attribute determines what kind 
of input they will be creating.

• type="text" 

When the type attribute has a 
value of text, it creates a single-line text input.

 name :

When users enter information 
into a form, the server needs to 
know which form control each 
piece of data was entered into. 
(For example, in a login form, the 
server needs to know what has 
been entered as the username 
and what has been given as the 
password.) Therefore, each form 
control requires a name attribute. 
The value of this attribute 
identifies the form control and is 
sent along with the information 
they enter to the server.

• maxlength : 

You can use the maxlength
attribute to limit the number 
of characters a user may enter 
into the text field. Its value is the 
number of characters they may 
enter. For example, if you were 
asking for a year, the maxlength
attribute could have a value of 4

• size :

The size attribute should not 
be used on new forms. It was 
used in older forms to indicate 
the width of the text input 
(measured by the number of 
characters that would be seen). 

For example, a value of 3 would 
create a box wide enough to 
display three characters 
(although a user could enter 
more characters if they desired).

In any new forms you write, 
CSS should be used to control 
the width of form elements. 
The size attribute is only 
mentioned here because you 
may come across it when looking 
at older code.

## Password Input :

## `<input>` :

• type="password" 

When the type attribute has 
a value of password it creates 
a text box that acts just like a 
single-line text input, except 
the characters are blocked out. 
They are hidden in this way so 
that if someone is looking over 
the user's shoulder, they cannot 
see sensitive data such as 
passwords.

• name :

The name attribute indicates 
the name of the password input, 
which is sent to the server with 
the password the user enters.

• size, maxlength :

It can also carry the size and 
maxlength attributes like the 
the single-line text input.

## Text Area :

## `<textarea>` :

* The `<textarea>` element 
is used to create a mutli-line 
text input. Unlike other input 
elements this is not an empty 
element. It should therefore have 
an opening and a closing tag.

* Any text that appears between 
the opening `<textarea>` and 
closing `</textarea>` tags will 
appear in the text box when the 
page loads.

* If the user does not delete any 
text between these tags, this 
message will get sent to the 
server along with whatever the 
user has typed. (Some sites 
use JavaScript to clear this 
information when the user clicks 
in the text area.)

## Radio Button :


## `<input>` :

• type="radio" 

Radio buttons allow users to pick 
just one of a number of options.

• name :

The name attribute is sent to 
the server with the value of the 
option the user selects. When 
a question provides users with 
options for answers in the form 
of radio buttons, the value of 
the name attribute should be the 
same for all of the radio buttons 
used to answer that question.

• value :

The value attribute indicates 
the value that is sent to the 
server for the selected option. 
The value of each of the buttons 
in a group should be different 
(so that the server knows which 
option the user has selected).

• checked :

The checked attribute can be 
used to indicate which value (if 
any) should be selected when 
the page loads. The value of this 
attribute is checked. Only one 
radio button in a group should 
use this attribute.

## CheckBox :

## `<input>` :
 
• type="checkbox" 

Checkboxes allow users to select 
(and unselect) one or more 
options in answer to a question.

• name :

The name attribute is sent to 
the server with the value of the 
option(s) the user selects. When 
a question provides users with 
options for answers in the form 
of checkboxes, the value of the 
name attribute should be the 
same for all of the buttons that 
answer that question.

• value :

The value attribute indicates 
the value sent to the server if this 
checkbox is checked.

• checked :

The checked attribute indicates 
that this box should be checked 
when the page loads. If used, its 
value should be checked.

## Drop Down List Box :

## `<select>` :

A drop down list box (also 
known as a select box) allows 
users to select one option from a 
drop down list.

The `<select>` element is used 
to create a drop down list box. It 
contains two or more `<option>`
elements. 

• name :
The name attribute indicates the 
name of the form control being 
sent to the server, along with the 
value the user selected.

 ## `<option>` :

The `<option>` element is used 
to specify the options that the 
user can select from. The words 
between the opening `<option>`
and closing `</option>` tags will 
be shown to the user in the drop 
down box.

• value :

The `<option>` element uses the 
value attribute to indicate the 
value that is sent to the server 
along with the name of the 
control if this option is selected.

• selected :

The selected attribute can be 
used to indicate the option that 
should be selected when the 
page loads. The value of this 
attribute should be selected.

If this attribute is not used, 
the first option will be shown 
when the page loads. If the user 
does not select an option, then 
the first item will be sent to 
the server as the value for this 
control.

The function of the drop down 
list box is similar to that of the 
radio buttons (in that only one 
option can be selected). There 
are two key factors in choosing 
which to use:

1. If users need to see all options 
at a glance, radio buttons are 
better suited.
2. If there is a very long list 
of options (such as a list of 
countries), drop down list boxes 
work better.

## Multiple Sekect Box 

## `<select>`

• size :

You can turn a drop down select 
box into a box that shows more 
than one option by adding the 
size attribute. Its value should 
be the number of options you 
want to show at once. In the 
example you can see that three 
of the four options are shown.

Unfortunately, the way that 
browsers have implemented this 
attribute is not perfect, and it 
should be tested throroughly if 
used (in particular in Firefox and 
Safari on a Mac).

• multiple :

You can allow users to select 
multiple options from this list by 
adding the multiple attribute 
with a value of multiple.

It is a good idea to tell users if 
they can select more than one 
option at a time. It is also helpful 
to indicate that on a PC they 
should hold down the control key 
while selecting multiple options 
and on a Mac they should use 
the command key while selecting 
options.

## File Input Box 

## `<input>` :

If you want to allow users to 
upload a file (for example an 
image, video, mp3, or a PDF), 
you will need to use a file input 
box.

• type="file" 

This type of input creates a 
box that looks like a text input 
followed by a browse button. 
When the user clicks on the 
browse button, a window opens 
up that allows them to select a 
file from their computer to be 
uploaded to the website. 

When you are allowing users 
to upload files, the method
attribute on the `<form>` element 
must have a value of post. (You 
cannot send files using the HTTP 
get method.)

When a user clicks on the 
browse button, the presentation 
of the window that allows 
them to browse for the file they 
want to upload will match the 
windows of the user's operating 
system. You cannot control the 
appearance of these windows.

## Submit Button 

## `<input>`
• type="submit" 

The submit button is used to 
send a form to the server.
name
It can use a name attribute but it 
does not need to have one.

• value :

The value attribute is used to 
control the text that appears 
on a button. It is a good idea to 
specify the words you want to 
appear on a button because the 
default value of buttons on some 
browsers is ‘Submit query’ and 
this might not be appropriate for 
all kinds of form.

Different browsers will show 
submit buttons in different 
ways and tend to fit the visual 
presentation of the browser. 
If you want to control the 
appearance of a submit button, 
you can either use CSS (as you 
will learn on page 343), or you 
can use an image for the button.







