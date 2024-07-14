[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/WfNmjXUk)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=15397557&assignment_repo_type=AssignmentRepo)
# SE-Assignment-6
 Assignment: Introduction to Python
Instructions:
Answer the following questions based on your understanding of Python programming. Provide detailed explanations and examples where appropriate.

 Questions:

1. Python Basics:
   - What is Python, and what are some of its key features that make it popular among developers? Provide examples of use cases where Python is particularly effective.
 
 Python is an interpreted programming language used by programmers.
 It is known for its readability and versatility.
	Readability in that it has a clear and readable syntax.
	Versatility in that it can be used widely, i.e., it can be used for web development, data analysis, AI, Scientific Computing and much more.
	Other key features include its extensive libraries i.e., NumPy, Pandas, and TensorFlow and that its open source i.e., free to use and distribute.

Web Development: 
Frameworks like Django and Flask enable rapid web application development.
Example: Building a full-stack web application

Data Analysis and Visualization: 
Libraries like Pandas, Matplotlib, and Seaborn help in data manipulation and visualization.
Example: Analyzing large datasets and creating visual reports.

Machine Learning and AI:
Libraries such as TensorFlow, Keras, and Scikit-learn are widely used for developing machine learning models.
Example: Developing a predictive model for customer churn.

Scientific Computing: 
Libraries like NumPy and SciPy are used for complex scientific calculations.
Example: Performing mathematical computations and simulations in physics or engineering.
Automation and Scripting: 
Python scripts automate repetitive tasks and processes.
Example: Automating data entry tasks or web scraping.

Game Development: 
Libraries like Pygame allow for game creation.
Example: Developing simple 2D games.

Cybersecurity: 
Tools and scripts for penetration testing and network security.
Example: Writing a script to scan for network vulnerabilities.

Financial Analysis: 
Libraries like QuantLib help in financial modeling and analysis.
Example: Analyzing stock market trends and creating trading algorithms.

Internet of Things (IoT): 
Python runs on microcontrollers for IoT applications.
Example: Programming a Raspberry Pi to control home automation systems.

2. Installing Python:
   - Describe the steps to install Python on your operating system (Windows, macOS, or Linux). Include how to verify the installation and set up a virtual environment.

I downloaded the latest version of python, which is version 3.12.4 
@ https://www.python.org/downloads/ 
I run it as administrator 
I selected add python.exe to PATH and the install now option 

To verify installation: 
python --version
I navigated to my project folder
Created the virtual environment by using the following code: 
python -m venv myenv
To activate my environment
source myenv/Scripts/activate


3. Python Syntax and Semantics:
   - Write a simple Python program that prints "Hello, World!" to the console. Explain the basic syntax elements used in the program.

print (“Hello, World”)
print 
Keyword used to display or print something to the screen        
And because it is a string, it is enclosed in brackets and quotation marks

4. Data Types and Variables:
   - List and describe the basic data types in Python. Write a short script that demonstrates how to create and use variables of different data types.
- 1. Integer (`int`): Represents whole numbers without a fractional component.
Example: 42, -7
Script:
integer_var = 42 creates an integer variable.

2. Float (`float`): Represents numbers with a fractional component.
Example: 3.14 or -0.001
Script:
float_var = 3.14 creates a float variable

3. String (`str`): Represents a sequence of characters (text).
Example: "Hello, World!", "Python3"
Script:
string_var = "Hello, World!" creates a string variable.

4. Boolean (`bool`): Represents one of two values: `True` or `False`.
Example: True, False
Script:
boolean_var = True creates a boolean variable.

5. List (`list`): Represents an ordered, mutable collection of elements.
Example: [1, 2, 3], ["apple", "banana", "cherry"]
Script:
list_var = [1, 2, 3, "apple", "banana"] creates a list containing integers and strings.



6. Tuple (`tuple`): Represents an ordered, immutable collection of elements.
Example: (1, 2, 3), ("apple", "banana", "cherry")
Script: 
tuple_var = (1, 2, 3, "apple", "banana") creates a tuple containing integers and strings.

