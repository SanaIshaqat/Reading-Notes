# Code 201 Class 10 Reading notes:

## JavaScript:

### Error Handling & Debugging:

### Code Debugging:

Programming code might contain syntax errors, or logical errors.
Many of these errors are difficult to diagnose.

Often, when programming code contains errors, nothing will happen. There are no error messages, and you will get no indications where to search for errors.

Searching for (and fixing) errors in programming code is called code debugging.

**JavaScript Debuggers**

Debugging is not easy. But fortunately, all modern browsers have a built-in JavaScript debugger.
Built-in debuggers can be turned on and off, forcing errors to be reported to the user.
With a debugger, you can also set breakpoints (places where code execution can be stopped), and examine variables while the code is executing.

Normally, otherwise follow the steps at the bottom of this page, you activate debugging in your browser with the F12 key, and select "Console" in the debugger menu.

* The console.log() Method


* Setting Breakpoints:


In the debugger window, you can set breakpoints in the JavaScript code.
At each breakpoint, JavaScript will stop executing, and let you examine JavaScript values.
After examining values, you can resume the execution of code (typically with a play button).

* The debugger Keyword:


The debugger keyword stops the execution of JavaScript, and calls (if available) the debugging function.
This has the same function as setting a breakpoint in the debugger.
If no debugging is available, the debugger statement has no effect.
With the debugger turned on, this code will stop executing before it executes the third line.

* Major Browsers' Debugging Tools:


Normally, you activate debugging in your **browser** with F12, and select "Console" in the debugger menu.


### JavaScript Errors:

**Try to Catch:**

- The **try** statement lets you test a block of code for errors.

- The **catch** statement lets you handle the error.

- The **throw** statement lets you create custom errors.

- The **finally** statement lets you execute code, after try and catch, regardless of the result.



**Syntax** 

The JavaScript statements try and catch come in pairs:

* try {
  Block of code to try
}
* catch(err) {
  Block of code to handle errors
}

**The throw Statement**
The throw statement allows you to create a custom error.

Technically you can throw an exception (throw an error).

The exception can be a JavaScript String, a Number, a Boolean or an Object:

throw "Too big";    // throw a text
throw 500;          // throw a number

*If you use throw together with try and catch, you can control program flow and generate custom error messages.*


**Error Name Values**
Six different values can be returned by the error name property:

- Error Name:	        Description
- EvalError:	        An error has occurred in the eval() function
- RangeError:	        A number "out of range" has occurred
- ReferenceError:	    An illegal reference has occurred
- SyntaxError:	        A syntax error has occurred
- TypeError:	        A type error has occurred
- URIError:	            An error in encodeURI() has occurred



#### Want To Know More ? 

[Visit our Resources website](https://www.w3schools.com)
OR
[Books](https://www.wiley.com/en-us/Web+Design+with+HTML%2C+CSS%2C+JavaScript+and+jQuery+Set-p-9781119038634)