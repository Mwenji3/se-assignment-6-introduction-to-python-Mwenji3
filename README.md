[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/WfNmjXUk)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=15375807&assignment_repo_type=AssignmentRepo)
# SE-Assignment-6
 Assignment: Introduction to Python
Instructions:
Answer the following questions based on your understanding of Python programming. Provide detailed explanations and examples where appropriate.

 Questions:

1. Python Basics:
   - What is Python, and what are some of its key features that make it popular among developers? Provide examples of use cases where Python is particularly effective.

Python is a high-level, interpreted programming language known for its readability and simplicity. Key features include dynamic typing, garbage collection, and a comprehensive standard library. Python's popularity stems from its ease of learning, extensive community support, and versatility in applications like web development (e.g., Django), data analysis (e.g., pandas), artificial intelligence (e.g., TensorFlow), and automation (e.g., scripting).

2. Installing Python:
   - Describe the steps to install Python on your operating system (Windows, macOS, or Linux). Include how to verify the installation and set up a virtual environment.

To install Python, download the installer from the official Python website and run it. On Windows, ensure the "Add Python to PATH" option is checked. On macOS and Linux, use package managers like Homebrew (brew install python) or apt-get (sudo apt-get install python3). Verify the installation by running python --version or python3 --version in the terminal. Set up a virtual environment with python -m venv env and activate it using source env/bin/activate (Linux/macOS) or env\Scripts\activate (Windows).

3. Python Syntax and Semantics:
   - Write a simple Python program that prints "Hello, World!" to the console. Explain the basic syntax elements used in the program.

print("Hello, World!")
This program uses the print() function to output text to the console. The string "Hello, World!" is passed as an argument to the function. Python syntax emphasizes readability, using indentation to define code blocks.

4. Data Types and Variables:
   - List and describe the basic data types in Python. Write a short script that demonstrates how to create and use variables of different data types.

   age = 30  # int
height = 5.9  # float
name = "Alice"  # str
is_student = True  # bool
print(age, height, name, is_student)
Basic data types in Python include integers (int), floating-point numbers (float), strings (str), and booleans (bool).

5. Control Structures:
   - Explain the use of conditional statements and loops in Python. Provide examples of an `if-else` statement and a `for` loop.

Conditional statements and loops control the flow of a Python program. An if-else statement executes code blocks based on a condition.
age = 18
if age >= 18:
    print("Adult")
else:
    print("Minor")

numbers = [1, 2, 3, 4, 5]
for num in numbers:
    print(num)


6. Functions in Python:
   - What are functions in Python, and why are they useful? Write a Python function that takes two arguments and returns their sum. Include an example of how to call this function.

Functions in Python are reusable blocks of code that perform specific tasks. They help organize code, making it modular and readable.
def add(a, b):
    return a + b

result = add(5, 3)
print(result)


7. Lists and Dictionaries:
   - Describe the differences between lists and dictionaries in Python. Write a script that creates a list of numbers and a dictionary with some key-value pairs, then demonstrates basic operations on both.

Lists (list) in Python are ordered collections of items, accessed by index. Dictionaries (dict) are unordered collections of key-value pairs. 
# Creating a list and a dictionary
numbers = [1, 2, 3, 4, 5]
person = {"name": "Alice", "age": 30, "city": "New York"}

# Accessing elements
print(numbers[0])      # Output: 1
print(person["name"])  # Output: Alice

# Adding elements
numbers.append(6)
person["email"] = "alice@example.com"

# Removing elements
numbers.remove(3)
del person["age"]
Lists allow accessing elements by index (numbers[0]) and modifying them (append()).
Dictionaries use keys ("name") to access values (person["name"]) and can dynamically add (person["email"]) or remove (del person["age"]) key-value pairs.

8. Exception Handling:
   - What is exception handling in Python? Provide an example of how to use `try`, `except`, and `finally` blocks to handle errors in a Python script.

# Example of exception handling
try:
    result = 10 / 0  # Division by zero
except ZeroDivisionError as e:
    print("Error:", e)
finally:
    print("Execution completed.")
try: block attempts the operation (10 / 0).
except ZeroDivisionError as e: catches the specific error (ZeroDivisionError) and prints the error message (e).
finally: block executes cleanup code (print("Execution completed.")) regardless of whether an exception occurred.

9. Modules and Packages:
   - Explain the concepts of modules and packages in Python. How can you import and use a module in your script? Provide an example using the `math` module.

Modules are Python files containing functions, classes, and variables that can be imported into other scripts. Packages are directories of modules with an __init__.py file.
# Using the math module
import math

print(math.sqrt(16))   # Output: 4.0
print(math.pi)         # Output: 3.141592653589793
import math imports the math module.
math.sqrt(16) calculates the square root of 16.
math.pi accesses the value of pi from the math module.

10. File I/O:
    - How do you read from and write to files in Python? Write a script that reads the content of a file and prints it to the console, and another script that writes a list of strings to a file.

Reading from and writing to files in Python involves opening a file (open()), reading or writing data, and closing the file (close()).
# Reading from a file
with open('sample.txt', 'r') as file:
    content = file.read()
    print(content)

# Writing to a file
data = ["Apple", "Banana", "Orange"]
with open('fruits.txt', 'w') as file:
    for fruit in data:
        file.write(fruit + '\n')
        
open('sample.txt', 'r') opens sample.txt for reading ('r').
file.read() reads the entire content of the file into content.
open('fruits.txt', 'w') opens fruits.txt for writing ('w').
file.write(fruit + '\n') writes each fruit followed by a newline character ('\n') to fruits.txt.

# Submission Guidelines:
- Your answers should be well-structured, concise, and to the point.
- Provide code snippets or complete scripts where applicable.
- Cite any references or sources you use in your answers.
- Submit your completed assignment by [due date].


