[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/WfNmjXUk)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=15417545&assignment_repo_type=AssignmentRepo)
# SE-Assignment-6
 Assignment: Introduction to Python
Instructions:
Answer the following questions based on your understanding of Python programming. Provide detailed explanations and examples where appropriate.

 Questions:

1. Python Basics:
   - What is Python, and what are some of its key features that make it popular among developers? Provide examples of use cases where Python is particularly effective.
   - Python is a high-level, interpreted programming language known for its simplicity, readability, and versatility. Some key features that make Python popular include:
Easy to learn syntax that emphasizes readability
Interpreted nature allowing for rapid development and testing
Support for multiple programming paradigms like procedural, object-oriented, and functional
Large standard library and ecosystem of third-party packages
Cross-platform compatibility
Python is effective for a wide range of use cases including:
Web development (with frameworks like Django and Flask)
Data analysis and scientific computing (with libraries like NumPy, Pandas, and SciPy)
Machine learning and artificial intelligence
Scripting and automation
Game development
Desktop applications

2. Installing Python:
   - Describe the steps to install Python on your operating system (Windows, macOS, or Linux). Include how to verify the installation and set up a virtual environment.
   - The steps to install Python depend on your operating system:
Windows
Go to https://www.python.org/downloads/ and download the latest version of Python for Windows
Run the installer and make sure to check "Add Python to PATH" during installation
Open the command prompt and type python --version to verify the installation
macOS
Go to https://www.python.org/downloads/ and download the latest version of Python for Mac
Run the installer and follow the prompts
Open Terminal and type python3 --version to verify the installation
Linux
Open a terminal and run sudo apt-get update (for Ubuntu/Debian) or sudo yum update (for CentOS/RHEL)
Install Python with sudo apt-get install python3 (for Ubuntu/Debian) or sudo yum install python3 (for CentOS/RHEL)
Type python3 --version in the terminal to verify the installation
To set up a virtual environment:
Install the venv module with sudo apt-get install python3-venv (Linux/macOS) or py -m pip install virtualenv (Windows)
Create a new virtual environment with python3 -m venv myenv (Linux/macOS) or py -m venv myenv (Windows)
Activate the virtual environment with source myenv/bin/activate (Linux/macOS) or myenv\Scripts\activate (Windows)

3. Python Syntax and Semantics:
   - Write a simple Python program that prints "Hello, World!" to the console. Explain the basic syntax elements used in the program.
   - Here's a simple Python program that prints "Hello, World!" to the console:
python
print("Hello, World!")

The basic syntax elements used are:
print() is a built-in function used to output data to the console
The string "Hello, World!" is the argument passed to the print() function
The statement ends with a newline character by default

4. Data Types and Variables:
   - List and describe the basic data types in Python. Write a short script that demonstrates how to create and use variables of different data types.
   - Python has several built-in data types including:
int: Integers (e.g. 42, -10)
float: Floating-point numbers (e.g. 3.14, -2.5)
str: Strings (e.g. "hello", 'world')
bool: Boolean values (True or False)
list: Ordered collections of items (e.g. [1, 2, 3], ["apple", "banana"])
dict: Unordered key-value pairs (e.g. {"name": "Alice", "age": 25})
Here's an example script demonstrating variables and data types:
python
# Integer variable
age = 30

# Float variable 
pi = 3.14

# String variable
name = "Alice"

# Boolean variable
is_student = True

# List of integers
numbers = [1, 2, 3, 4, 5]

# Dictionary of key-value pairs 
person = {
    "name": "Bob",
    "age": 35,
    "city": "New York"
}

print(age)       # Output: 30
print(pi)        # Output: 3.14
print(name)      # Output: Alice
print(is_student)# Output: True
print(numbers)   # Output: [1, 2, 3, 4, 5]
print(person)    # Output: {'name': 'Bob', 'age': 35, 'city': 'New York'}

5. Control Structures:
   - Explain the use of conditional statements and loops in Python. Provide examples of an `if-else` statement and a `for` loop.
   - Python uses indentation to define code blocks, making control structures like conditional statements and loops very readable. Here's an example of an if-else statement:
python
x = 10
y = 20

if x > y:
    print("x is greater than y")
else:
    print("y is greater than or equal to x")

This will output:
text
y is greater than or equal to x

And here's an example of a for loop:
python
fruits = ["apple", "banana", "cherry"]

for fruit in fruits:
    print(fruit)

