<sub>Think you might be in the wrong place? [Go home!](../README.md)</sub>
### Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’?

Render happens first

### What is the very first thing to happen in the lifecycle of React?

The very first thing to happen in the lifecycle of a React component is the __"constructor"__ method. The constructor is called when a component is being created and initialized. It's the right place to initialize state and bind event handlers.

### Put the following things in the order that they happen: componentDidMount, render, constructor, componentWillUnmount, React Updates

     Constructor, react updates, render, componentDidMount, componentWillUnmount

### What does componentDidMount do?

The ____componentDidMount____ method is part of the React component lifecycle. It is called after a component has been rendered to the screen. This is a good place to perform tasks that require interaction with the DOM or external data fetching, such as initiating AJAX requests to load data.

### What types of things can you pass in the props?

* Received from parent components.
* Immutable data passed to child components.
* Used for communication between components.

### What is the big difference between props and state?

* Managed within the component.
* Mutable data for internal component state.
* Updated using __setState__ triggers re-render.

### When do we re-render our application?

* Occurs on state or props changes.
* React handles updates efficiently.
* Components re-render based on changing data.

### What are some examples of things that we could store in state?

* Form data, UI visibility, fetched data.
* Toggle states, counter values.
* Holds mutable data affecting rendering.

<sub>Information gathered using ChatGPT</sub>