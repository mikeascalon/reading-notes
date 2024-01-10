# Reading Notes

## Class 3  FileIO & Exceptions

What is the purpose of the ‘with’ statement when opening a file in Python, and how does it help manage resources while reading and writing files?

with statement is particularly useful because it simplifies the syntax, makes the code cleaner, and reduces the chances of resource leaks  like having a helpful assistant that ensures things are set up properly and cleaned up afterward, without you needing to remember all the details manually.

Explain the difference between the ‘read()’ and ‘readline()’ methods for file objects in Python. Provide examples of when to use each method.

`read()` is for reading the entire content at once, while `readline()` is for reading one line at a time. 

Briefly describe the concept of exception handling in Python. How can the ‘try’, ‘except’, and ‘finally’ blocks be used to handle exceptions and ensure proper execution of code? Provide a simple example.

* `try` block: This block contains the code that might raise an exception. It is the part of the code that you want to monitor for errors.

* `except` block: If an exception occurs in the try block, the corresponding except block is executed. It contains the code that handles or responds to the exception.

* `finally` block: This block is optional. It contains code that is always executed, regardless of whether an exception occurred or not. It's often used for cleanup operations.

```python
try:
    # Code that might raise an exception
    number = int(input("Enter a number: "))
    result = 10 / number

except ZeroDivisionError:
    # Handling the specific exception of dividing by zero
    print("Error: Cannot divide by zero!")

except ValueError:
    # Handling the exception when the input is not an integer
    print("Error: Please enter a valid number!")

else:
    # Code to be executed if no exception occurs
    print("Result:", result)

finally:
    # Code to be executed regardless of whether an exception occurred or not
    print("Finally block: This always runs!")

```


### Resources

[Python Tutorial: File Objects - Reading and Writing to Files](https://www.youtube.com/watch?v=Uh2ebFW8OYM)

[Read & Write Files in Python](https://realpython.com/read-write-files-python/)

[Python Exceptions](https://realpython.com/python-exceptions/)

[ChatGPT](https://chat.openai.com/)