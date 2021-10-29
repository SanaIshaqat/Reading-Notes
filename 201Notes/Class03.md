# Code 201 Class 03 Reading notes:

## JavaScript :

### ARRAYS:
An array is a special variable, which can hold more than one value at a time,an array can hold many values under a single name, and you can access the values by referring to an index number (starts with 0).

**Syntax:**

const array_name = [item1, item2, ...];     

**Example:**
const cars = ["Saab", "Volvo", "BMW"];


**Changing an Array Element**
This statement changes the value of the first element in cars:

cars[ 0] = "Opel";

### The else if Statement
Use the else if statement to specify a new condition if the first condition is false.

**Syntax**
if (condition1) {
  //  block of code to be executed if condition1 is true
} else if (condition2) {
  //  block of code to be executed if the condition1 is false and condition2 is true
} else {
  //  block of code to be executed if the condition1 is false and condition2 is false
}
**Example**
If time is less than 10:00, create a "Good morning" greeting, if not, but time is less than 20:00, create a "Good day" greeting, otherwise a "Good evening":

if (time < 10) {
  greeting = "Good morning";
} else if (time < 20) {
  greeting = "Good day";
} else {
  greeting = "Good evening";
}
The result of greeting will be:

Good day

### Switch Statement:
The switch statement is used to perform different actions based on different conditions.
Use the switch statement to select one of many code blocks to be executed.

**Syntax**
switch(expression) {
  case x:
    // code block
    break;
  case y:
    // code block
    break;
  default:
    // code block
}

**This is how it works:**

1. The switch expression is evaluated once.
2. The value of the expression is compared with the values of each case.
3. there is a match, the associated block of code is executed.
4. If there is no match, the default code block is executed.

### Type Coercion and Weak Typing:

When you write an expression, function, etc. (anything with a variable in it really), JavaScript will take the variable you declare and define and do it’s best to figure out what data type seems appropriate to the context. This is called type coercion.

Type coercion can lead to unexpected values in your code (and also cause errors).Therefore, when checking if two values are equal, it is considered
**better to use strict equals operators ===and ! == rather than == and ! =** as these strict operators check that the value and data types match.

### Loops:

Loops are handy, if you want to run the same code over and over again, each time with a different value.
Loops can execute a block of code a number of times.

* **The For Loop**

The for loop has the following syntax:

for (statement 1; statement 2; statement 3) {
  // code block to be executed
}
Statement 1 is executed (one time) before the execution of the code block.

Statement 2 defines the condition for executing the code block.

Statement 3 is executed (every time) after the code block has been executed.


**Example:**

for (let i = 0; i < 5; i++) {
  text += "The number is " + i + "<br>";
}
From the example above, you can read:

Statement 1 sets a variable before the loop starts (let i = 0).

Statement 2 defines the condition for the loop to run (i must be less than 5).

Statement 3 increases a value (i++) each time the code block in the loop has been executed.

* **The While Loop**

The while loop loops through a block of code as long as a specified condition is true.

Syntax
while (condition) {
  // code block to be executed
}
**Example**
In the following example, the code in the loop will run, over and over again, as long as a variable (i) is less than 10:


while (i < 10) {
  text += "The number is " + i;
  i++;
}

* **The Do While Loop**
The do while loop is a variant of the while loop. This loop will execute the code block once, before checking if the condition is true, then it will repeat the loop as long as the condition is true.

Syntax
do {
  // code block to be executed
}
while (condition);

**Example**
The example below uses a do while loop. The loop will always be executed at least once, even if the condition is false, because the code block is executed before the condition is tested:


do {
  text += "The number is " + i;
  i++;
}
while (i < 10);


## HTML & CSS:

### HTML Lists:

* **Unordered HTML List**

 An unordered list starts with the < ul> tag. Each list item starts with the 
< li> tag.

The list items will be marked with bullets (small black circles) by default

* **Ordered HTML List**

An ordered list starts with the < ol> tag. Each list item starts with the 
< li> tag.

The list items will be marked with numbers by default


* **HTML Description Lists**


A description list is a list of terms, with a description of each term.

The <dl> tag defines the description list, the <dt> tag defines the term (name), and the <dd> tag describes each term:


**Lists can be nested inside one another**

### CSS Boxes:

**Box Dimensions:**


1. Border (Style, Width, Color)

Every box has a border (even if it is not visible or is specified to
be 0 pixels wide). The border separates the edge of one box from another.
2. Margin

Margins sit outside the edge of the border. You can set the width of a margin to create a gap between the borders of two
adjacent boxes.

3. Padding

Padding is the space between the border of a box and any
content contained within it. Adding padding can increase the readability of its contents.


**Summary Boxes**

* CSS treats each HTML element as if it has its own box.

* You can use CSS to control the dimensions of a box.

*  You can also control the borders, margin and padding
for each box with CSS.

* It is possible to hide elements using the display and
visibility properties.

* Block-level boxes can be made into inline boxes, and
inline boxes made into block-level boxes.

* Legibility can be improved by controlling the width of
boxes containing text and the leading.

* CSS3 has introduced the ability to create image
borders and rounded borders.



#### Want To Know More ? 
[Visit our Resources website](https://www.w3schools.com)
OR
[Books](https://www.wiley.com/en-us/Web+Design+with+HTML%2C+CSS%2C+JavaScript+and+jQuery+Set-p-9781119038634)