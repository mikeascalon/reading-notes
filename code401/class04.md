# Reading Notes

What are the key differences between classes and objects in Python, and how are they used to create and manage instances of a class?

* Objects are an encapsulation of variables and functions into a single entity. Objects get their variables and functions from classes. Classes are essentially a template to create your objects. Instances have their own set of attributes and share the methods defined in the class. Classes and objects provide a way to model and organize code in an object-oriented fashion, promoting encapsulation and reusability.

Explain the concept of recursion and provide an example of how it can be used to solve a problem in Python. What are some best practices to follow when implementing a recursive function?

* Recursion is a programming concept where a function calls itself directly or indirectly to solve a smaller instance of the same problem. In other words, a function uses its own result in a smaller version of the problem to solve the original problem.

```python
def factorial(n):
    # Base case: factorial of 0 or 1 is 1
    if n == 0 or n == 1:
        return 1
    else:
        # Recursive case: n! = n * (n-1)!
        return n * factorial(n - 1)
```
* In this example, the factorial function calculates the factorial of a number using recursion. The base case is when n is 0 or 1, where the factorial is 1. In the recursive case, the function calls itself with a smaller argument (n-1), and the results are combined to get the final result.

What is the purpose of pytest fixtures and code coverage in testing Python code? Explain how they can be used together to improve the quality and maintainability of a project.

* By combining Pytest fixtures and code coverage, you can create a testing environment that is not only well-organized and maintainable but also provides insights into the effectiveness of your tests. This combination helps in identifying and addressing areas where the test coverage can be improved, contributing to higher code quality and more robust software.

## Resources

[Classes and Objects](https://www.learnpython.org/en/Classes_and_Objects)

[Thinking Recursively](https://realpython.com/python-thinking-recursively/)

[Pytest Fixtures and Coverage](https://www.linuxjournal.com/content/python-testing-pytest-fixtures-and-coverage)

[Pytest Fixtures and Coverage](https://docs.pytest.org/en/latest/explanation/fixtures.html)

[Pytest Fixtures](https://docs.pytest.org/en/latest/explanation/fixtures.html)

[Chatgpt](https://chat.openai.com/)