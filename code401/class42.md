# Reading Notes

What are dunder methods in Python, and how do they allow for the customization of built-in behavior in classes? Provide an example of a common dunder method and its purpose.

These “dunders” or “special methods” in Python are also sometimes called “magic methods.” But using this terminology can make them seem more complicated than they really are—at the end of the day there’s nothing “magical” about them.

Dunder methods let you emulate the behavior of built-in types. For example, to get the length of a string you can call len('string'). But an empty class definition doesn’t support this behavior out of the box:

```python
class NoLenSupport:
    pass

>>> obj = NoLenSupport()
>>> len(obj)
TypeError: "object of type 'NoLenSupport' has no len()"
```

To fix this, you can add a __len__ dunder method to your class:

```python
class LenSupport:
    def __len__(self):
        return 42

>>> obj = LenSupport()
>>> len(obj)
42
```

Explain the concept of an iterator in Python. How do you create a custom iterator using the iter() and next() methods, and why are they important for enabling iteration in a class?

An iterator in Python is a mechanism that enables looping or iteration over elements in a sequence or collection, like lists, tuples, or dictionaries. To create a custom iterator, you need to define two special methods: `__iter__()` and `__next__()`. The` __iter__()` method initializes the iterator and returns itself, while the `__next__()` method fetches the next element from the sequence and raises a StopIteration exception when the sequence is exhausted.

Here's a step-by-step tutorial:

1. Begin by defining a class that represents your iterator. This class should have an `__init__()` method to initialize its state, and it should store any necessary data, like the value to be repeated.

2. Implement the `__iter__()` method within your class. This method should return the iterator object itself, usually by simply returning self. This method is called when the iterator is initialized.

3. Define the `__next__()` method in your class. This method should return the next element of the sequence each time it's called, and it should raise a StopIteration exception when there are no more elements to iterate over.

What is a generator in Python, and how does it differ from a regular function? Illustrate your answer with an example of a generator function using the ‘yield’ keyword.

A generator in Python is a special type of function that can generate a sequence of values lazily, one at a time, instead of returning them all at once like a regular function. Generators are created using a `yield` statement instead of a `return` statement. They differ from regular functions in that they maintain their state between invocations and can suspend and resume execution at the point of the `yield` statement.

```python
def repeater(value):
    while True:
        yield value

# Using the generator in a loop
for x in repeater('Hi'):
    print(x)

```

Define decorators in Python and explain their primary use case. How can you create and apply a custom decorator to a function or method? Provide a simple example to demonstrate this concept.

Decorators are functions that modify the behavior of other functions or methods. They allow you to wrap a function or method with additional functionality without modifying its code directly. Decorators are often used for tasks such as logging, authentication, caching, or modifying the behavior of functions based on certain conditions.

```python
from datetime import datetime

def not_during_the_night(func):
    def wrapper():
        if 7 <= datetime.now().hour < 22:
            func()
        else:
            pass  # Hush, the neighbors are asleep
    return wrapper

def say_whee():
    print("Whee!")

say_whee = not_during_the_night(say_whee)
```

## Resouces

[Python Iterators: A Step-By-Step Introduction](https://dbader.org/blog/python-iterators)

[Enriching Your Python Classes With Dunder (Magic, Special) Methods](https://dbader.org/blog/python-dunder-methods)

[What Are Python Generators?](https://dbader.org/blog/python-generators)

[Primer on Python Decorators](https://realpython.com/primer-on-python-decorators/#simple-decorators-in-python)

[ChatGPT](https://chat.openai.com/)