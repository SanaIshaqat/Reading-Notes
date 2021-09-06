# Code 301 Class 03 Reading notes:


## React Docs - lists and keys


### What does .map() return?
we use the map() function to take an array and change something with in values. We assign the new array returned by map() .

### If I want to loop through an array and display each value in JSX, how do I do that in React?
You can build collections of elements and include them in JSX using curly braces {}.

Below, we loop through the numbers array using the JavaScript map() function. We return a <li> element for each item. Finally, we assign the resulting array of elements to listItems:

 **Example**

const numbers = [1, 2, 3, 4, 5];
const listItems = numbers.map((number) =>
  <li>{number}</li>
);

### Each list item needs a unique key / IDs .

### What is the purpose of a key?

Keys help React identify which items have changed, are added, or are removed. Keys should be given to the elements inside the array to give the elements a stable identity.

 **Example**
const numbers = [1, 2, 3, 4, 5];
const listItems = numbers.map((number) =>
  <li key={number.toString()}>
    {number}
  </li>
);

## The Spread Operator


### What is the spread operator?

InJavaScript, spread syntax refers to the use of an ellipsis of three dots (…) to expand an iterable object into the list of arguments.
The spread operator was added to JavaScript in ES6 (ES2015), just like the rest parameters, which have the same syntax: three magic dots ….

### List 4 things that the spread operator can do.
The **…** spread operator is useful for many different routine tasks in JavaScript, including the following:
- Copying an array
- Concatenating or combining arrays
- Using Math functions
- Using an array as arguments
- Adding an item to a list
- Adding to state in React
- Combining objects
- Converting NodeList to an array


In each case, the spread syntax expands an iterable object, usually an array, though it can be used on any interable, including a string.

### Give an example of using the spread operator to combine two arrays.
Concatenating arrays
Asseen in the last example, the spread operator can quickly combine two arrays, an operation known as array concatenation:
**Example:**
const myArray = [`🤪`,`🐻`,`🎌`]
const yourArray = [`🙂`,`🤗`,`🤩`]
const ourArray = [...myArray,...yourArray]
console.log(...ourArray) // 🤪 🐻 🎌 🙂 🤗 🤩

### Give an example of using the spread operator to add a new item to an array.
Adding an item to a list
Asnoted in the last example, the spread operator can add an item to an another array with a natural, easy-to-understand syntax:
**Example:**
const fewFruit = ['🍏','🍊','🍌']
const fewMoreFruit = ['🍉', '🍍', ...fewFruit]
console.log(fewMoreFruit) //  Array(5) [ "🍉", "🍍", "🍏", "🍊", "🍌" ]
### Give an example of using the spread operator to combine two objects into one.
Combining objects
The spread syntax is useful for combining the properties and methods on objects into a new object:
**Example:**
const objectOne = {hello: "🤪"}
const objectTwo = {world: "🐻"}
const objectThree = {...objectOne, ...objectTwo, laugh: "😂"}
console.log(objectThree) // Object { hello: "🤪", world: "🐻", laugh: "😂" }
const objectFour = {...objectOne, ...objectTwo, laugh: () => {console.log("😂".repeat(5))}}
objectFour.laugh() // 😂😂😂😂😂



## How to Pass Functions Between Components

### In the video, what is the first step that the developer does to pass functions between components?
created this. props. with same name of the function along with this. calling the funtion. 

### In your own words, what does the increment function do?
when the button is clicked it changes the state and then causes a rerender which then causes a lable with "updated" to appear on the object that it's button was clicked and addes +1 each time to the count.
### How can you pass a method from a parent component into a child component?
ex:
increment=this.increment
### How does the child component invoke a method that was passed to it from a parent component?
using props in the other component js page similar to this:
this.props.increment(this.props.name"ex")

## Things I want to know more about


#### Want To Know More ? 

[Lists & Key](https://reactjs.org/docs/lists-and-keys.html)
[Spread Operator](https://medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab)
[Youtube](https://www.youtube.com/watch?v=c05OL7XbwXU)