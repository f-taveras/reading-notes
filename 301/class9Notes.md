<sub>Think you might be in the wrong place? [Go home!](../README.md)</sub>

### What is functional programming?

Functional programming is a programming paradigm that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data. In functional programming, functions are first-class citizens, meaning they can be passed around as arguments, returned from other functions, and assigned to variables.

### What is a pure function and how do we know if something is a pure function?

A pure function is a function that, given the same input, will always return the same output and has no observable side effects. In other words:

* It relies only on its input parameters.
* It doesn't modify external state.
* It doesn't produce side effects, such as network requests or console logs.

If a function consistently returns the same output for the same input, if it doesn't rely on or modify external state. and If it doesn't produce side effects. it's likely a pure function.

### What are the benefits of a pure function?

* __Predictability:__ Since pure functions have no side effects, they are predictable and easier to reason about.
* __Testability:__ Pure functions are easy to test because they depend only on their input and produce a specific output.
* __Concurrency:__ They are safer in a concurrent or parallel environment as they don't share state.

### What is immutability?

Immutability is a concept where the state of an object cannot be modified after it is created. In functional programming, immutability is favored, and data is treated as immutable. Instead of modifying existing data structures, new ones are created.

### What is Referential transparency?

Referential transparency is a property of pure functions. It means that a function call with a specific set of arguments can be replaced by its return value without affecting the program's behavior. This property allows for optimization, caching, and reasoning about code more easily.

### What is a module?

A module is a self-contained unit of code that encapsulates related functionalities.

### What does the word ‘require’ do?

In _Node.js_, the __require__ function is used to import and include external modules into a program. It is part of the _CommonJS_ module system used by _Node.js_. The __require__ function takes the path to the module as an argument and returns the exported functionalities from that module.

### How do we bring another module into the file the we are working in?

To bring another module into the file you are working in, you use the __require__ function and assign the result to a variable. This variable then contains the exported functionalities from the imported module, and you can use it within the current file.

### What do we have to do to make a module available?

Export functionalities using '__module.exports__' or exports to make a module available.

Example __(math.js)__:

```
exports.add = (a, b) => a + b;
exports.subtract = (a, b) => a - b;
```


Usage __(app.js)__:
```
const math = require('./math');
console.log(math.add(5, 3));           // Output: 8
console.log(math.subtract(10, 4));     // Output: 6
```

<sub>Information gathered using ChatGPT</sub>