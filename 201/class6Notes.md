<sub>Think you might be in the wrong place? [Go home!](../README.md)</sub>

### How would you describe an object to a non-technical friend you grew up with?
Think of an object as a digital container that holds related information about something. It's like a collection of attributes, much like a book having a title, author, and pages.
### What are some advantages to creating object literals?
* __Clarity:__ Organizes related data clearly.
* __Readability:__ Easily understood.
* __Access Control:__ Controls data access.
* __Extensibility:__ Easily adds or removes properties.
### How do objects differ from arrays?
* __bjects:__ Key-value pairs, ideal for complex entities.
* __Arrays:__ Ordered lists, suitable for storing related items.
### Give an example for when you would need to use bracket notation to access an object’s property instead of dot notation.
Use bracket notation when property names have special characters, spaces, or when using variables for dynamic access. 

### Evaluate the code below. What does the term this refer to and what is the advantage to using this?

```
const dog = {
  name: 'Spot',
  age: 2,
  color: 'white with black spots',
  humanAge: function (){
    console.log(`${this.name} is ${this.age*7} in human years`);
  }
}
````
this refers to the object to which the method belongs, which is the dog object.
The use of this allows you to access and manipulate the object's properties and methods from within the object itself. It refers to the current instance, making the code flexible and reusable. 

### What is the __DOM__?
The DOM (Document Object Model) is a way to represent the structure of a web page.
### Briefly describe the relationship between the DOM and JavaScript.
 JavaScript can interact with and modify this structure, making web pages dynamic and interactive.

 <sub>Information gathered using ChatGPT</sub>