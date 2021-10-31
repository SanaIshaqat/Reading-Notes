# Code 401 Class 01 Reading notes:


## What Array.map() does?
The Array. map() method allows you to iterate over an array and modify its elements using a callback function. The callback function will then be executed on each of the array's elements.



## what Array.reduce() does?
The reduce() method executes a user-supplied “reducer” callback function on each element of the array, passing in the return value from the calculation on the preceding element.The final result of running the reducer across all elements of the array is a single value.

## Provide code snippets showing how to use superagent() to fetch data from a URL and log the result:

### With normal Promise .then() syntax 
**From Entrance Exam: Promises**

* const superagent=require('superagent');

const getData =async(req,res)=>{
const url='https://watches-world.herokuapp.com/watches-list/';
await superagent.get(url).then(response=>{
    const responseData=response.body.map(watch=>{
        return new ApiModel(watch);  
    })
    res.send(responseData)
})
}
module.exports={getData} 

### Again with async / await syntax

**From challenge04: Promises**
const superagent = require('superagent');
let characters = {};


let getCharacters = async () => {
 await superagent.get(`https://swapi.dev/api/people/`).then(  (data) => {
   data.body.results.map((item) => {
      characters[item.name] = item.url; 
    })
     console.log(characters);
  });
}

getCharacters();


## Explain promises as though you were mentoring a Code 301 level student

JavaScript is single threaded, meaning that two bits of script cannot run at the same time; they have to run one after another. A Promise is an object that represents the eventual completion (or failure) of an asynchronous operation, and its resulting value.

## Are all callback functions considered to be Asynchronous? Why or Why Not?

Simply taking a callback doesn't make a function asynchronous. There are many examples of functions that take a function argument but are not asynchronous.It iterates over each item and calls the function once per item. This can be used among other things to calculate total value from a property of each item.


#### Want To Know More ? 
- [W3Schools](https://www.w3schools.com/js/)
- [asynchronous programming](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Asynchronous/Async_await)
