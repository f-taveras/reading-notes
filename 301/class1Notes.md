<sub>Think you might be in the wrong place? [Go home!](../README.md)</sub>

### What is a “component”?

A _"component"_ refers to a modular, self-contained, and reusable unit of software that encapsulates a set of related functionalities. Components are designed to be easily integrated into larger systems or applications.

### What are the characteristics of a component?

* __Reusability:__ Components are usually designed to be reused in different situations in different applications. However, some components may be designed for a specific task.

* __Replaceable:__ Components may be freely substituted with other similar components.

* __Not context specific:__ Components are designed to operate in different environments and contexts.

* __Extensible:__ A component can be extended from existing components to provide new behavior.

* __Encapsulated:__ A component depicts the interfaces, which allow the caller to use its functionality, and do not expose details of the internal processes or any internal variables or state.

* __Independent:__ Components are designed to have minimal dependencies on other components.

### What are the advantages of using component-based architecture?

* __Reusability:__ Components can be reused in different projects or parts of the same project, reducing development time and effort. This leads to more maintainable and consistent software.

* __Ease of Maintenance:__ Since components are independent and encapsulated, updates or changes to one component do not affect others. This simplifies maintenance and reduces the risk of introducing errors.

* __Collaborative Development:__ Different teams or developers can work on individual components simultaneously, promoting parallel development and collaboration.

* __Rapid Development:__ Components can be developed and tested independently, allowing for faster development cycles. This is especially beneficial in agile development environments.

* __Scalability:__ As components are independent, they can be distributed across multiple servers or containers, facilitating scalability and performance optimization.

* __Interoperability:__ Components with well-defined interfaces can be easily integrated with other components or systems, even if they are built using different technologies.

* __Flexibility and Adaptability:__ Changes to the system can be implemented by modifying or replacing individual components, making the system more adaptable to evolving requirements.


### What is “props” short for?

In React, _"props"_ is short for _"properties."_ Props are a mechanism for passing data from a parent component to a child component. They allow you to pass values, functions, or objects from one component to another.

### How are props used in React?

#### Passing Props:

In a parent component, you can pass data to a child component by including attributes in the child component's JSX. These attributes are known as props.

Example: ``` <ChildComponent propName={propValue} />```

#### Receiving Props:

In the child component, you can access the passed props through the props object.

Example: ```const propValue = this.props.propName;```

#### Using Props:

Once received, props can be used in the child component like regular variables.

Example: ```<p>{propValue}</p>```

### What is the flow of props?

* __Parent to Child:__ Props flow in a unidirectional manner, from parent to child components. The parent component passes data down to its child components through props.

* __Immutable:__ Props are immutable, meaning that a child component cannot modify the props it receives from its parent. They are read-only.

* __Updating Props:__ If the parent component's state changes, and it re-renders, the new values of props are passed down to the child component.

* __Top-Down Data Flow:__ React follows a top-down data flow, where the data is passed from higher-level components to lower-level components through props.

<sub>Information gathered using ChatGPT</sub>