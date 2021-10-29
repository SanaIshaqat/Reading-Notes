# Code 201 Class 06 Reading notes:

## JavaScript :

### Objects:

Objects can be initialized using new Object(), Object.create(), or using the literal notation (initializer notation). An object initializer is a comma-delimited list of zero or more pairs of property names and associated values of an object, enclosed in curly braces ({}).

### Object literal notation vs JSON:
The object literal notation is not the same as the JavaScript Object Notation (JSON). Although they look similar, there are differences between them:

JSON permits only property definition using "property": value syntax.  The property name must be double-quoted, and the definition cannot be a shorthand.
In JSON the values can only be strings, numbers, arrays, true, false, null, or another (JSON) object.
A function value (see "Methods" below) can not be assigned to a value in JSON.
Objects like Date will be a string after JSON.parse().
JSON.parse() will reject computed property names and an error will be thrown.



### The While Loop:
The while loop loops through a block of code as long as a specified condition is true.

Syntax
while (condition) {
  // code block to be executed
}

### The do while Loop:
This loop will always be executed at least once, even if the condition is false, because the code block is executed before the condition is tested.

Syntax:

do {
  code block to be executed
}
while (condition);

- for - loops through a block of code a number of times.
- for/in - loops through the properties of an object.
- for/of - loops through the values of an iterable object.
- while - loops through a block of code while a specified condition is true.
- do/while - loops through a block of code once, and then repeats the loop while a specified condition is true.

**DOM tree**

The backbone of an HTML document is tags.

According to the Document Object Model (DOM), every HTML tag is an object. Nested tags are “children” of the enclosing one. The text inside a tag is an object as well.

All these objects are accessible using JavaScript, and we can use them to modify the page.

For example, document.body is the object representing the < body> tag.

*Running this code will make the < body> red for 3 seconds:*

document.body.style.background = 'red'; // make the background red

setTimeout(() => document.body.style.background = '', 3000); // return back




### Introduction to JavaScript getElementById() method:

An HTML element often has an id attribute like this:

< div id="root"></ div>
Code language: HTML, XML (xml)
The id is used to uniquely identify an HTML element within the document. By rules, the id root is unique within the document; no other elements can have this root id.

The id is case-sensitive. For example, the 'root' and 'Root' are totally different id.

To select the element by its id, you use the document.getElementById method.

The following shows the syntax of the getElementById() method:

let element = document.getElementById(id);
Code language: JavaScript (javascript)
In this syntax, the id represents the id of the element that you want to select.

The getElementById() returns an Element object that describes the DOM element object with the specified id. It returns null if there is no element with that id exists.

As mentioned earlier, id is unique within a document. However, HTML is a forgiving language. If a document has more than one element with the same id, the getElementById() method returns the first one it encounters.

JavaScript getElementById() method example
Consider the following HTML document:

< html>
    < head>
        < title>JavaScript getElementById() Method< /title>
    </ head>
    < body>
        < p id="message">A paragraph< /p>
    </ body>
</ html>
Code language: HTML, XML (xml)
The document contains a < p> element that has the id attribute with the value message:

const p = document.getElementById('message');
console.log(p);
Code language: JavaScript (javascript)
Output:

< p id="message">A paragraph< /p>
Code language: HTML, XML (xml)
Once you selected an element, you can add styles to the element, manipulate its attributes, and traversing to parent and child elements.

**Summary**
The getElementById() returns a DOM element specified by an id or null if no matching element found.
If multiple elements share the same id, even though it is invalid, the getElementById() returns the first element it encounters.







#### Want To Know More ? 

[Visit our Resources website](https://www.w3schools.com)
OR
[Books](https://www.wiley.com/en-us/Web+Design+with+HTML%2C+CSS%2C+JavaScript+and+jQuery+Set-p-9781119038634)