This will output:
text
apple
banana 
cherry

The loop iterates over each item in the fruits list, assigning it to the variable fruit on each iteration.

6. Functions in Python:
   - What are functions in Python, and why are they useful? Write a Python function that takes two arguments and returns their sum. Include an example of how to call this function.
   - Functions in Python are reusable blocks of code that perform a specific task. They are defined using the def keyword followed by the function name and parameters (if any). Here's an example:
python
def add_numbers(a, b):
    return a + b

result = add_numbers(5, 10)
print(result)  # Output: 15

The add_numbers() function takes two arguments a and b, adds them together, and returns the result. We call the function with arguments 5 and 10, store the returned value in the result variable, and print it.

7. Lists and Dictionaries:
   - Describe the differences between lists and dictionaries in Python. Write a script that creates a list of numbers and a dictionary with some key-value pairs, then demonstrates basic operations on both.
   - Lists and dictionaries are two of the most commonly used data structures in Python. Here's a script demonstrating their usage:
python
# List of numbers
numbers = [10, 20, 30, 40, 50]

# Access elements in a list
print(numbers[0])   # Output: 10
print(numbers[-1])  # Output: 50

# Modify an element in a list
numbers[2] = 35
print(numbers)      # Output: [10, 20, 35, 40, 50]

# Dictionary of key-value pairs
person = {
    "name": "Alice",
    "age": 25,
    "city": "New York"
}

# Access values in a dictionary
print(person["name"])   # Output: Alice
print(person.get("age")) # Output: 25

# Add a new key-value pair
person["email"] = "alice@example.com"
print(person)          # Output: {'name': 'Alice', 'age': 25, 'city': 'New York', 'email': 'alice@example.com'}

Lists are ordered collections of items, while dictionaries are unordered key-value pairs. Lists use integer indices to access elements, while dictionaries use keys (which can be strings, integers, or other immutable types).

8. Exception Handling:
   - What is exception handling in Python? Provide an example of how to use `try`, `except`, and `finally` blocks to handle errors in a Python script.
   - Exception handling in Python allows you to gracefully handle errors that may occur during program execution. The try, except, and finally blocks are used for this purpose. Here's an example:
python
try:
    result = 10 / 0  # Causes a ZeroDivisionError
except ZeroDivisionError:
    print("Error: Division by zero")
finally:
    print("This block will always execute")

Output:
text
Error: Division by zero
This block will always execute

The try block contains the code that might raise an exception. If a ZeroDivisionError occurs, the code inside the except block is executed, printing an error message. The finally block is always executed, regardless of whether an exception occurred or not.

9. Modules and Packages:
   - Explain the concepts of modules and packages in Python. How can you import and use a module in your script? Provide an example using the `math` module.
   - Modules in Python are files containing Python definitions and statements. They allow you to organize and reuse code. Here's an example of importing and using the math module:
python
import math

# Access functions and attributes from the math module
result = math.sqrt(16)
print(result)  # Output: 4.0

value = math.pi
print(value)   # Output: 3.141592653589793

The math module provides mathematical functions and constants. We import the entire module using import math, then access its functions and attributes using dot notation (math.sqrt(), math.pi).
Packages in Python are collections of modules organized into hierarchical directories. They provide a way to structure and namespace code. For example, the numpy package provides a wide range of mathematical functions and data structures for scientific computing.

10. File I/O:
    - How do you read from and write to files in Python? Write a script that reads the content of a file and prints it to the console, and another script that writes a list of strings to a file.
    - Python provides built-in functions to read from and write to files. Here's an example of reading from a file:
python
# Open a file in read mode
with open("example.txt", "r") as file:
    content = file.read()
    print(content)

This reads the entire contents of the file example.txt and prints it to the console. The with statement ensures that the file is properly closed after the block of code is executed.
And here's an example of writing to a file:
python
# Open a file in write mode
with open("output.txt", "w") as file:
    lines = ["Line 1", "Line 2", "Line 3"]
    file.writelines("\n".join(lines))

This writes a list of strings to the file output.txt, separating each line with a newline character \n. The "w" mode opens the file for writing, creating a new file if it doesn't exist or overwriting an existing file.



# Submission Guidelines:
- Your answers should be well-structured, concise, and to the point.
- Provide code snippets or complete scripts where applicable.
- Cite any references or sources you use in your answers.
- Submit your completed assignment by [due date].


