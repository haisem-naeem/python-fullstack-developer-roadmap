
## Python Learning Journey

## Table of Contents

- [Variable and Data types](#variable-and-datatypes-setting-up-and-basic-syntax) 
  - [Python Interpreter and Interactive Mode](#python-interpreter-and-interactive-mode) 
- [Data Structure](#data-structure-lists-tuples-dictionaries-and-sets)
- [Control Flow](#control-flow)
- [Loops](#loops)
- [Python Functions and Modules](#python-function-and-module-examples)
  - [Basic Functions](#functions)
  - [Function parameters](#function-parameters)
  - [Return statements](#return-statements)
  - [Built in modules](#built-in-modules)
  - [Custom modules](#custom-modules)
- [File Handling and Error Handling](#python-file-handling-and-error-handling)
  - [File Handling](#file-handling)
    - [Opening File](#opening-and-reading-a-file)
    - [writing File](#writing-to-a-file)
    - [Apppending File](#appending-to-a-file)
  - [Error Handling](#error-handling)
    - [Try except block](#try-except-block)
    - [Try except else block](#try-except-else-block)
    - [Try except finally block](#try-except-finally-block)
    - [Try except else finally block](#try-except-else-finally-block)
    - [Custom Exception Handlers](#custom-exception-handlers)
- [OOP](#oop)

  - [Encapsulation in Python](#encapsulation-in-python)
    - [Basic Encapsulation](#example-1-basic-encapsulation)
    - [Property Decorators](#example-2-property-decorators)
  - [Abstraction](#introduction)
    - [Abstract Classes](#abstract-classes)
    - [Abstract Methods](#abstract-methods)


 Variable and Datatypes (Setting Up and Basic Syntax)
 ====================================================

## Python Interpreter and Interactive Mode:

- **Understand the Python interpreter and interactive mode.**
  - Write a simple "Hello, World!" program:
    ```python
    print("Hello, World!")
    ```

- **Variables and Datatypes:**
  - Example of variable and datatypes:
    ```python
    age = 25
    height = 5.9
    name = "John Doe"
    ```
  - Perform basic operations with variables:
    ```python
    age = 20
    height = 5.6
    result = age * height
    print(result)
    ```
  - Explore string manipulation and formatting:
    ```python
    greeting = f"Hello, {name}! You are {age} years old."
    print(greeting)
    ```
  - Boolean data type and operations:
    ```python
    is_adult = age >= 18
    print(is_adult)
    ```
  - Basic arithmetic and logical operators:
    ```python
    sum_result = age + 5
    logical_result = is_adult and (height > 5)
    ```

## Data Structure (Lists, Tuples, Dictionaries, and Sets)

- **Lists and Their Properties:**
  - Understand lists and their properties:
    ```python
    numbers = [1, 2, 3, 4, 5]
    print(numbers)
    ```

- **Tuple Data Type and Immutability:**
  - Learn about tuple data type and its immutability:
    ```python
    coordinates = (10, 20)
    ```

- **Practice Manipulating Data with Lists and Tuples:**
  - Practice manipulating data with lists and tuples.

  
- **Dictionaries and Key-Value Pairs:**
  - Explore dictionaries and understand key-value pairs:
    ```python
    student_info = {"name": "Alice", "age": 20, "grade": "A"}
    ```

- **Sets and Their Unique Features:**
  - Learn about sets and their unique features:
    ```python
    unique_numbers = {1, 2, 3, 4, 5}
    ```

- **Practice Using Dictionaries and Sets:**
  - Practice using dictionaries and sets in practical scenarios.
    


--------------------------------------------------------------------------
### Practice:

 - Practice writing small programs that involve variables and basic operations.
  
--------------------------------------------------------------------------

## Control Flow


- **Conditional Statements (if, else):**
  - Study conditional statements (if, else):

    ```python
      if is_adult:
          print("You are an adult.")
      else:
          print("You are a minor.")
    ```

- **Indentation and Simple if-else Conditions:**
  - Understand the concept of indentation in Python.
  - Write programs involving simple if-else conditions:
  
    ```python
    if height > 6:
        print("You are tall!")
    else:
        print("You are not very tall.")
    ```

- **elif Statement for Multiple Conditions:**
  - Explore the elif statement for multiple conditions:
    ```python
    if age < 18:
        print("You are a minor.")
    elif age < 65:
        print("You are an adult.")
    else:
        print("You are a senior.")
    ```

- **Nested if Statements:**
  - Learn about nested if statements:
    ```python
    if age >= 18:
        if height > 5:
            print("You are an adult and tall.")
        else:
            print("You are an adult but not very tall.")
    else:
        print("You are a minor.")
    ```

- **Practice:**
  - Practice writing programs that involve complex control flow.
## Loops

- **For Loop and Syntax:**
  - Learn about the for loop and its syntax:

    ```python
    for i in range(5):
        print(i)
    ```

- **range() Function and Applications:**
  - Understand the range() function and its applications:
    ```python
    for i in range(1, 10, 2):
        print(i)
    ```

- **Programs Using For Loops:**
  - Write programs using for loops:
    ```python
    for char in name:
        print(char)
    ```

- **While Loop and Syntax:**
  - Study the while loop and its syntax:
    ```python
    count = 0
    while count < 3:
        print("Count:", count)
        count += 1
    ```

- **Using Loops for Iteration:**
  - Understand how to use loops for iteration:
    ```python
    for _ in range(3):
        print("Iteration")
    ```

- **Practice:**
  - Practice writing programs using both for and while loops.
  
---------------------------------------------------------------------------

## Python Functions and Modules
## Functions


- **Basics of Functions:**
  - Understand the basics of functions:
    ```python
    def greet():
        print("Hello!")

    greet()
    ```

- **Defining and Calling Functions:**
  - Learn how to define and call functions:
    ```python
    def square(num):
        return num * num

    result = square(4)
    print(result)
    ```

- **Function Parameters and Return Values:**
  - Explore function parameters and return values:
    ```python
    def add(a, b):
        return a + b

    sum_result = add(3, 5)
    print(sum_result)
    ```

- **Function Scopes and Variables:**
  - Study function scopes and local vs. global variables:
    ```python
    global_var = 10

    def print_global():
        local_var = 5
        print("Global Variable:", global_var)
        print("Local Variable:", local_var)

    print_global()
    ```

- **Default and Keyword Arguments:**
  - Learn about default and keyword arguments:
    ```python
    def greet_person(name, greeting="Hello"):
        print(f"{greeting}, {name}!")

    greet_person("Alice")
    greet_person("Bob", greeting="Hi")
    ```

- **Practice:**
  - Practice writing functions for specific tasks.

-----------------------------------------------------------------------

## Function Parameters

### Positional Parameters

```python
    def greet(name, greeting):
        return f"{greeting}, {name}!"
    
    result = greet("Alice", "Hello")
    print(result)
```


### Default Values

```python

    def power(base, exponent=2):
        return base ** exponent
    
    result = power(3)
    print(result)  # Output: 9
```


### Variable-Length Argument Lists

```python
    
    def sum_all(*numbers):
        return sum(numbers)
    
    result = sum_all(1, 2, 3, 4, 5)
    print(result)  # Output: 15
```
## Return Statements


### Single Value

```python
    
    def add(x, y):
        return x + y
    
    result = add(2, 3)
    print(result)  # Output: 5
```    

### Multiple Values

```python
    
    def calculate(x, y):
        return x + y, x - y, x * y
    
    addition, subtraction, multiplication = calculate(5, 3)
    print(addition, subtraction, multiplication)  # Output: 8 2 15
    
```

### Return Types

```python
    
    def divide(x, y) -> float:
        if y != 0:
            return x / y
        else:
            return "Cannot divide by zero"
    
    result = divide(10, 2)
    print(result)  # Output: 5.0
```

## Built-in Modules


### Math Module

```python
    
    import math
    
    circle_area = math.pi * math.pow(2, 2)
    print(circle_area)  # Output: 12.566370614359172
    
```
### Random Module

```python
    import random

    random_number = random.randint(1, 10)
    print(random_number)
```
## Custom Modules


### Creating a Module

```python
    
    # mymodule.py
    
    def multiply(a, b):
        return a * b
```    

### Importing and Using the Module

```python
    # main.py
    import mymodule
    
    result = mymodule.multiply(3, 4)
    print(result)  # Output: 12
```



---------------------------------------------------------------------------------------------

Python File Handling and Error Handling
=======================================

## File Handling


### Opening and Reading a File

```python
    try:         # Open a file in read mode         
        with open('example.txt', 'r') as file:             
            content = file.read()             
            print(content)     
    except FileNotFoundError:         
        print("File not found.")
```

### Writing to a File

```python
    try:         # Open a file in write mode         
        with open('example.txt', 'w') as file:             
            file.write("Hello, World!")     
        except IOError:         
            print("Error writing to the file.")
```

### Appending to a File

```python
    try:         # Open a file in append mode         
        with open('example.txt', 'a') as file:             
            file.write("\nAppending new content.")     
        except IOError:         
            print("Error appending to the file.")
```

------------------------------------------------------------------------

## Error Handling


### Try-Except Block

```python
    try:         
        result = 10 / 0     
    except ZeroDivisionError:         
        print("Cannot divide by zero!")
```

### Try-Except-Else Block

```python
    try:         
        result = 10 / 2     
    except ZeroDivisionError:         
        print("Cannot divide by zero!")     
    else:         
        print("Division successful. Result:", result)
    
```

### Try-Except-Finally Block

```python

    try:         
        file = open('example.txt', 'r')         # Perform file operations
    except IOError:         
        print("Error reading the file.")     
    finally:         
        file.close()
```

### Try-Except-Else-Finally Block

```python

    try:         
        file = open('example.txt', 'r')         # Perform file operations
    except IOError:         
        print("Error reading the file.")   
    else:         
        print("Data in the file:", file)        # Only execute when the try block executes successfully
    finally:         
        file.close()
```
----------------------------------------------------------------------------------------

## Custom Exception Handlers


### Creating Custom Exception

```python
    class CustomError(Exception):         
        def __init__(self, message):             
            self.message = message      
            try:         
                raise CustomError("This is a custom error.")     
            except CustomError as ce:         
                print(f"Custom error caught: {ce.message}")
```

### Raising Custom Exception

```python

    def validate_input(value):         
        if not isinstance(value, int):             
            raise ValueError("Input must be an integer.")      
        try:         
            validate_input("invalid")     
        except ValueError as ve:         
            print(f"Validation error: {ve}")
```



----------------------------------------------------------------------------

OOP
========

## Encapsulation in Python

Encapsulation is one of the fundamental principles of object-oriented programming (OOP) that involves bundling data (attributes) and methods (functions) that operate on the data into a single unit known as a class. The internal workings of a class are hidden from the outside world, and access to the data is restricted to methods defined within the class.

Benefits of Encapsulation:
--------------------------

*   **Data Hiding:** Encapsulation helps in hiding the implementation details of a class and exposes only what is necessary.
*   **Modularity:** It allows you to divide the program into smaller, manageable units (classes).
*   **Code Organization:** Encapsulation promotes better code organization and maintenance.

Examples in Python:
-------------------

### Example 1: Basic Encapsulation

```python

    class Car:
        def __init__(self, make, model):
            self.__make = make  # private attribute
            self.__model = model  # private attribute

        def get_make(self):
            return self.__make

        def get_model(self):
            return self.__model

    # Creating an instance of the Car class
    my_car = Car("Toyota", "Camry")

    # Accessing attributes through methods
    print("Make:", my_car.get_make())  # Output: Make: Toyota
    print("Model:", my_car.get_model())  # Output: Model: Camry

``` 
In this example, the attributes `__make` and `__model` are private, and their values are accessed through getter methods (`get_make` and `get_model`). This ensures that the internal state of the `Car` class is encapsulated.

### Example 2: Property Decorators

```python

    class Circle:
        def __init__(self, radius):
            self.__radius = radius  # private attribute

        @property
        def radius(self):
            return self.__radius

        @radius.setter
        def radius(self, value):
            if value > 0:
                self.__radius = value
            else:
                print("Radius must be greater than zero.")

    # Creating an instance of the Circle class
    my_circle = Circle(5)

    # Accessing and modifying the radius using properties
    print("Radius:", my_circle.radius)  # Output: Radius: 5
    my_circle.radius = 7
    print("New Radius:", my_circle.radius)  # Output: New Radius: 7
    

``` 
Here, the `@property` and `@radius.setter` decorators are used to create a property `radius` with getter and setter methods. This allows controlled access to the private attribute `__radius`.

These examples illustrate the concept of encapsulation in Python, emphasizing the importance of hiding internal details and providing controlled access to class attributes.

---------------------------------------------------------------------------------------------


## Introduction to Abstraction 
Abstraction is a fundamental concept in object-oriented programming that allows the creation of abstract classes and methods, providing a blueprint for concrete classes while hiding the implementation details.

## Abstract Classes
- Abstract classes cannot be instantiated and are meant to be subclassed. They may contain abstract methods, enforcing derived classes to implement specific behaviors.

    ```python
    from abc import ABC, abstractmethod
    
    class Vehicle(ABC):
        @abstractmethod
        def start(self):
            pass
    
        @abstractmethod
        def stop(self):
            pass
    ```

### Abstract Methods
- Abstract methods are declared in abstract classes without providing an implementation. 
Subclasses must implement these methods.

    ``` python
    class Car(Vehicle):
        def start(self):
            print("Car started")
    
        def stop(self):
            print("Car stopped")
    ```

### Interfaces
 - While Python does not have explicit interfaces, abstraction can be achieved by using abstract classes with abstract methods.

    ```python
    class Drawable(ABC):
        @abstractmethod
        def draw(self):
            pass
    
    class Circle(Drawable):
        def draw(self):
            print("Drawing a circle")
    ```

### Example: Abstraction Shape Hierarchy
- A practical example demonstrating abstraction in a shape hierarchy.
    
    ```python
    class Shape(ABC):
        @abstractmethod
        def area(self):
            pass
    
    class Circle(Shape):
        def __init__(self, radius):
            self.radius = radius
    
        def area(self):
            return 3.14 * self.radius * self.radius
    
    class Square(Shape):
        def __init__(self, side):
            self.side = side
    
        def area(self):
            return self.side * self.side
    ```
  
### Conclusion
- Abstraction in Python enables the creation of flexible and extensible code by allowing the definition of abstract classes and methods. It promotes code reuse and modularity.
