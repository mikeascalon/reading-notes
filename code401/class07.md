# Ten Thousand 2

Explain the concept of variable scope in Python and describe the difference between local and global scope. Provide an example illustrating the usage of both.

In Python, variable scope defines the context in which a variable is valid and can be accessed. There are two primary scopes: local and global. Local scope applies to variables defined within a function, making them accessible only within that specific function. Once the function completes, these local variables cease to exist. For instance, if a variable 'x' is defined inside a function, it is confined to that function's scope and cannot be accessed outside of it.

Example of local scope:

```python
def example_function():
    x = 10  # Local variable
    print("Inside the function:", x)

example_function()
# Attempting to access x here will result in an error

```

On the other hand, global scope refers to variables defined outside of any function or block, making them accessible from anywhere in the program. Global variables persist throughout the entire program's execution. It's essential to note that if a variable with the same name exists both globally and locally, the local variable takes precedence within its specific scope. Understanding variable scope is crucial for writing robust and error-free code, preventing unintended conflicts or modifications between variables in different parts of the program. This distinction helps maintain code clarity and promotes better organization.

Example of global scope:

```python
y = 5  # Global variable

def another_function():
    print("Inside another_function:", y)

another_function()
print("Outside any function:", y)

```

How do the global and nonlocal keywords work in Python, and in what situations might you use them?

1.Global Keyword:
* The global keyword is used to indicate that a variable is a global variable, allowing it to be accessed and modified from anywhere in the program.
* When a variable is defined as global inside a function, it refers to the global variable rather than creating a local one.

2.Nonlocal Keyword:

* The nonlocal keyword is used within a nested function to indicate that a variable is not local to that function but belongs to the enclosing (non-global) scope.
* This is particularly useful when dealing with nested functions and you want to modify a variable from an outer (enclosing) scope.

In your own words, describe the purpose and importance of Big O notation in the context of algorithm analysis.

Imagine you have a bunch of different ways to solve a problem, like finding a specific book in a library. Each approach may take a different amount of time and effort. Big O notation is like a simplified guide that helps us compare these approaches in terms of efficiency.

Based on the Rolling Dice Example, explain how you would simulate a dice roll using Python. Describe how you would use code to calculate the probability of rolling a specific number (e.g., the probability of rolling a 6) over a large number of trials.

To simulate a dice roll in Python, you can use the random module, which provides a randint function to generate random integers. 

```python
import random

def simulate_dice_roll():
    # Simulate a single dice roll (assuming a standard six-sided die)
    return random.randint(1, 6)

def calculate_probability(target_number, num_trials):
    # Simulate dice rolls and count occurrences of the target number
    count_target = 0
    for _ in range(num_trials):
        if simulate_dice_roll() == target_number:
            count_target += 1

    # Calculate the probability
    probability = count_target / num_trials
    return probability

# Example: Simulate 10,000 dice rolls and calculate the probability of rolling a 6
target_number = 6
num_trials = 10000

result_probability = calculate_probability(target_number, num_trials)
print(f"The probability of rolling a {target_number} in {num_trials} trials is approximately: {result_probability:.4f}")

```

In this example, the simulate_dice_roll function generates a random integer between 1 and 6, simulating a single dice roll. The calculate_probability function then uses this to simulate a specified number of trials and calculates the probability of rolling the target number over those trials.

Adjust the target_number and num_trials variables based on your specific scenario. Running the code multiple times with different parameters can give you an idea of how the probability converges to the theoretical probability as the number of trials increases. Keep in mind that the result may vary slightly due to the inherent randomness of the simulation.

### Resources

[Python Scope & the LEGB Rule: Resolving Names in Your Code](https://realpython.com/python-scope-legb-rule/)

[Big O notation is simpler than you might think](https://www.youtube.com/watch?v=dNorFNlDbX0)

[Basic Programming With Python](https://web.archive.org/web/20220608035657/https://artofproblemsolving.com/wiki/index.php/Basic_Programming_With_Python#Random)

[ChatGPT](https://chat.openai.com/)