# 🐍 Python for Data Science & AI

> A complete Python learning repository covering Python fundamentals, data structures, functions, file handling, and Object-Oriented Programming as a foundation for Data Science and AI.

---

## 📌 About

Python is one of the most widely used programming languages in **Data Science, Artificial Intelligence, Machine Learning, Web Development, and Automation**.

This repository provides a structured path to learn Python from **basic concepts to advanced programming**, with practical examples and exercises.

---

## 🎯 Objectives

- Learn Python programming from basics.
- Understand Python data types and operators.
- Work with Python data structures.
- Learn conditions and loops.
- Create and use functions.
- Understand file handling.
- Learn Object-Oriented Programming.
- Practice Python through examples and problems.
- Build a strong foundation for Data Science and AI.

---

# 📚 Topics Covered

## 1. 🔰 Python Basics

- Introduction to Python
- Python Features
- Python Installation
- Python Syntax
- Comments
- Variables
- Keywords
- Identifiers
- Input and Output
- `print()`
- `input()`

### Example

```python
name = input("Enter your name: ")
print("Hello", name)
```

---

# 2. 🔢 Data Types

Python provides different built-in data types.

### Basic Data Types

- `int`
- `float`
- `complex`
- `bool`
- `str`

### Collection Data Types

- `list`
- `tuple`
- `set`
- `dict`

### Other

- `NoneType`
- `range`

### Example

```python
num = 10
price = 99.5
name = "Python"
status = True

print(type(num))
print(type(price))
print(type(name))
print(type(status))
```

---

# 3. 🔄 Type Checking & Type Conversion

### Type Checking

```python
num = 10

print(type(num))
```

### Type Conversion

```python
num = "100"

print(int(num))
print(float(num))
print(str(num))
```

Common conversion functions:

```text
int()
float()
str()
bool()
list()
tuple()
set()
dict()
```

---

# 4. ➕ Operators

## Arithmetic Operators

```text
+    Addition
-    Subtraction
*    Multiplication
/    Division
//   Floor Division
%    Modulus
**   Exponentiation
```

## Comparison Operators

```text
==
!=
>
<
>=
<=
```

## Logical Operators

```text
and
or
not
```

## Assignment Operators

```text
=
+=
-=
*=
/=
```

## Membership Operators

```text
in
not in
```

## Identity Operators

```text
is
is not
```

---

# 5. 🔀 Conditional Statements

Conditional statements are used to make decisions.

### Topics

- `if`
- `if-else`
- `if-elif-else`
- Nested `if`

### Example

```python
marks = 75

if marks >= 50:
    print("Pass")
else:
    print("Fail")
```

---

# 6. 🔁 Loops

Loops are used to execute a block of code repeatedly.

## For Loop

```python
for i in range(1, 6):
    print(i)
```

## While Loop

```python
i = 1

while i <= 5:
    print(i)
    i += 1
```

## Loop Control Statements

- `break`
- `continue`
- `pass`

---

# 7. 📋 Strings

A string is a sequence of characters.

### Topics

- Creating Strings
- Indexing
- Slicing
- String Concatenation
- String Repetition
- String Formatting
- String Methods

### Example

```python
text = "Python"

print(text[0])
print(text[1:4])
print(text.upper())
print(text.lower())
```

### Important String Methods

```text
upper()
lower()
title()
capitalize()
swapcase()
find()
index()
replace()
split()
join()
strip()
startswith()
endswith()
```

---

# 8. 📦 Lists

A list is an **ordered and mutable** collection.

### Example

```python
numbers = [10, 20, 30, 40]

numbers.append(50)

print(numbers)
```

### Important List Methods

```text
append()
extend()
insert()
remove()
pop()
clear()
index()
count()
sort()
reverse()
copy()
```

### List Slicing

```python
numbers = [10, 20, 30, 40, 50]

print(numbers[1:4])
print(numbers[:3])
print(numbers[2:])
print(numbers[::-1])
```

---

# 9. 📦 Tuples

A tuple is an **ordered and immutable** collection.

```python
numbers = (10, 20, 30, 40)

print(numbers)
print(numbers[0])
```

### Important Tuple Methods

```text
count()
index()
```

---

# 10. 🔹 Sets

A set is an **unordered collection of unique elements**.

```python
numbers = {10, 20, 30, 20}

print(numbers)
```

### Important Set Methods

