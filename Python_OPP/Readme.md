# Python OOPs — Object-Oriented Programming

A complete beginner-friendly guide to **Object-Oriented Programming (OOPs) in Python**, covering classes, objects, constructors, inheritance, polymorphism, encapsulation, abstraction, and more.

## 📚 Topics Covered

* Class and Object
* `__init__()` Constructor
* Instance Variables
* Class Variables
* Instance Methods
* Class Methods
* Static Methods
* Encapsulation
* Inheritance
* Polymorphism
* Method Overriding
* Method Overloading
* Abstraction
* `super()`
* Access Modifiers
* Properties
* Magic/Dunder Methods

---

## 1. Class and Object

A **class** is a blueprint for creating objects.

An **object** is an instance of a class.

```python
class Student:
    def display(self):
        print("Student details")


student1 = Student()

student1.display()
```

### Output

```text
Student details
```

---

## 2. Constructor — `__init__()`

The `__init__()` method is automatically called when an object is created.

```python
class Student:

    def __init__(self, name, age):
        self.name = name
        self.age = age

    def display(self):
        print(self.name)
        print(self.age)


student1 = Student("Chetan", 22)

student1.display()
```

---

## 3. Instance Variables

Instance variables belong to a particular object.

```python
class Student:

    def __init__(self, name, age):
        self.name = name
        self.age = age


student1 = Student("Chetan", 22)
student2 = Student("Rahul", 21)

print(student1.name)
print(student2.name)
```

Each object has its own values.

---

## 4. Class Variables

A class variable is shared by all objects of a class.

```python
class Student:

    college = "ABC College"

    def __init__(self, name):
        self.name = name


student1 = Student("Chetan")
student2 = Student("Rahul")

print(student1.college)
print(student2.college)
```

---

## 5. Instance Method

An instance method works with object-specific data.

```python
class Student:

    def __init__(self, name):
        self.name = name

    def display(self):
        print(self.name)


student = Student("Chetan")

student.display()
```

---

## 6. Class Method

A class method works with class-level data.

Use the `@classmethod` decorator.

```python
class Student:

    college = "ABC College"

    @classmethod
    def change_college(cls, college_name):
        cls.college = college_name


Student.change_college("XYZ College")

print(Student.college)
```

---

## 7. Static Method

A static method does not depend on object or class data.

Use the `@staticmethod` decorator.

```python
class Calculator:

    @staticmethod
    def add(a, b):
        return a + b


print(Calculator.add(10, 20))
```

---

# 🔐 Encapsulation

Encapsulation means **binding data and methods together inside a class** and controlling access to data.

Python commonly uses:

```text
Public
_Protected
__Private
```

### Example

```python
class BankAccount:

    def __init__(self, balance):
        self.__balance = balance

    def get_balance(self):
        return self.__balance


account = BankAccount(5000)

print(account.get_balance())
```

Here `__balance` is treated as a private attribute.

---

# 🧬 Inheritance

Inheritance allows one class to reuse the properties and methods of another class.

### Parent Class

```python
class Animal:

    def eat(self):
        print("Animal is eating")
```

### Child Class

```python
class Dog(Animal):

    def bark(self):
        print("Dog is barking")


dog = Dog()

dog.eat()
dog.bark()
```

---

## Types of Inheritance

Python supports:

1. Single Inheritance
2. Multiple Inheritance
3. Multilevel Inheritance
4. Hierarchical Inheritance
5. Hybrid Inheritance

---

## 8. Single Inheritance

```python
class Animal:

    def eat(self):
        print("Eating")


class Dog(Animal):

    def bark(self):
        print("Barking")


dog = Dog()

dog.eat()
dog.bark()
```

---

## 9. Multiple Inheritance

A child class inherits from multiple parent classes.

```python
class Father:

    def skills(self):
        print("Driving")


class Mother:

    def cooking(self):
        print("Cooking")


class Child(Father, Mother):
    pass


child = Child()

child.skills()
child.cooking()
```

---

