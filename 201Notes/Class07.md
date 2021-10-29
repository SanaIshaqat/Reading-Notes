# Code 201 Class 07 Reading notes:

## JavaScript :

### Objects constructor notation:

Sometimes you will want several objects to represent similar things.
Object constructors can use a function as a template for creating objects.
First, create the template with the object's properties and methods.

Define the object type by writing a constructor function. There is a strong convention, with good reason, to use a capital initial letter.
Create an instance of the object with new.
To define an object type, create a function for the object type that specifies its name, properties, and methods. 

**For example**, suppose you want to create an object type for cars. You want this type of object to be called Car, and you want it to have properties for make, model, and year. To do this, you would write the following function:

function Car(make, model, year) {
  this.make = make;
  this.model = model;
  this.year = year;
}

#### The HTML DOM (Document Object Model):
When a web page is loaded, the browser creates a Document Object Model of the page.

The HTML DOM model is constructed as a tree of Objects.

With the object model, JavaScript gets all the power it needs to create dynamic HTML:

* JavaScript can change all the HTML elements in the page
* JavaScript can change all the HTML attributes in the page
* JavaScript can change all the CSS styles in the page
* JavaScript can remove existing HTML elements and attributes
* JavaScript can add new HTML elements and attributes
* JavaScript can react to all existing HTML events in the page
* JavaScript can create new HTML events in the page

### JavaScript Random:

**Getting a random integer between two values, inclusive**

While the getRandomInt() function above is inclusive at the minimum, it's exclusive at the maximum. What if you need the results to be inclusive at both the minimum and the maximum? The getRandomIntInclusive() function below accomplishes that.

**Example:**
function getRandomIntInclusive(min, max) {
  min = Math.ceil(min);
  max = Math.floor(max);
  return Math.floor(Math.random() * (max - min + 1) + min); //The maximum is inclusive and the minimum is inclusive
}

### Summary:

* Functions allow you to group a set of related
statements together that represent a single task.
* Functions can take parameters (informatiorJ required to do their job) and may return a value.
* An object is a series of variables and functions that
represent something from the world around you.
* In an object, variables are known as properties of the
object; functions are known as methods of the object.
* Web browsers implement objects that represent both the browser window and the document loaded into the browser window.
* JavaScript also has several built-in objects such as String, Number, Math, and Date. Their properties and
methods offer functionality that help you write scripts.
* Arrays and objects can be used to create complex data
sets (and both can contain the other).


## HTML:

### Tables:

* < table>
The < table> element is used
to create a table. The contents
of the table are written out row
by row.

* < tr>
You indicate the start of each
row using the opening < tr> tag.
(The tr stands for table row.)
It is followed by one or more
< td> elements (one for each cell
in that row).
At the end of the row you use a
closing < /tr> tag.

* < td>
Each cell of a table is
represented using a < td>
element. (The td stands for
table data.)
At the end of each cell you use a
closing < /td> tag.

* < th>
The < th> element is used just
like the < td> element but its
purpose is to represent the
heading for either a column or
a row. (The th stands for table
heading.)

* Even if a cell has no content,
you should still use a < td> or
< th> element to represent
the presence of an empty cell
otherwise the table will not
render correctly. (The first cell
in the first row of this example
shows an empty cell.)

### Summary:

* The < table> element is used to add tables to a web
page.

* A table is drawn out row by row. Each row is created
with the < tr> element.

* Inside each row there are a number of cells
represented by the < td> element (or < th> if it is a
header).

* You can make cells of a table span more than one row
or column using the rowspan and colspan attributes.

* For long tables you can split the table into a < thead>,
< tbody>, and < tfoot>.


#### Want To Know More ? 

[Visit our Resources website](https://www.w3schools.com)
OR
[Books](https://www.wiley.com/en-us/Web+Design+with+HTML%2C+CSS%2C+JavaScript+and+jQuery+Set-p-9781119038634)