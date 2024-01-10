### What is the purpose of the _‘with’_ statement when opening a file in Python, and how does it help manage resources while reading and writing files?

The __'with'__ statement in Python is used when opening files to ensure proper resource management, specifically for file handling. It creates a context where the file is automatically opened and closed, ensuring that the file is closed properly when you are done with it or if an exception occurs. This helps in preventing resource leaks and makes your code cleaner and more readable.

Here's an example of how to use the __'with'__ statement to open and read a file:
```
with open('example.txt', 'r') as file:
    data = file.read()
  ```


### Explain the difference between the _‘read()’_ and _‘readline()’_ methods for file objects in Python. Provide examples of when to use each method.

* __read():__ The __read()__ method reads the entire contents of the file as a single string or bytes object (depending on the file mode). It reads until the end of the file or until you specify the number of bytes to read. It's suitable for reading the entire file or if you want to process the entire content at once.

    __Example:__
```
with open('example.txt', 'r') as file:
    data = file.read()
```

* __readline():__ The readline() method reads one line from the file at a time. It returns a string containing the characters up to and including the newline character ('\n'). It's useful when you want to process the file line by line.

    __Example:__
```
with open('example.txt', 'r') as file:
    line = file.readline()
    while line:
        line = file.readline()
```

### Briefly describe the concept of exception handling in Python. How can the _‘try’_, _‘except’_, and _‘finally’_ blocks be used to handle exceptions and ensure proper execution of code? Provide a simple example.

Exception handling in Python is a mechanism for dealing with errors and exceptions that may occur during the execution of a program. It allows you to gracefully handle errors without causing the program to crash.

* __try:__ The try block is used to enclose the code that might raise an exception. If an exception occurs within the try block, it will be caught.
* __except:__ The except block is used to specify what should happen when a specific exception is raised. You can have multiple except blocks to handle different types of exceptions.
* __finally:__ The finally block is optional and is used to specify code that should be executed regardless of whether an exception occurred or not. It's typically used for cleanup operations, like closing files or releasing resources.

    __Example:__
```
try:
    num1 = int(input("Enter a number: "))
    num2 = int(input("Enter another number: "))
    result = num1 / num2
    print("Result:", result)
except ValueError:
    print("Invalid input. Please enter valid numbers.")
except ZeroDivisionError:
    print("Cannot divide by zero.")
finally:
    print("Execution completed.")
```