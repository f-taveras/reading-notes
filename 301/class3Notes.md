<sub>Think you might be in the wrong place? [Go home!](../README.md)</sub>


### What does .map() return?

The __.map()__ method in JavaScript returns a new array by applying a provided function to each element of the original array.

### If I want to loop through an array and display each value in JSX, how do I do that in React?

To loop through an array and display each value in JSX in React, you can use the __.map()__ method to iterate over the array and generate JSX elements for each item. Here's an example:

```
const myArray = [1, 2, 3, 4];

const myList = myArray.map((item) => (
  <li key={item.toString()}>{item}</li>
));

return <ul>{myList}</ul>;
```

### Each list item needs a unique

    Key

### What is the purpose of a key?

The purpose of a __"key"__ is to help identify and track individual elements in a dynamic list. When rendering a list of elements, React uses the keys to optimize the updating process. Keys assist React in efficiently updating and re-rendering only the elements that have changed, rather than re-rendering the entire list. Keys should be unique among siblings in the same list and are typically assigned to the key attribute when using the .__map()__ function to generate elements dynamically.



### What is the spread operator?

The spread operator (...) in JavaScript is used for expanding or spreading the elements of an iterable (like an array or string) into places where multiple elements or arguments are expected.

### List 4 things that the spread operator can do.

* __Copying Arrays and Objects:__

```
const originalArray = [1, 2, 3];
const copiedArray = [...originalArray];
```

* __Concatenating Arrays:__

```
const array1 = [1, 2, 3];
const array2 = [4, 5, 6];
const combinedArray = [...array1, ...array2];
```

* __Adding Elemets to Arrays:__
```
const newArray = [...oldArray, newItem];
```
* __Merging Objects:__
```
const obj1 = { a: 1, b: 2 };
const obj2 = { c: 3, d: 4 };
const mergedObj = { ...obj1, ...obj2 };
```

### Give an example of using the spread operator to combine two arrays.

```
const array1 = [1, 2, 3];
const array2 = [4, 5, 6];
const combinedArray = [...array1, ...array2];
// Result: [1, 2, 3, 4, 5, 6]

```

### Give an example of using the spread operator to add a new item to an array.

```
const oldArray = [1, 2, 3];
const newItem = 4;
const newArray = [...oldArray, newItem];
// Result: [1, 2, 3, 4]
```

### Give an example of using the spread operator to combine two objects into one.

```
const obj1 = { a: 1, b: 2 };
const obj2 = { c: 3, d: 4 };
const mergedObj = { ...obj1, ...obj2 };
// Result: { a: 1, b: 2, c: 3, d: 4 }
```


### In the video, what is the first step that the developer does to pass functions between components?

He passes the function as a prop

### In your own words, what does the handleClick function do?

the function logs "parent click" to the console
### How can you pass a method from a parent component into a child component?

He passes the function as a prop and then attaches the handleClick to the onClick event

### How does the child component invoke a method that was passed to it from a parent component?

creating a function inside the parent component that takes a callback, which is the function we need to pass from the child component




























<sub>Information gathered using ChatGPT</sub>