## 10. Multilevel Inheritance

```text
Grandparent
     ↓
   Parent
     ↓
   Child
```

```python
class Grandparent:

    def property(self):
        print("Property")


class Parent(Grandparent):

    def car(self):
        print("Car")


class Child(Parent):

    def bike(self):
        print("Bike")


child = Child()

child.property()
child.car()
child.bike()
```

---

# 🔄 Polymorphism

Polymorphism means **one interface, multiple forms**.

For example, different classes can have the same method name but different implementations.

```python
class Dog:

    def sound(self):
        print("Bark")


class Cat:

    def sound(self):
        print("Meow")


dog = Dog()
cat = Cat()

dog.sound()
cat.sound()
```

---

# 🔄 Method Overriding

When a child class provides its own implementation of a parent class method, it is called **method overriding**.

```python
class Animal:

    def sound(self):
        print("Animal sound")


class Dog(Animal):

    def sound(self):
        print("Bark")


dog = Dog()

dog.sound()
```

Output:

```text
Bark
```

---

# ⚡ `super()`

`super()` is used to access methods or the constructor of the parent class.

```python
class Animal:

    def __init__(self):
        print("Animal constructor")


class Dog(Animal):

    def __init__(self):
        super().__init__()
        print("Dog constructor")


dog = Dog()
```

Output:

```text
Animal constructor
Dog constructor
```

---

# 🔒 Abstraction

Abstraction means **hiding implementation details and showing only the required functionality**.

Python provides abstraction using the `abc` module.

```python
from abc import ABC, abstractmethod


class Vehicle(ABC):

    @abstractmethod
    def start(self):
        pass


class Car(Vehicle):

    def start(self):
        print("Car started")


car = Car()

car.start()
```

---

# 🪄 Magic / Dunder Methods

Magic methods are special methods that start and end with double underscores.

Examples:

```text
__init__
__str__
__len__
__add__
__eq__
```

### Example

```python
class Student:

    def __init__(self, name):
        self.name = name

    def __str__(self):
        return self.name


student = Student("Chetan")

print(student)
```

---

# 🏠 Property

The `@property` decorator allows a method to be accessed like an attribute.

```python
class Student:

    def __init__(self, name):
        self._name = name

    @property
    def name(self):
        return self._name


student = Student("Chetan")

print(student.name)
```

---

# 🧠 Four Main Pillars of OOP

| Pillar        | Meaning                                   |
| ------------- | ----------------------------------------- |
| Encapsulation | Binding data and methods together         |
| Inheritance   | Reusing properties and methods            |
| Polymorphism  | One interface, multiple implementations   |
| Abstraction   | Hiding unnecessary implementation details |

---

# 📂 Suggested Project Structure

```text
python-oops/
│
├── README.md
│
├── 01_class_object.py
├── 02_constructor.py
├── 03_instance_class_variable.py
├── 04_methods.py
├── 05_encapsulation.py
├── 06_inheritance.py
├── 07_polymorphism.py
├── 08_abstraction.py
├── 09_super.py
├── 10_magic_methods.py
└── 11_property.py
```

---

# 🎯 Learning Path

```text
Class & Object
      ↓
Constructor
      ↓
Instance/Class Variables
      ↓
Methods
      ↓
Encapsulation
      ↓
Inheritance
      ↓
Polymorphism
      ↓
Abstraction
      ↓
Magic Methods
      ↓
Real-World OOP Projects
```

---

## 🚀 Goal

The goal of this repository is to build a strong understanding of **Python Object-Oriented Programming** through simple explanations, examples, and practical implementations.

### Technologies

* Python 3
* Object-Oriented Programming
* Git & GitHub

---

## ⭐ Practice Projects

After completing the concepts, try building:

* Bank Management System
* Student Management System
* Library Management System
* ATM System
* Employee Management System
* Shopping Cart
* Vehicle Management System

---

## 📌 Author

**Chetan**

If you find this repository useful, consider giving it a ⭐ on GitHub.
