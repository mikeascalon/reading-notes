# Reading Notes

What is the basic syntax of Python list comprehension, and how does it differ from using a for loop to create a list? Provide an example of a list comprehension that squares the elements in a given list of integers.

The basic syntax of Python list comprehension

```python
my_new_list = [expression for item in iterable_object]

```

* iterable_object: Represents an iterable object such as a list, tuple, set, etc. The elements of the iterable_object are used to create a new list.
* item: Represents an element of the iterable_object.
expression: Represents the operation that is performed on each item to create the new list.

List comprehension with using a for loop to create a list. Here's an example using a for loop to square the elements in a given list of integers:

```python
myList = [1, 2, 3, 4, 5, 6]
newList = []

for item in myList:
    square = item**2
    newList.append(square)

print("The original list is:", myList)
print("The output list using for loop is:", newList)

```

What is a decorator in Python?

A decorator is a design pattern that allows you to extend or modify the behavior of functions or methods without altering their actual code. Decorators are applied using the "@" syntax, followed by the decorator function or class.

The primary purpose of decorators is to wrap a function or method with additional functionality. This can be useful for tasks such as logging, measuring execution time, enforcing access control, or modifying the return value.

Explain the concept of decorators in Python. How do they work, and what are some common use cases for them? Provide an example of a simple decorator function from the reading.


Decorators in Python are a powerful and flexible way to modify or extend the behavior of functions or methods. They are applied using the "@" syntax, and they wrap a function, allowing you to add functionality before and/or after the original function is called. Decorators are particularly useful for code reuse, separation of concerns, and maintaining clean and readable code.

```python
def my_decorator(func):
    def wrapper():
        print("Something is happening before the function is called.")
        func()
        print("Something is happening after the function is called.")
    return wrapper

def say_whee():
    print("Whee!")

say_whee = my_decorator(say_whee)
```

The my_decorator function is a simple decorator that wraps the say_whee function. When you call say_whee(), it actually invokes the wrapped version created by the decorator. The output would be

```python
Something is happening before the function is called.
Whee!
Something is happening after the function is called.
```

To simplify the syntax for applying decorators, Python provides the "@" syntax. Here's how you can use it for the same example:

```python
@my_decorator
def say_whee():
    print("Whee!")
```
This is equivalent to the previous version where we manually applied the decorator. The syntax @my_decorator is a shorthand way of writing say_whee = my_decorator(say_whee).

Common use cases for decorators include:

1.Logging: Adding logging statements before and after function calls.

2.Timing: Measuring the execution time of functions.

3.Authorization: Enforcing access control to certain functions.

4.Validation: Checking input parameters or output results.

5.Caching: Storing and reusing the results of expensive function calls.


## Resources

[Primer on Python Decorators](https://realpython.com/primer-on-python-decorators/)

[List Comprehension in Python](https://www.pythonforbeginners.com/basics/list-comprehensions-in-python)

[ChatGPT](https://chat.openai.com/)