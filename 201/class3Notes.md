<sub>Think you might be in the wrong place? [Go home!](../README.md)</sub>

### When should you use an unordered list in your HTML document?

Employ an unordered list when you want to create a list of items without a specific sequence, such as features or key points.

### How do you change the bullet style of unordered list items?
You can change the bullet style of unordered list items using CSS. Use the list-style-type property to set values like "disc," "circle," "square," or "none."
### When should you use an ordered list vs an unorder list in your HTML document?
Choose an ordered list when you need a numbered or ordered sequence, like step-by-step instructions. Use an unordered list for items without a specific order, like bullet points.
### Describe two ways you can change the numbers on list items provided by an ordered list?

* To change numbers in ordered lists, use CSS. Two ways are:

Modify the numbering style with the __list-style-type__ property, e.g., "upper-roman."
Customize list item markers with the __::marker__ pseudo-element in CSS to control their appearance, such as color or size.


### Describe the CSS properties of margin and padding as characters in a story. What is their role in a story titled: “The Box Model”?

In the story "The Box Model" of web design, there are two characters: Margin and Padding.

Margin is the elder, responsible for maintaining space between elements, ensuring they respect their personal boundaries, much like a good neighbor.

Padding, the younger character, protects the content within elements, creating an interior space, like a warm embrace, shielding it from the outside.

Margin and Padding are crucial characters in this story, ensuring order, spacing, and content protection in the web design world.

### List and describe the four parts of an HTML elements box as referred to by the box model.

* __Content:__ The core content of the element.
* __Padding:__ The interior space around the content.
* __Border:__ The protective barrier around the padding.
* __Margin:__ The outermost layer, defining space between elements.

### What data types can you store inside of an Array?

* __Numbers:__ You can store integer or floating-point numbers.
* __Strings:__ Storing text values is common in arrays.
* __Booleans:__ You can store true or false values.
* __Objects:__ You can store objects, which could be other arrays, functions, or custom objects.
* __Arrays:__ Arrays can also hold other arrays, allowing for multidimensional arrays.
* __Functions:__ You can store functions as elements within an array.
* __Undefined:__ If you don't assign a value to an array element, it will be undefined.
* __Null:__ You can store null to represent the absence of a value.
* __Symbols:__ If you're using ES6 or later, you can store symbols.


### Is the people array a valid JavaScript array? If so, how can I access the values stored? If not, why?

``const name = people[0][0];``

### List five shorthand operators for assignment in javascript and describe what they do.

### +=: Adds the value on the right to the variable on the left.
### -=: Subtracts the value on the right from the variable on the left.
### *=: Multiplies the variable on the left by the value on the right.
### /=: Divides the variable on the left by the value on the right.
### %=: Calculates the remainder when dividing the variable on the left by the value on the right and assigns it to the variable.

Read the code below and evaluate the last expression and explain what the result would be and why.
````
 let a = 10;
 let b = 'dog';
 let c = false;

 // evaluate this
 (a + c) + b;
 ````
The expression __(a + c) + b__ results in the string __'10dog'.__ Since one is an interger and the other is a string, they add next to each other.

### Describe a real world example of when a conditional statement should be used in a JavaScript program.

Suppose you're developing an e-commerce website, and you want to show a discount message if a user's cart total is above a certain amount. 

### Give an example of when a Loop is useful in JavaScript.

In an email application, when you need to go through a list of unread messages and mark them as read, you can use a loop.


<sub>Information gathered using ChatGPT</sub>