```text
add()
update()
remove()
discard()
pop()
clear()
union()
intersection()
difference()
symmetric_difference()
```

---

# 11. 📖 Dictionaries

A dictionary stores data in **key-value pairs**.

```python
student = {
    "name": "Chetan",
    "age": 25,
    "marks": 85
}

print(student["name"])
```

### Important Dictionary Methods

```text
keys()
values()
items()
get()
update()
pop()
popitem()
clear()
copy()
setdefault()
```

---

# 12. 📦 Packing & Unpacking

### Packing

Multiple values can be packed into a single variable.

```python
data = 10, 20, 30

print(data)
```

### Unpacking

Values can be assigned to multiple variables.

```python
a, b, c = (10, 20, 30)

print(a)
print(b)
print(c)
```

---

# 13. ✂️ Slicing

Slicing is used to extract a portion of a sequence.

### Syntax

```text
sequence[start : stop : step]
```

### Example

```python
text = "PYTHON"

print(text[1:4])
print(text[:4])
print(text[2:])
print(text[::-1])
```

Slicing can be used with:

- Strings
- Lists
- Tuples
- Other sequence types

---

# 14. 🧩 Functions

Functions are reusable blocks of code.

### Basic Function

```python
def greet():
    print("Hello Python")

greet()
```

### Function with Parameters

```python
def add(a, b):
    return a + b

result = add(10, 20)

print(result)
```

### Types of Arguments

- Positional Arguments
- Keyword Arguments
- Default Arguments
- Variable-Length Arguments
- `*args`
- `**kwargs`

---

# 15. ⚡ Lambda Functions

A lambda function is a small anonymous function.

```python
square = lambda x: x * x

print(square(5))
```

---

# 16. 📝 Comprehensions

Comprehensions provide a short way to create collections.

### List Comprehension

```python
numbers = [1, 2, 3, 4, 5]

squares = [x * x for x in numbers]

print(squares)
```

### Dictionary Comprehension

```python
numbers = [1, 2, 3]

squares = {x: x*x for x in numbers}

print(squares)
```

---

# 17. 📁 File Handling

File handling is used to create, read, write, and modify files.

### Opening a File

```python
file = open("data.txt", "r")
```

### File Modes

```text
r     Read
w     Write
a     Append
x     Create
r+    Read + Write
w+    Write + Read
a+    Append + Read
```

### Important File Methods

```text
read()
readline()
readlines()
write()
writelines()
close()
```

### Example

```python
with open("data.txt", "w") as file:
    file.write("Hello Python")
```

---

# 18. ⚠️ Exception Handling

Exception handling is used to handle runtime errors.

### Keywords

- `try`
- `except`
- `else`
- `finally`
- `raise`

### Example

```python
try:
    num = int(input("Enter a number: "))
    print(10 / num)

except ZeroDivisionError:
    print("Cannot divide by zero")

except ValueError:
    print("Please enter a valid number")
```

---

# 19. 🏗️ Object-Oriented Programming

OOP is a programming approach based on **classes and objects**.

### Main Concepts

- Class
- Object
- Constructor
- Methods
- Attributes
- Encapsulation
- Inheritance
- Polymorphism
- Abstraction

### Example

```python
class Student:

    def display(self):
        print("Student Details")

student = Student()

student.display()
```

---

# 20. 👨‍👩‍👦 Inheritance

Inheritance allows one class to acquire properties and methods from another class.

### Types

- Single Inheritance
- Multiple Inheritance
- Multilevel Inheritance
- Hierarchical Inheritance
- Hybrid Inheritance

### Example

```python
class Parent:

    def show(self):
        print("Parent Class")


class Child(Parent):

    def display(self):
        print("Child Class")


obj = Child()

obj.show()
obj.display()
```

---

# 21. 🔄 Polymorphism

Polymorphism means **one interface, different behavior**.

Example:

```python
class Dog:

    def sound(self):
        print("Bark")


class Cat:

    def sound(self):
        print("Meow")


for animal in [Dog(), Cat()]:
    animal.sound()
```

---

# 22. 🔒 Encapsulation

Encapsulation means bundling data and methods together and controlling access to data.

```python
class Student:

    def __init__(self):
        self.__marks = 90

    def get_marks(self):
        return self.__marks


student = Student()

print(student.get_marks())
```

---

# 23. 🎭 Abstraction

