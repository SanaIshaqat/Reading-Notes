# Code 201 Class 02 Reading notes:

## HTML & CSS :

### HTML Text:

**Headings:**

HTML has six "levels" of headings:

< h1> is used for main headings 

< h2> is used for subheadings
If there are further sections
under the subheadings then the
< h3> element is used, and so
on..

**Paragraphs:**

To create a paragraph, surround the words that make up the
paragraph with an opening < p>
tag and closing < /p> tag.

**Bold & Italic:**

* By enclosing words in the tags
< b> and < /b> we can make
characters appear bold. < Strong>< /Strong> also.
* By enclosing words in the tags
< i> and < /i> we can make
characters appear italic.< em>< /em> also.

*They can be added within a < p>< /p> tag.*

**Superscript & subscript:**

*< sup>*

The < sup> element is used
to contain characters that
should be superscript such
as the suffixes of dates or
mathematical concepts like
raising a number to a power such
as 22.

*< sub>*

The < sub> element is used to
contain characters that should
be subscript. It is commonly
used with foot notes or chemical
formulas such as H20.

**White Space:**

When the browser comes across
two or more spaces next to each
other, it only displays one space.

**Line Breaks & Horizontal Rules:**

*< br />*

The browser will automatically show
each new paragraph or heading
on a new line. But if you wanted
to add a line break inside the
middle of a paragraph you can
use the line break tag < br />.

*< hr />*

To create a break between
themes — such as a change of
topic in a book or a new scene
in a play — you can add a
horizontal rule between sections
using the < hr /> tag.

**Quotations:**

*< blockquote>*

The < blockquote> element is
used for longer quotes that take
up an entire paragraph. the < p> element is still
used inside the < blockquote>
element.

*< q>*

The < q> element is used for
shorter quotes that sit within
a paragraph. Browsers are
supposed to put quotes around
the < q> element, however
Internet Explorer does not 
therefore many people avoid
using the <q> element.

**Abbreviations & Acronyms:**

*< abbr>* *< acronym>

html HTML If you use an abbreviation or
an acronym, then the < abbr>
element can be used. A title
attribute on the opening tag is
used to specify the full term.

*< p>< abbr title="Professor">Prof< /abbr> Stephen
Hawking is a theoretical physicist and
cosmologist.< /p>
< p>< acronym title="National Aeronautics and Space
Administration">NASA< /acronym> do some crazy
space stuff.< /p>*


**Changes to Content:**

*< ins>* *< del>*

The < ins> element can be used
to show content that has been
inserted into a document, while
the < del> element can show text
that has been deleted from it.

### CSS Introduction:
CSS allows you to create rules that specify how the content of
an element should appear.

**Block level elements** look
like they start on a new line.
Examples include the < h1>-
< h6>, < p> and < div> elements.


**Inline elements** flow within the
text and do not start on a new
line. Examples include < b>, < i>,
< img>, < em> and < span>.

**Example Styles**

Boxes: Width and height
Borders (color, width, and style)
Background color and images
Position in the browser window.

Text: Typeface
Size
Color
Italics, bold, uppercase,
lowercase, small-caps

Specific: There are also specific ways
in which you can style certain
elements such as lists, tables,
and forms.


**CSS** works by associating rules with **HTML** elements. These rules govern
how the content of specified elements should be displayed. A CSS rule
contains two parts: a **selector and a declaration**.
CSS Associates Style
rules with HTML
elements

**CSS** declarations sit inside curly brackets and each is made up of two
parts: a **property and a value**, separated by a colon. You can specify
several properties in one declaration, each separated by a semi-colon.

**CSS Types:**

**External Css:** < link> external-css.html HTML
The < link> element can be used
in an HTML document to tell the
browser where to find the CSS
file used to style the page. It is an
empty element (meaning it does
not need a closing tag), and it
lives inside the < head> element.

**Internal CSS:**
< style>
You can also include CSS rules
within an HTML page by placing
them inside a < style> element,
which usually sits inside the
< head> element of the page.

### Summary:

* CSS treats each HTML element as if it appears inside
its own box and uses rules to indicate how that
element should look.
* Rules are made up of selectors (that specify the
elements the rule applies to) and declarations (that
indicate what these elements should look like).
* Different types of selectors allow you to target your
rules at different elements.
* Declarations are made up of two parts: the properties
of the element that you want to change, and the values
of those properties. For example, the font-family
property sets the choice of font, and the value arial
specifies Arial as the preferred typeface.
* CSS rules usually appear in a separate document,
although they may appear within an HTML page.


