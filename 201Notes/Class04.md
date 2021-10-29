# Code 201 Class 04 Reading notes:

## JavaScript :

### FUNCTIONS & METHODS:

**JavaScript Methods:** A JavaScript method is a property of an object that contains a function definition. Methods are functions stored as object properties. Object method can be accessed with the following syntax:

Syntax:

object = {
    methodName: function() {
        // Content
    }
};

object.methodName()

**JavaScript Functions:** A function is a block of code written to perform some specific set of tasks. We can define a function using the function keyword, followed by Name and optional parameters. Body of function is enclosed in Curly braces.
Functions let you group a series of statements together to perform a
specific task. If different parts of a script repeat the same task, you can
reuse the function (rather than repeating the same set of st atements).
Syntax: 

function functionName(parameters) {
    // Content
}

**Function Return**
When JavaScript reaches a return statement, the function will stop executing.

If the function was invoked from a statement, JavaScript will "return" to execute the code after the invoking statement.

Functions often compute a return value. The return value is "returned" back to the "caller":

Example
Calculate the product of two numbers, and return the result:

let x = myFunction(4, 3);   // Function is called, return value will end up in x

function myFunction(a, b) {
  return a * b;             // Function returns the product of a and b
}
The result in x will be:

12

**JavaScript Objects:**

JavaScript variables are containers for data values, objects are variables too, But objects can contain many values.

**Pair programming:**

Two roles: the Driver and the Navigator. 
- *The Driver* is the programmer who is typing and the only one whose hands are on the keyboard. Handling the “mechanics” of coding, the Driver manages the text editor, switching files, version control, and—of course writing—code. 

- *The Navigator* uses their words to guide the Driver but does not provide any direct input to the computer. The Navigator thinks about the big picture, what comes next, how an algorithm might be converted in to code, while scanning for typos or bugs. The Navigator might also utilize their computer as a second screen to look up solutions and documentation, but should not be writing any code.

## HTML & CSS:

### Links:

Links are the defining feature of the web because they allow you to move from one web page to another — enabling the very idea of browsing or surfing.

Links are created using the < a> element. Users can click on anything
between the opening < a> tag and the closing < /a> tag. You specify
which page you want to link to using the href attribute.
Writing Links
< a href="http://www.imdb.com">IMDB< /a >

**Summary**

- Links are created using the <a> element.
- The <a> element uses the href attribute to indicate
the page you are linking to.
-  If you are linking to a page within your own site, it is
best to use relative links rather than qualified URLs.
-  You can create links to open email programs with an
email address in the "to" field.
-  You can use the id attribute to target elements within
a page that can be linked to.

### CSS Layouts:
Controls where each element sits on a page and how to create attractive page layouts.

- Different ways to position elements using normal
flow, relative positioning, absolute positioning and floats.
- Various devices have different screen sizes
and resolution, and how this affects the design process.
- Difference between fixed width and liquid layouts,
and how they are created.
- Use grids to make page designs look more professional.


**Block-level boxes** start on a new line and act as the main building blocks
of any layout, **while inline boxes** flow between surrounding text. You can
control how much space each box takes up by setting the width of the
boxes (and sometimes the height, too). 

To separate boxes, you can use
borders, margins, padding, and background colors.

Block-level elements start on a new line.

Examples include:

< h1> < p> < ul> < li>

Inline elements flow in between surrounding text.
Examples include:

< img> < b> < i>

**Containing Elements**

If one block-level element sits inside another block-level element then the outer box is known as the containing or parent element.

**Controlling the Position of Elements**

CSS has the following positioning schemes that allow you to control the layout of a page: **normal flow, relative positioning, and absolute positioning** . 

You specify the positioning scheme using the position property in CSS. You can also float elements using the float property.


#### Want To Know More ? 
[Visit our Resources website](https://www.w3schools.com)
OR
[Books](https://www.wiley.com/en-us/Web+Design+with+HTML%2C+CSS%2C+JavaScript+and+jQuery+Set-p-9781119038634)