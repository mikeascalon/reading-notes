# Reading notes

How can you use regular expressions in Python to search for specific patterns in a string, and what is the primary module to work with them?

To use regular expressions in Python, you start by importing the re module. Then, depending on your task, you can compile regular expression patterns, use functions like search(), match(), etc., to find patterns in strings, and use functions like sub() to replace text. Groups and special sequences (like \d for digits, \s for whitespace) are also crucial for more complex pattern matching. Regular expressions are a powerful tool in Python for text processing and data manipulation.

What is the purpose of the shutil module in Python, and provide an example of a common use case for file or directory management with this module?

The shutil module in Python provides a number of high-level operations on files and collections of files. This includes functions to support copying and removal of files and directories. Essentially, shutil is used for automating the process of copying and removal of files and directories.

A common use case for the shutil module is copying an entire directory (with all its contents) to a new location. This can be done using the shutil.copytree() function.

```python
import shutil

# Copy the entire contents of "source_directory" to "new_directory".
# If "new_directory" does not exist, it will be created.
# All subdirectories and files in "source_directory" will be copied.

source_directory = "/path/to/source_directory"
new_directory = "/path/to/new_directory"

try:
    shutil.copytree(source_directory, new_directory)
    print("Directory copied successfully.")
except Exception as e:
    print(f"Error occurred: {e}")

```

Compare and contrast the os and shutil modules. When would you choose to use one over the other?

* **Choose os** when you need to interact with the operating system or perform low-level operations like path manipulations, reading or writing individual files, or working with environment variables.
* 
* **Choose shutil** for higher-level file operations like copying or moving directories, deleting directory trees, or working with archives.

## Resouces

[Python Regular Expression Tutorial](https://www.datacamp.com/tutorial/python-regular-expression-tutorial)

[shutil](https://pymotw.com/3/shutil/)

[os](https://pymotw.com/3/os/)

[ChatGPT](https://chat.openai.com/)
