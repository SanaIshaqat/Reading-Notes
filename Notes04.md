# Code 301 Class 04 Reading notes:


## React Docs - Forms


## What is a ‘Controlled Component’?

In HTML, form elements such as < input>, < textarea>, and < select> typically maintain their own state and update it based on user input. In React, mutable state is typically kept in the state property of components, and only updated with setState().

We can combine the two by making the React state be the “single source of truth”. Then the React component that renders a form also controls what happens in that form on subsequent user input. An input form element whose value is controlled by React in this way is called a “controlled component”.

## Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.
No we Shouldn't, controlled inputs don’t suffer from the limitations of uncontrolled ones, opening up the follow possibilities:

1. **instant input validation:** 

we can give the user instant feedback without having to wait for them to submit the form (e.g. if their password is not complex enough)

2. **instant input formatting:**

 we can add proper separators to currency inputs, or grouping to phone numbers on the fly

3. **conditionally disable form submission:** 

we can enable the submit button after certain criteria are met (e.g. the user consented to the terms and conditions)

4. **dynamically generate new inputs:** 

we can add additional inputs to a form based on the user’s previous input (e.g. adding details of additional people on a hotel booking)



### How do we target what the user is entering if we have an event handler on an input field?

Since the value attribute is set on our form element, the displayed value will always be **this.state.value**, making the React state the source of truth. Since handleChange runs on every keystroke to update the React state, the displayed value will update as the user types.

With a controlled component, the input’s value is always driven by the React state. While this means you have to type a bit more code, you can now pass the value to other UI elements too, or reset it from other event handlers.


## The Conditional (Ternary) Operator Explained


### Why would we use a ternary operator?

- We use the ternary operator to simplify your if-else statements that are used to assign values to variables. The ternary operator is commonly used when assigning post data or validating forms.

- The ternary operator greatly increases the conciseness of your code. When it is formatted correctly it can also be very easy to read and, dare I say it, even easier then if-else statements.

### Rewrite the following statement using a ternary statement:
  if(x===y){
 console.log(true);
  } else {
 console.log(false);
  }

  **Solution**

x===y?console.log(true):console.log (false)





## Things I want to know more about


#### Want To Know More ? 

[Forms](https://reactjs.org/docs/forms.html)

[The Conditional](https://codeburst.io/javascript-the-conditional-ternary-operator-explained-cac7218beeff)
