<sub>Think you might be in the wrong place? [Go home!](../README.md)</sub>


# What are dunder methods in Python, and how do they allow for the customization of built-in behavior in classes? Provide an example of a common dunder method and its purpose.


Dunder methods, short for "double underscore" methods, are special methods in Python that begin and end with double underscores (`__`). They are also known as magic methods. These methods allow developers to define or customize the behavior of built-in operations for their objects, enabling classes to emulate the behavior of built-in types more closely or to implement operator overloading.

For example, the `__init__` method is a common dunder method used for object initialization:
```
class ExampleClass:
    def __init__(self, value):
        self.value = value
```

This method is automatically invoked when a new instance of the class is created, allowing for initial setup of the object with specific attributes.



# Explain the concept of an iterator in Python. How do you create a custom iterator using the iter() and next() methods, and why are they important for enabling iteration in a class?

An iterator in Python is an object that can be iterated over, meaning you can traverse through all the values. Technically, an iterator is an object which implements the iterator protocol, consisting of the methods `__iter__()` and `__next__()`.

To create a custom iterator, you need to implement these two methods:

`__iter__()` returns the iterator object itself and is called upon the initialization of the iterator.
`__next__()` returns the next value from the sequence. On reaching the end, it should raise a StopIteration exception.
Here's a simple example of a custom iterator:
```
class Count:
    def __init__(self, low, high):
        self.current = low
        self.high = high

    def __iter__(self):
        return self

    def __next__(self):
        if self.current > self.high:
            raise StopIteration
        else:
            self.current += 1
            return self.current - 1
```
Iterators are important for enabling explicit iteration over objects in Python, especially within loops like `for` loops.

# What is a generator in Python, and how does it differ from a regular function? Illustrate your answer with an example of a generator function using the ‘yield’ keyword.

A generator in Python is a function that behaves like an iterator. It allows you to write code that can produce a series of values over time, yielding one value at a time. Generators are written using the `yield` keyword. When a generator function calls `yield`, the function execution is paused, and the value is returned to the caller. The function execution resumes on the next call to `next()` on the generator.

Generators are a convenient way to implement iterators as they handle the boilerplate parts of creating an iterator, including the `__iter__()` and `__next__()` methods and the `StopIteration` exception automatically.

Here's an example of a generator function:
```
def count_up_to(max):
    count = 1
    while count <= max:
        yield count
        count += 1
```

# Define decorators in Python and explain their primary use case. How can you create and apply a custom decorator to a function or method? Provide a simple example to demonstrate this concept.

Decorators in Python are a powerful and expressive tool for modifying the behavior of functions or methods. They allow for the wrapping of another function in order to extend the behavior of the wrapped function, without permanently modifying it. Decorators are a very useful aspect of metaprogramming in Python.

To create and apply a custom decorator, you define a wrapper function that takes a function as an argument, defines a nested function inside it to wrap the original function's call, and then returns this nested function. Here's a simple example:
```
def my_decorator(func):
    def wrapper():
        print("Something is happening before the function is called.")
        func()
        print("Something is happening after the function is called.")
    return wrapper

@my_decorator
def say_hello():
    print("Hello!")

say_hello()
```
In this example, `@my_decorator` is applied to `say_hello()`, meaning `say_hello()` will be passed to `my_decorator` as `func`, and the `wrapper()` function will be returned and called instead. This allows us to add behavior before and after the original `say_hello()` function runs, without modifying its definition.

<sub>Information modeled using ChatGPT</sub>