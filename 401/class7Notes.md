## Explain the concept of variable scope in Python and describe the difference between local and global scope. Provide an example illustrating the usage of both.

Variable scope refers to the region or part of the code where a variable can be accessed or modified. __In Python, there are two main types of variable scope:__

* __Local Scope:__ Variables defined within a function have a local scope, meaning they can only be accessed and modified within that function. They are not visible outside the function.
* __Global Scope:__ Variables defined outside of any function have a global scope. They can be accessed and modified from anywhere in the code, including within functions.
__Example illustrating Local and Global Scope:__
```
global_variable = 10  # This is a global variable

def my_function():
    local_variable = 5  # This is a local variable
    print("Inside the function - local_variable:", local_variable)
    print("Inside the function - global_variable:", global_variable)

my_function()
print("Outside the function - global_variable:", global_variable)
# Attempting to print local_variable here would result in an error because it's 
not accessible outside the function.
```

__Output:__
```
Inside the function - local_variable: 5
Inside the function - global_variable: 10
Outside the function - global_variable: 10
```
## How do the global and nonlocal keywords work in Python, and in what situations might you use them?

* The __global__ keyword is used to indicate that a variable is a global variable within a function. It allows you to modify the global variable from within a function.
* The __nonlocal__ keyword is used to indicate that a variable in an enclosing (non-global) scope should be modified, rather than creating a new local variable with the same name.

__Example illustrating the use of global and nonlocal keywords:__

```
global_variable = 10

def my_function():
    local_variable = 5
    global global_variable  # Declare that we want to modify the global variable
    global_variable += 1
    print("Inside the function - local_variable:", local_variable)
    print("Inside the function - global_variable:", global_variable)

my_function()
print("Outside the function - global_variable:", global_variable)

def outer_function():
    outer_variable = 10
    def inner_function():
        nonlocal outer_variable  # Declare that we want to modify the enclosing (outer) variable
        outer_variable += 1
        print("Inside inner_function - outer_variable:", outer_variable)
    inner_function()

outer_function()
```
__Output:__
```
Inside the function - local_variable: 5
Inside the function - global_variable: 11
Outside the function - global_variable: 11
Inside inner_function - outer_variable: 11
```
## In your own words, describe the purpose and importance of Big O notation in the context of algorithm analysis.

Big O notation is used in algorithm analysis to describe the upper bound or worst-case performance of an algorithm in terms of time complexity or space complexity. It provides a way to compare and analyze algorithms independently of the hardware and other low-level details.

__The purpose and importance of Big O notation:__

* It helps in evaluating the efficiency of algorithms and choosing the most efficient one for a particular problem.
* It provides a common language for discussing and comparing algorithms in a standardized way.
* It helps in predicting how an algorithm's performance will scale as the input size increases, which is crucial for large datasets and real-world applications.
* It aids in identifying bottlenecks and optimizing code.

## Based on the Rolling Dice Example, explain how you would simulate a dice roll using Python. Describe how you would use code to calculate the probability of rolling a specific number (e.g., the probability of rolling a 6) over a large number of trials.

To simulate a dice roll in Python, you can use the __random__ module. __Here's how you can simulate a dice roll and calculate the probability of rolling a specific number (e.g., 6) over a large number of trials:__
```
import random

def simulate_dice_roll(trials, target_number):
    count_success = 0
    for _ in range(trials):
        roll_result = random.randint(1, 6)  # Simulate a dice roll (1 to 6)
        if roll_result == target_number:
            count_success += 1

    probability = count_success / trials
    return probability

trials = 100000  # Number of trials
target_number = 6  # The number we want to calculate the probability for
result = simulate_dice_roll(trials, target_number)
print(f"Probability of rolling a {target_number} over {trials} trials: {result:.4f}")
```
In this code, we use __random.randint(1, 6)__ to simulate a dice roll, and we repeat this process for a large number of trials. The probability is calculated as the ratio of successful outcomes (rolling a 6) to the total number of trials. This provides an estimate of the probability based on the law of large numbers.