Abstraction hides implementation details and shows only essential functionality.

Python provides abstraction using the `abc` module.

```python
from abc import ABC, abstractmethod

class Animal(ABC):

    @abstractmethod
    def sound(self):
        pass


class Dog(Animal):

    def sound(self):
        print("Bark")


dog = Dog()
dog.sound()
```

---

# 24. 🧠 Useful Built-in Functions

Some important Python built-in functions:

```text
print()
input()
type()
len()
range()
sum()
min()
max()
abs()
round()
sorted()
enumerate()
zip()
map()
filter()
any()
all()
```

---

# 25. 🧪 Practice Programs

This repository can include Python practice programs such as:

- Check Even or Odd
- Check Positive or Negative
- Find Maximum Number
- Find Minimum Number
- Calculate Factorial
- Generate Fibonacci Series
- Check Prime Number
- Check Palindrome
- Reverse a String
- Count Vowels
- Find Duplicate Elements
- Calculate Average
- Student Grade Calculator
- ATM Program
- Number Guessing Game
- Simple Calculator

---

# 📂 Repository Structure

```text
PYTHON/
│
├── README.md
│
├── Basics/
│   ├── Variables/
│   ├── Data_Types/
│   ├── Input_Output/
│   └── Type_Casting/
│
├── Operators/
│   ├── Arithmetic/
│   ├── Comparison/
│   ├── Logical/
│   ├── Assignment/
│   ├── Membership/
│   └── Identity/
│
├── Conditions/
│   ├── If/
│   ├── If_Else/
│   └── If_Elif_Else/
│
├── Loops/
│   ├── For_Loop/
│   ├── While_Loop/
│   └── Loop_Control/
│
├── Data_Structures/
│   ├── String/
│   ├── List/
│   ├── Tuple/
│   ├── Set/
│   └── Dictionary/
│
├── Functions/
│   ├── Functions/
│   ├── Arguments/
│   ├── Lambda/
│   └── Comprehension/
│
├── File_Handling/
│
├── Exception_Handling/
│
├── OOP/
│   ├── Class_Object/
│   ├── Encapsulation/
│   ├── Inheritance/
│   ├── Polymorphism/
│   └── Abstraction/
│
└── Practice_Programs/
```

---

# 🚀 Installation

Install Python from the official Python website.

Check the installed version:

```bash
python --version
```

Or:

```bash
python3 --version
```

---

# ▶️ How to Run

Run a Python file using:

```bash
python filename.py
```

Example:

```bash
python hello.py
```

---

# ☁️ Google Colab

Python programs can also be executed using Google Colab.

```python
print("Hello, Python!")
```

---

# 🗺️ Python Learning Roadmap

```text
Python Basics
      ↓
Data Types
      ↓
Operators
      ↓
Conditions
      ↓
Loops
      ↓
Strings
      ↓
Lists / Tuples / Sets / Dictionary
      ↓
Functions
      ↓
Comprehensions
      ↓
File Handling
      ↓
Exception Handling
      ↓
OOP
      ↓
Advanced Python
      ↓
NumPy & Pandas
      ↓
Data Science & AI
```

---

# 🎓 Learning Outcomes

After completing this repository, learners should be able to:

- Write Python programs confidently.
- Understand Python syntax and concepts.
- Work with Python data structures.
- Use loops and conditional statements.
- Create reusable functions.
- Handle files and exceptions.
- Apply Object-Oriented Programming.
- Solve programming problems.
- Build a strong foundation for NumPy, Pandas, Machine Learning, and AI.

---

# 🤝 Contributing

Contributions are welcome!

1. Fork the repository.
2. Create a new branch.
3. Add your changes.
4. Commit your changes.
5. Push your branch.
6. Create a Pull Request.

Example:

```bash
git checkout -b feature/new-topic
git add .
git commit -m "Add new Python topic"
git push origin feature/new-topic
```

---

# 📜 License

This repository is created for **educational and learning purposes**.

---

# 👨‍💻 Author

## Chetan

**Python | Data Science | AI | Machine Learning**

---

# ⭐ Support

If you find this repository useful:

- ⭐ Star the repository
- 🍴 Fork the repository
- 📢 Share it with other learners
- 🤝 Contribute to the project

---

## 🚀 Keep Learning

```text
Learn → Practice → Code → Debug → Build
```

> **"Learn Python today, build AI tomorrow."** 🐍🤖
