<sub>Think you might be in the wrong place? [Go home!](../README.md)</sub>

### What are the key principles of Test-Driven Development (TDD) in Python, and how do they contribute to the overall quality of code?

1.  __Write Tests First:__ Before writing functional code, write tests that define the desired behavior.
2.  __Red, Green, Refactor:__
    - __Red:__ Write a test that fails because the feature isn't implemented yet.
    - __Green:__ Write minimal code to make the test pass.
    - __Refactor:__ Clean up the code while ensuring tests still pass.


3. __Small Iterations:__ Implement features in small increments, always keeping the code in a functional state.
4. __Continuous Testing:__ Run tests frequently to catch issues early.
5. __Refactoring:__ Regularly refactor code to improve structure and readability without changing its external behavior.

These principles ensure that the codebase remains reliable and easy to maintain, with a focus on fulfilling requirements and preventing regression.

### Explain the purpose of the if `__name__ == '__main__':` statement in Python scripts. What are some use cases for including this conditional in your code?

Purpose of if `__name__ == '__main__':` in Python Scripts
This statement checks if the script is being run as the main program and not being imported as a module in another script. It allows a script to provide functionality when run standalone and also serve as a reusable module.

- __Use Cases:__

    * __Testing:__ To run tests when the script is executed directly.
Executable Code: To execute specific code (like calling a main function) only when the script is run directly, not when imported.
    * __Providing a CLI:__ When building a script that can be used as both a standalone CLI tool and a module.


### Describe the concept of recursion in Python.

Recursion in Python is a technique where a function calls itself within its definition. It's used to solve problems that can be broken down into smaller, identical problems. A recursive function must have a base case to terminate recursion and avoid infinite loops.

### What is the difference between Python modules and packages? Explain how to create, import, and use them in your Python programs.

* __Modules:__

    A module is a single Python file containing Python definitions and statements, created by writing Python code in a `.py` file imported using import `module_name` or specific objects with from `module_name` import object.
* __Packages:__

    A package is a collection of Python modules in a directory, which must contain an `__init__.py` file.Created by placing multiple `.py` files (modules) in a directory with an `__init__.py` file. Imported similarly to modules, but you can also import specific modules from a package using from package import module.

<sub>Information modeled using ChatGPT</sub>