# Reading Notes

What are the key principles of Test-Driven Development (TDD) in Python, and how do they contribute to the overall quality of code?

* Test-Driven Development (TDD) in Python adheres to key principles that contribute significantly to code quality. The primary principle involves writing tests before implementing the actual code, ensuring a clear definition of expected behavior. This approach enables the early detection of issues, as tests are expected to fail initially. The subsequent cycle of writing the minimal code to pass the tests, followed by refactoring, promotes the development of modular and maintainable code. 

Explain the purpose of the if __name__ == '__main__': statement in Python scripts. What are some use cases for including this conditional in your code?

* The article provides an example where the code under this conditional is executed when the script is invoked directly, and a different code is executed when the script is imported. This construct is particularly useful when developing scripts that can be both standalone programs and reusable modules. It enables developers to include specific actions or tests that should only occur when the script is the main entry point to the program.

Describe the concept of recursion in Python.

Recursion in Python is a programming concept where a function calls itself directly or indirectly in order to solve a problem. In a recursive function, the problem is divided into smaller instances of the same problem, and the function is applied to these smaller instances. 

What is the difference between Python modules and packages? Explain how to create, import, and use them in your Python programs.


In Python, modules and packages serve distinct purposes for organizing and structuring code. A module is a single file containing Python definitions and statements, acting as a logical grouping of related functionalities. To create a module, one simply needs to create a Python file and define the desired code within it.On the other hand, a package is a directory hierarchy containing related modules. It includes a special __init__.py file, indicating that the directory should be treated as a package. 

## Resources

[In Tests We Trust — TDD with Python](https://code.likeagirl.io/in-tests-we-trust-tdd-with-python-af69f47e6932)

[What does the if __name__ == “__main__”: do?](https://www.geeksforgeeks.org/what-does-the-if-__name__-__main__-do/)

[Introduction to Recursion – Data Structure and Algorithm](https://www.geeksforgeeks.org/introduction-to-recursion-data-structure-and-algorithm-tutorials/)

[What on Earth is Recursion? - Computerphile](https://www.youtube.com/watch?v=Mv9NEXX1VHc)

[ChatGPT](https://chat.openai.com/)