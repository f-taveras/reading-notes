<sub>Think you might be in the wrong place? [Go home!](../README.md)</sub>

### What does a CSS transform allow the developer to do to an element?

CSS transform allows developers to change the appearance of elements by applying transformations like rotation, scaling, skewing, and translation

### Provide an example of a transform and how you could see that being used on a website.

```
.card {
    width: 200px;
    height: 300px;
    background-color: #27ae60;
    transition: transform 0.3s ease-in-out;
}

.card:hover {
    transform: rotate(5deg) scale(1.1);
}

/* HTML */
<div class="card"></div>
```

### What does a CSS transition allow the developer to do to an element?

A CSS transition allows the developer to smoothly animate changes to CSS properties over a specified duration. It provides a way to create simple animations during state changes, such as hover effects. Transitions are triggered by changes in the element's state, like a hover or a class change.

### How does a CSS animation differ from a CSS transition?

CSS animation, on the other hand, is a more complex mechanism that allows for more intricate and detailed animations. It involves the creation of keyframes and the definition of how an element should change its style over the duration of the animation. Animations can loop, have more advanced timing functions, and are generally more flexible for creating complex, multi-step animations.


### What are some benefits to using CSS transitions on websites?

* __Improved User Engagement:__ Transitions can make interactions more engaging and visually appealing, capturing users' attention and making the website more enjoyable to navigate.

* __Smooth State Changes:__ By smoothly transitioning between different states (e.g., hover, active), transitions provide a polished and seamless feel to user interactions.

* __Enhanced Readability and Usability:__ Applying transitions to elements like dropdowns or tooltips can improve readability and usability by providing a gradual reveal or hide effect.

* __Visual Feedback:__ Transitions can offer visual feedback, indicating to users that an action has been taken, such as a button press or link hover.

* __Professional Aesthetics:__ When used appropriately, transitions contribute to the overall aesthetics of a website, giving it a modern and professional appearance.

### How this topic fit in with your long-term goals?

This info gives me the knowledge of the different tools CSS offers for me to utilize and have control over the design of my project.

<sub>Information gathered using ChatGPT</sub>