## JavaScript:
**STATEMENTS**

A script is a series of instructions that a computer can follow one-by-one.
Each individual instruction or step is known as a statement.
Statements should end with a semicolon.

**COMMENTS**

You should write comments to explain what your code does.
They help make your code easier to read and understand.
This can help you and others who read your code.

**Variables**

Variables are containers that store values. You start by declaring a variable with the var (less recommended, dive deeper for the explanation) or the let keyword, followed by the name you give to the variable


**RULES FOR NAMING VARIABLES**

1. The name must begin with
a letter, dollar sign ($),or an
underscore (_). It must not start
with a number.


2. All variables are case sensitive,
so score and Score would be
different variable names, but
it is bad practice to create two
variables that have the same
name using different cases.


3. The name can contain letters,
numbers, dollar sign ($), or an
underscore (_). Note that you
must not use a dash(-) or a
period (.) in a variable name.


4. Use a name that describes the
kind of information that the
variable stores. For example,
fi rstName might be used to
store a person's first name,
l astNarne for their last name,
and age for their age.


5. You cannot use keywords or
reserved words. Keywords
are special words that tell the
interpreter to do something. For
example, var is a keyword used
to declare a variable. Reserved
words are ones that may be used
in a future version of JavaScript.
ONLINE EXTRA
View a full list of keywords and
reserved words in JavaScript.


6. If your variable name is made
up of more than one word, use a
capital letter for the first letter of
every word after the first word.
For example, firstName rather
than firstname (this is referred
to as camel case). You can also
use an underscore between each
word (you cannot use a dash).


**EXPRESSIONS**


An expression evaluates into (results in) a single value. Broadly speaking
there are two types of expressions.

**OPERATORS**

Expressions rely on things called operators; they allow programmers to
create a single value from one or more values.

**ARITHMETIC OPERATORS**

JavaScript contains the following mathematical
operators, which you can use with numbers.

ADDITION +, SUBTRACTION -, DIVISION /, MULTIPLICATION *, 
INCREMENT ++, DECREMENT --, MODULUS %.

**STRING OPERATOR**

There is just one string operator: the+ symbol.
It is used to join the strings on either side of it.

### Decisions & Loops:

**USING COMPARISON OPERATORS**

At the most basic level, you can
evaluate two variables using a
comparison operator to return a
true or false value.

 EXAMPLE:

*var pass = 50; // Pass mark*


*var score = 90; //Score*


*// Check if t he user has passed*

var hasPas sed = score >= pass ;*


*//Write the message into the page*

*var el = document .getElementByld(' answer ');*


*e 1 . t extContent = 'Leve 1 passed: ' + has Passed;*

The example starts by setting
two variables:

1. pass to hold the pass mark
2. score to hold the users score
To see if the user has passed,

A comparison operator checks
whether score is greater than or
equal to pass. The result will be
true or false, and is stored in
a variable called has Passed. On
the next line, the result is written
to the screen.

**USING LOGICAL AND**

he logical AND (&&) operator (logical conjunction) for a set of operands is true if and only if all of its operands are true. It is typically used with Boolean (logical) values. When it is, it returns a Boolean value. However, the && operator actually returns the value of one of the specified operands, so if this operator is used with non-Boolean values, it will return a non-Boolean value.




**USING LOGICAL OR & LOGICAL NOT**

The logical OR (||) operator (logical disjunction) for a set of operands is true if and only if one or more of its operands is true. It is typically used with Boolean (logical) values. When it is, it returns a Boolean value. However, the || operator actually returns the value of one of the specified operands, so if this operator is used with non-Boolean values, it will return a non-Boolean value.

The logical NOT (!) operator (logical complement, negation) takes truth to falsity and vice versa. It is typically used with Boolean (logical) values. When used with non-Boolean values, it returns false if its single operand can be converted to true; otherwise, returns true.

**USING IF STATEMENTS**

- Use if to specify a block of code to be executed, if a specified condition is true

- Use else to specify a block of code to be executed, if the same condition is false

- Use else if to specify a new condition to test, if the first condition is false

- Use switch to specify many alternative blocks of code to be executed