7.  Dictionary (`dict`): Represents a collection of key-value pairs, unordered and mutable.
Example: {"name": "Alice", "age": 30}`, {"apple": 1, "banana": 2}
Script: 
dict_var = {"name": "Alice", "age": 30} creates a dictionary with string keys and mixed value types.

8. Set (`set`): Represents an unordered collection of unique elements that are mutable.
Example: {1, 2, 3}, {"apple", "banana", "cherry"}
Script:
set_var = {1, 2, 3, "apple", "banana"} creates a set containing integers and strings.




5. Control Structures:
   - Explain the use of conditional statements and loops in Python. Provide examples of an `if-else` statement and a `for` loop.

If-else
Conditional statements allow you to execute specific blocks of code based on certain conditions. The keywords if, elif, and else are usually used to execute these conditions
Example 
age = 18
if age >= 18:
    print("You are an adult.")
else:
    print("You are a minor.")
Interpretation
The if statement checks the condition age >= 18 if it is true. It will print  that “You are an adult” where this condition is satisfied else it will print that “You are minor” 
Loops
Loops are used to execute a block of code repeatedly
Example 
fruits = [“lemon", "banana", "orange"]
for fruit in fruits:
    print(fruit) 

Interpretation
It iterates through the fruit list taking the value of the current element in the list.
 i.e., 
1st iteration = lemon will be printed
2nd iteration = banana will be printed
3rd iteration = orange will be printed


6. Functions in Python:
   - What are functions in Python, and why are they useful? Write a Python function that takes two arguments and returns their sum. Include an example of how to call this function.

Blocks of reusable code that perform a specific task. They allow you to break your code into smaller, modular pieces, making it easier to read, maintain, and debug.
  
1. Reusability: You can call a function multiple times throughout your code without rewriting it.
2. Modularity: Breaking code into functions makes it easier to understand and manage.
3. Maintainability: Functions help isolate different parts of your code, making it easier to update and maintain.

# Function example to add two numbers 
def add_two_numbers(a, b):
    return a + b

Interpretation
The def keyword is used to define a function named add_two_numbers.
The function takes two parameters, a and b.
The return statement returns the sum of a and b.

# Example of how to call this function
result = add_two_numbers(5, 3)
print(f"The sum of 5 and 3 is: {result}")

Interpretation
The function is called with arguments 5 and 3, and the result is stored in the variable result.
The result is printed, showing the sum of 5 and 3 is 8

7. Lists and Dictionaries:
   - Describe the differences between lists and dictionaries in Python. Write a script that creates a list of numbers and a dictionary with some key-value pairs, then demonstrates basic operations on both.
   - 
Lists:
	Ordered: Elements in a list have a defined order and can be accessed by their index.
	Mutable: You can modify the elements of a list after its creation (add, remove, change elements).
	Indexed: Elements are accessed using integer indices starting from 0.
	Homogeneous/ Heterogeneous: Can store elements of any data type, either of the same or different types.
	Syntax: Defined using square brackets []


Dictionaries:
•	Unordered: Dictionaries do not maintain the order of elements 
•	Mutable: You can modify the key-value pairs after creation (add, remove, change pairs).
•	Key-Value Pairs: Elements are accessed using unique keys, which can be of any immutable data type (usually strings or numbers).
•	Homogeneous/ Heterogeneous: Can store values of any data type, and the keys can be of different types.
•	Syntax: Defined using curly braces {} with key-value pairs separated by a colon :

# Creating a list of numbers
numbers_list = [1, 2, 3, 4, 5]   [1, 2, 3, 4, 5] creates a list of numbers
print("Original List:", numbers_list) Output  Original List: 1, 2, 3, 4, 5


Demonstrate basic operations[Lists]
Append
numbers_list.append(6)    	 # Append, adds an element to the end of the  list
print("List after appending 6:", numbers_list)	Output  List after appending 6: 1, 2, 3, 4 , 5, 6 
Remove
numbers_list.remove(3)      	 # Remove, removes an element from the list
print("List after removing 3:", numbers_list)       Output  List after removing  3: 1, 2, 4, 5, 6

print("Element at index 2:", numbers_list[2])  	# Accessing an element by index
							Output  Element at index: 3

# Creating a dictionary with key-value pairs
person_dict = {		{"name": "Alice", "age": 30, "city": "New York"} creates a dictionary with key-value pairs
  "name": "Alice",
    "age": 30,
    "city": "New York"
}
print("\nOriginal Dictionary:", person_dict) 

Output Original Dictionary: {'name': 'Alice', 'age': 30, 'city': 'New York' }  

Demonstrate basic operations[Dictionary]
person_dict["email"] = alice@example.com  # person_dict["email"] Adds a key-value pair
print("Dictionary after adding email:", person_dict)

Output  Dictionary after adding email: {'name': 'Alice', 'age': 30, 'city': 'New York’, ’email’: ‘alice@example.com’}

del person_dict["age"]  # del, removes a key-value pair
print("Dictionary after removing age:", person_dict)

Output  Dictionary after adding email: {'name': 'Alice', 'city': 'New York’, ’email’: ‘alice@example.com}

print ("Value for key 'name':", person_dict["name"])  # Access a value by key

Output  Value for key ‘name’: Alice 

8. Exception Handling:
   - What is exception handling in Python? Provide an example of how to use `try`, `except`, and `finally` blocks to handle errors in a Python script.
 - Exception handling in Python is a way to manage errors that occur during the execution of a program. 
By using try, except, and finally blocks, you can handle exceptions gracefully and ensure that your program can recover from unexpected situations or perform necessary cleanup tasks.

# Example 1: Division by Zero
num1 = 10
num2 = 0

def divide_numbers(a, b):
    try:  
        result = a / b
    except ZeroDivisionError as e:
        print(f"Error: Division by zero is not allowed. Details: {e}")
        result = None
    finally:
        print("Execution of the try-except-finally block is complete.")
    return result

Calling the function
divide_numbers(num1, num2)

Output
Error: Division by zero is not allowed. Details: division by zero
Execution of the try-except-finally block is complete.


Interpretation
try Block: Attempts to divide `10` by `0`, which raises a `ZeroDivisionError`.
except Block: Catches the `ZeroDivisionError` and prints an error message.
finally Block: Always executes and prints a message indicating completion of the block.

# Example 2: Invalid Data Type
num1 = 10
num2 = "five"

def divide_numbers(a, b):
    try:
        result = a / b
    except TypeError as e:
        print(f"Error: Invalid data type. Details: {e}")
        result = None
    finally:
        print("Execution of the try-except-finally block is complete.")
    return result

Calling the function
divide_numbers(num1, num2)

Output
Error: Invalid data type. Details: unsupported operand type(s) for /: 'int' and 'str'
Execution of the try-except-finally block is complete.

Interpretation
try Block: Attempts to divide `10` by `"five"`, which raises a `TypeError` because you can't divide an integer by a string.
except Block: Catches the `TypeError` and prints an error message.
finally Block: Always executes and prints a message indicating completion of the block.


# Example 3: Successful Division
num1 = 10
num2 = 2

def divide_numbers(a, b):
    try:
        result = a / b
    except ZeroDivisionError as e:
        print(f"Error: Division by zero is not allowed. Details: {e}")
        result = None
    except TypeError as e:
        print(f"Error: Invalid data type. Details: {e}")
        result = None
    else:
        print(f"Division successful. Result: {result}")
    finally:
        # This block always runs, regardless of whether an exception occurred
        print("Execution of the try-except-finally block is complete.")
    return result
Calling the function
divide_numbers(num1, num2)

Output
Division successful. Result: 5.0
Execution of the try-except-finally block is complete.

Interpretation:
try Block: Successfully divides `10` by `2`, resulting in `5.0`.
else Block: Executes because no exception was raised, printing the successful division result.
finally Block: Always executes and prints a message indicating completion of the block.


9. Modules and Packages:
   - Explain the concepts of modules and packages in Python. How can you import and use a module in your script? Provide an example using the `math` module.

Modules
A module in Python is a file containing Python code (e.g., functions, classes, variables) that you can import and use in other Python scripts. 
Modules help in organizing code into manageable sections and promoting code reusability. One can create their own modules or use the built-in and third-party modules.

Packages
A package is a collection of modules organized in directories that provide a hierarchical structure. A package typically contains an __init__.py file, which indicates to Python that the directory should be treated as a package. 
Packages allow for a structured module namespace.
How can you import and use a module in your script? Provide an example using the `math` module.
To use a module in your script, you need to import it. There are several ways to import a module:
	Import the whole module:
import module_name
	Import specific attributes from a module:
from module_name import attribute1, attribute2

Example 1: Importing the whole math module

import math

Example 2: Calculate the square root of a number using math.sqrt():

number = 4
square_root = math.sqrt(number)
print(f"The square root of {number} is {square_root}")


10.  File I/O:
    - How do you read from and write to files in Python? Write a script that reads the content of a file and prints it to the console, and another script that writes a list of strings to a file.

Reading from a File
To read from a file in Python, you can use the open function in combination with the read or readlines methods. 

Example: How to read a file
file_path = 'example.txt'
with open(file_path, 'r') as file:
    content = file.read()
    print(content)

Interpretation
open(file_path, 'r'): Opens the file in read mode ('r').
with statement: Ensures the file is properly closed after the block of code is executed.
file.read(): Reads the entire content of the file.
print(content): Prints the content of the file to the console.

Example: 
Suppose example.txt contains the following text:
Hello, World!
This is an example file.
It has multiple lines.

Running script 
Hello, World!
This is an example file.
It has multiple lines.

Writing to a File
To write to a file, you use the open function with the write mode ('w'), and then the write or writelines methods to write the content to the file.

file_path = 'output.txt'
lines = ["First line of text\n", "Second line of text\n", "Third line of text\n"]

with open(file_path, 'w') as file:
    file.writelines(lines)

Interpretation
open(file_path, 'w'): Opens the file in write mode ('w'). If the file does not exist, it creates a new file. If it exists, it truncates the file.
with statement: Ensures the file is properly closed after the block of code is executed.
file.writelines(lines): Writes the list of strings to the file. Each string in the list is written as a new line in the file.

Example
After running the writing script, output.txt will contain:
First line of text
Second line of text
Third line of text	




# Submission Guidelines:
- Your answers should be well-structured, concise, and to the point.
- Provide code snippets or complete scripts where applicable.
- Cite any references or sources you use in your answers.
- Submit your completed assignment by [due date].


