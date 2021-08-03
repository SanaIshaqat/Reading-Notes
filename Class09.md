# Code 201 Class 09 Reading notes:

## JavaScript:

### Events:

HTML events are "things" that happen to HTML elements.

When JavaScript is used in HTML pages, JavaScript can "react" on these events.

**HTML Events**
An HTML event can be something the browser does, or something a user does.

Here are some examples of HTML events:

An HTML web page has finished loading
An HTML input field was changed
An HTML button was clicked
Often, when events happen, you may want to do something.

**JavaScript lets you execute code when events are detected.**

HTML allows event handler attributes, with JavaScript code, to be added to HTML elements.

With single quotes:

< element event='some JavaScript'>
With double quotes:

< element event="some JavaScript">
In the following example, an onclick attribute (with code), is added to a < button> element:

**Example**
< button onclick="document.getElementById('demo').innerHTML = Date()">The time is?< /button>
In the example above, the JavaScript code changes the content of the element with id="demo".

In the next example, the code changes the content of its own element (using this.innerHTML):

**Example**
< button onclick="this.innerHTML = Date()">The time is?< /button>
JavaScript code is often several lines long. It is more common to see event attributes calling functions:

**Example**
< button onclick="displayDate()">The time is?< /button>

**JavaScript event flow model**
Event flow is when a node triggers an event, the event will flow from the current node to other nodes
According to the direction of event flow, the event flow model can be divided into event bubbling and event capturing
Based on the event bubbling, a new binding method was born, "event delegation"

![Illustration](https://www.programmersought.com/images/827/58af504b81d1e0ded491fcedf16fc8bb.JPEG)


### Events Summary:

* Events are the browser's way of indicating when
something has happened (such as when a page has
finished loading or a button has been clicked).


* Binding is the process of stating which event you are
waiting to happen, and which element you are waiting
for that event to happen upon.


* When an event occurs on an element, it can trigger a
JavaScript function. When this function then changes
the web page in some way, it feels interactive because
it has responded to the user.


* You can use event delegation to monitor for events
that happen on all of the children of an element.


* The most commonly used events are W3C DOM
events, although there are others in the HTMLS
specification as well as browser-specific events.


## HTML:

### Forms:
A form may have several form controls, each
gathering different information. The server
needs to know which piece of inputted data
corresponds with which form element.

* Whenever you want to collect information from
visitors you will need a form, which lives inside a
< form> element.

* Information from a form is sent in name/value pairs.

* Each form control is given a name, and the text the
user types in or the values of the options they select
are sent to the server.

* HTML5 introduces new form elements which make it
easier for visitors to fill in forms.


## CSS:

### Lists, Tables, Forms:

Specifying bullet point styles
Adding borders and backgrounds to tables
Changing the appearance of form elements
There are several CSS properties that were created to work with specific types of HTML elements, such as lists, tables, and forms.


Specify the type of bullet point or numbering on lists
Add borders and backgrounds to table cells
Control the appearance of form controls
Together, these properties allow you to take finer control over specific parts of your pages.

**Examples:**

1. List Style Type
2. List Style Image
3. List Style Position
4. List Style Shorthand
5. Table Properties
6. Empty Cells
7. Gaps Between Cells
8. Styling Text Inputs
9. Styling Submit Buttons
10. Styling Fieldsets and Legends
11. Aligning Form Controls: Problem
12. Aligning Form Controls: Solution
13. Cursor

**Summary:**

* In addition to the CSS properties covered in other
chapters which work with the contents of all elements,
there are several others that are specifically used to
control the appearance of lists, tables, and forms.

* List markers can be given different appearances
using the list-style-type and list-style image
properties.

* Table cells can have different borders and spacing in
different browsers, but there are properties you can
use to control them and make them more consistent.

* Forms are easier to use if the form controls are
vertically aligned using CSS.

* Forms benefit from styles that make them feel more
interactive.




#### Want To Know More ? 
[Code Samples:](http://www.htmlandcssbook.com/code-samples/chapter-14/)
[Visit our Resources website](https://www.w3schools.com)
OR
[Books](https://www.wiley.com/en-us/Web+Design+with+HTML%2C+CSS%2C+JavaScript+and+jQuery+Set-p-9781119038634)