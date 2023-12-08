<sub>Think you might be in the wrong place? [Go home!](../README.md)</sub>



### What is a ‘call’?

A 'call' refers to the execution of a function in a programming context. When a function is called, the program transfers control to the function, and the statements inside the function are executed.

### How many ‘calls’ can happen at once?

In a single-threaded environment, only one call can happen at a time. This is because JavaScript follows a single-threaded, synchronous execution model. However, it's important to note that asynchronous operations, such as callbacks, can occur concurrently without blocking the main thread.

### What does LIFO mean?

__LIFO__ stands for _"Last In, First Out."_ It is a principle used in data structures, and in the context of a call stack, it means that the last function that was called is the first one to finish and return control to the calling function.

### Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.

```
function first() {
  second();
  console.log('Inside first');
}

function second() {
  third();
  console.log('Inside second');
}

function third() {
  console.log('Inside third');
}

first();
```

Call Stack:
```
|         |
|  third  | <--- current function (top of the stack)
|  second |
|  first  |
-----------
```

### What causes a Stack Overflow?

A Stack Overflow occurs when the call stack exceeds its maximum size due to an excessive number of function calls. This often happens with recursive functions that don't have a proper base case, leading to an infinite loop of function calls. When the stack limit is reached, the browser or runtime raises a _"Maximum call stack size exceeded"_ error, resulting in a stack overflow.

<sub>Information gathered using ChatGPT</sub>