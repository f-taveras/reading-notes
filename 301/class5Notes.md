sub>Think you might be in the wrong place? [Go home!](../README.md)</sub>





### What is the single responsibility principle and how does it apply to components?
SRP dictates that a component should have one responsibility or reason to change. Applied to React, each component should focus on a specific aspect, like rendering UI or managing state.

### What does it mean to build a ‘static’ version of your application?

Creating a 'static' version involves building the UI with fixed data, providing a foundation for the application's structure.

### Once you have a static application, what do you need to add?

Once you have a static version of your application, the next step is to add interactivity. This involves introducing dynamic behavior, handling user input, and managing state changes. You'll start incorporating React features like state and props to make your application respond to user actions and update the UI accordingly.

### What are the three questions you can ask to determine if something is state?

* Three Questions:
  - Does it change over time?
  - Can it be computed from other state or props?
  - Does it affect the rendering of the component?
  - Identifying Where State Needs to Live:

### How can you identify where state needs to live?

* Steps:
    - Find components that re-render based on state.
    - Determine the source of truth for the state.
    - Lift state up to a common ancestor if shared among components.


### What is a “higher-order function”?

A higher-order function is a function that takes one or more functions as arguments or returns a function as its result. In JavaScript, functions are first-class citizens, meaning they can be treated as values, passed as parameters, and returned from other functions. Higher-order functions enable powerful and flexible programming paradigms like functional programming

### Explore the greaterThan function as defined in the reading. In your own words, what is line 2 of this function doing?

In this function, __'greaterThan__' takes a parameter '__n__' and returns an anonymous function that takes another parameter '__m__'. This returned function checks whether '__m__' is greater than the initial value '__n__'. It utilizes a closure to remember the value of __'n'__ from the outer function.

### Explain how either map or reduce operates, with regards to higher-order functions.

The '__map__' function is a higher-order function that applies a provided function to each element of an array and returns a new array with the results. It transforms each element without mutating the original array.


<sub>Information gathered using ChatGPT</sub>