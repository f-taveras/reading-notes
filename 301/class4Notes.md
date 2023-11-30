<sub>Think you might be in the wrong place? [Go home!](../README.md)</sub>


### What is a ‘Controlled Component’?

A "controlled component" in React refers to a form element (like ``<input>``, ``<textarea>``, or ``<select>``) whose value is controlled by the state of a React component. In a controlled component, the value of the form element is handled by the React component's state, and any changes to the input are controlled by React through state updates. This means that the source of truth for the input value is the React state, and the input value is set and updated through the onChange event handler.

### Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.

It is common and recommended to update the state with the user's responses as soon as they enter them rather than waiting until they submit the form. This approach is known as "controlled components" and provides a more interactive and responsive user experience. By updating the state as the user types, you can show instant feedback, perform real-time validation, and make the form more user-friendly.

Updating the state on each keystroke allows you to respond to changes dynamically, providing a better user experience. However, the decision may also depend on the specific requirements of your application and the type of form you are dealing with.

### How do we target what the user is entering if we have an event handler on an input field?

In React, you can target what the user is entering by accessing the __event__ object in the event handler function. The event object contains information about the input event, including the current value of the input field.

### Why would we use a ternary operator?

A ternary operator is a concise way to write an if-else statement in a single line of code. It's a shorthand syntax that can make your code more readable and less verbose.

Rewrite the following statement using a ternary statement:
```
if(x===y){
  console.log(true);
} else {
  console.log(false);
}
```

Answer:

```
console.log(x === y ? true : false);
```





















<sub>Information gathered using ChatGPT</sub>