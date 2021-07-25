# Code 201 Class 01 Reading notes:
## How People Access the Web? 

### Browsers
People access websites using
software called a web browser.
Popular examples include
Firefox, Internet Explorer, Safari,
Chrome, and Opera.

### Web Servers
When you ask your browser for
a web page, the request is sent
across the Internet to a special
computer known as a web
server which hosts the website.
### Devices
People are accessing websites
on an increasing range of devices
including desktop computers,
laptops, tablets, and mobile
phones. 
### Screen readers
Screen readers are programs
that read out the contents of a
computer screen to a user. They
are commonly used by people
with visual impairments.

## How Websites Are Created?
**All websites use HTML and CSS, but content
management systems, blogging software, and
e-commerce platforms often add a few more
technologies into the mix.**

## How the Web Works?
When you visit a website, the web server
hosting that site could be anywhere in the
world. In order for you to find the location of
the web server, your browser will first connect
to a Domain Name System **(DNS)** server.


## HTML Uses Elements to Describe the Structure of Pages:
1. There are several different elements. Each
element has an opening tag and a closing tag.

2. Tags act like containers. They tell you
something about the information that lies
between their opening and closing tags.
3. Attributes Tell Us More About Elements.


## Summary STRUCTURE HTML 
* pages are text documents.
* HTML uses tags (characters that sit inside angled
brackets) to give the information they surround special
meaning.
* Tags are often referred to as elements.
* Tags usually come in pairs. The opening tag denotes
the start of a piece of content; the closing tag denotes
the end.
* Opening tags can carry attributes, which tell us more
about the content of that element.
* Attributes require a name and a value.
* To learn HTML you need to know what tags are
available for you to use, what they do, and where they
can go.


## Extra Markup :

* DOCTYPES tell browsers which version of HTML you
are using.
* You can add comments to your code between the
< !-- and --> markers.
* The id and class attributes allow you to identify
particular elements.
* The <div> and <span> elements allow you to group
block-level and inline elements together.
* <iframes> cut windows into your web pages through
which other pages can be displayed.
* The <meta> tag allows you to supply all kinds of
information about your web page.
* Escape characters are used to include special
characters in your pages such as <, >, and ©.

## HTML5:
HTML5 is introducing a new set of
elements that help define the structure of
a page.
They are covered here (rather than with the other HTML
elements you met earlier in the book) because you'll find
it easier to understand how they can be used now that you
have seen how CSS can control the layout a page. These
new elements are going to play an important part in creating
layouts going forward.


**HTML5 introduces a new set of elements that allow you to divide up the
parts of a page. The names of these elements indicate the kind of content
you will find in them. They are still subject to change, but that has not
stopped many web page authors using them already.**

* The new HTML5 elements indicate the purpose of
different parts of a web page and help to describe
its structure.
* The new elements provide clearer code (compared
with using multiple <div> elements).
* Older browsers that do not understand HTML5
elements need to be told which elements are
block-level elements.
* To make HTML5 elements work in Internet Explorer 8
(and older versions of IE), extra JavaScript is needed,
which is available free from Google.

## Process & Design:
1. It's important to understand who your target audience
is, why they would come to your site, what information
they want to find and when they are likely to return.
2. Site maps allow you to plan the structure of a site.
3. Wireframes allow you to organize the information that
will need to go on each page.
3. Design is about communication. Visual hierarchy helps
visitors understand what you are trying to tell them.
4. You can differentiate between pieces of information
using size, color, and style.
5. You can use grouping and similarity to help simplify
the information you present.



## JavaScript
### The ABC of Progamming:
#### What is a script and how to create one?
A script is a series of instructions that the computer
can follow in order to achieve a goal.

Each time the script runs, it might only use a subset of
all the instructions.

Computers approach tasks in a different way than
humans, so your instructions must let the computer
solve the task prggrammatically.

To approach writing a script, break down your goal into
a series of tasks and then work out each step needed
to complete that task (a flowchart can help).



#### How to write script for webpage?

It is best to keep JavaScript code in its own JavaScript
file. JavaScript files are text files (like HTML pages and
CSS style sheets), but they have the . j s extension.

The HTML <script> element is used in HTML pages
to tell the browser to load the JavaScript file (rather like
the <link> element can be used to load a CSS file).

If you view the source code of the page in the browser,
the JavaScript will not have changed the HTML,
because the script works with the model of the web
page that the browser has created.