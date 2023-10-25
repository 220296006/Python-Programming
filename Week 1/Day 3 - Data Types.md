# Data Types in Python

Data types are fundamental in programming as they define the kind of data a variable can hold and the operations that can be performed on it. Python has several built-in data types, which can be broadly categorized as follows:

## Numeric Data Types

### 1. Integers (int)

Integers represent whole numbers, both positive and negative. They do not have a decimal point.

Example:

```python

x = 5
y = -10

```

### 2. Floating-Point Numbers (float)

Floating-point numbers represent real numbers and have a decimal point. They can also use scientific notation.

Example:

```python

pi = 3.14159
price = 4.99

```

### 3. Strings (str)

Strings represent text and are enclosed in single, double, or triple quotes. They are immutable in Python.

Example:

```python

name = "Alice"
message = 'Hello, World!'

```

### 4. Booleans (bool)

Booleans represent binary values, True or False. They are often used for conditions and logic.

Example:

```python

is_valid = True
is_authenticated = False

```

## 5. Lists (list)

Lists are ordered collections of items. They can contain elements of different data types and are mutable.

Example:

```python

fruits = ["apple", "banana", "cherry"]
numbers = [1, 2, 3, 4, 5]

```

## 6. Tuples (tuple)

Tuples are similar to lists but are immutable. Once created, their elements cannot be changed.

Example:

```python

coordinates = (3, 4)
colors = ("red", "green", "blue")

```

## 7. Dictionaries (dict)

Dictionaries store data in key-value pairs. They are unordered and mutable.

Example:

```python

person = {"name": "Alice", "age": 30}
student = {"id": 12345, "name": "Bob", "courses": ["Math", "Science"]}

```

## 8. Sets (set)

Sets are collections of unique elements. They are unordered and mutable.

Example:

```python

fruits = {"apple", "banana", "cherry"}
numbers = {1, 2, 3, 4, 5}

```

## 9. NoneType (None)

None represents the absence of a value. It is often used to indicate a missing or undefined value.

Example:

```python

value = None

```

Python's flexibility in handling different data types makes it a versatile language for a wide range of applications. Understanding data types is crucial for effectively working with data in Python.

## Integers in Python

Integers are a fundamental data type in Python that represent whole numbers. They can be both positive and negative and do not have a decimal point. Here's an overview of integers in Python:

## Integer Variables

You can assign integer values to variables, and Python will determine their data type automatically:

```python
x = 5  # A positive integer
y = -10  # A negative integer

```

## Mathematical Operations

Python supports various mathematical operations on integers, such as addition, subtraction, multiplication, and division:

```python
a = 10
b = 5

addition_result = a + b  # Addition
subtraction_result = a - b  # Subtraction
multiplication_result = a * b  # Multiplication
division_result = a / b  # Division (result is a float)

```

## Integer Division and Modulus

Python also allows integer division (//) to obtain the quotient of a division and the modulus (%) to get the remainder:

```python

dividend = 17
divisor = 5

quotient = dividend // divisor  # Integer division
remainder = dividend % divisor  # Modulus

```

## Built-in Functions

Python provides built-in functions for working with integers, such as abs(), pow(), and round():

```python

absolute_value = abs(-5)  # Absolute value
power_result = pow(2, 3)  # Exponentiation (2^3)
rounded_number = round(3.14159)  # Rounding

```

## Integer Limits

In Python, integers have no fixed size. They can grow as large as the available memory of your system allows. Python 2 had a distinction between int and long, but Python 3 unified them into a single int type.

## Type Conversion

You can convert other data types to integers using the int() function. For example, converting a string to an integer:

```python

x = "42"  # A string
y = int(x)  # Convert to an integer


```

Integers play a crucial role in various mathematical and computational tasks in Python, making them an essential data type to work with.

## Booleans in Python

Booleans are a fundamental data type in Python that represent binary values: `True` or `False`. They are often used for conditions and logical operations. Here's an overview of booleans in Python:

## Boolean Variables

You can assign boolean values to variables:

```python
is_valid = True  # A boolean variable with a value of True
is_authenticated = False  # A boolean variable with a value of False

```

## Logical Operators

Python provides several logical operators for working with booleans, including and, or, and not:

and Operator
The and operator returns True if both operands are True:

```python

result = True and True  # result is True
result = True and False  # result is False

```

## or Operator

The or operator returns True if at least one of the operands is True:

```python

result = True or False  # result is True
result = False or False  # result is False

```

## not Operator

The not operator negates a boolean value, turning True into False and vice versa:

```python

result = not True  # result is False
result = not False  # result is True

```

## Comparison Operators

Comparison operators are used to compare values and return a boolean result. Common comparison operators include == (equal), != (not equal), < (less than), > (greater than), <= (less than or equal to), and >= (greater than or equal to):

```python

result = 5 == 5  # result is True
result = 5 != 3  # result is True
result = 5 < 10  # result is True
result = 5 > 10  # result is False

```

## Conditional Statements

Booleans are frequently used in conditional statements like if, elif, and else to control the flow of a program:

```python

if is_valid:
    print("This condition is valid.")
elif is_authenticated:
    print("Authentication succeeded.")
else:
    print("Neither condition is met.")

```

## Truthy and Falsy Values

In Python, certain values are considered "truthy" (evaluate to True) and "falsy" (evaluate to False). Some common falsy values include False, None, 0, 0.0, and empty containers (e.g., empty strings, lists, dictionaries). All other values are considered truthy.

Understanding and working with booleans is essential for creating conditional logic and controlling the flow of your Python programs.

## Floating-Point Numbers (float) in Python

Floating-point numbers are a fundamental data type in Python that represent real numbers with decimal points. They are used for calculations involving non-integer values and can also use scientific notation. Here's an overview of floating-point numbers in Python:

## Floating-Point Variables

You can assign floating-point values to variables:

```python
pi = 3.14159  # A floating-point number
price = 4.99  # Another floating-point number

```

## Mathematical Operation

Python supports various mathematical operations on floating-point numbers, such as addition, subtraction, multiplication, and division:

```python

a = 3.14
b = 1.5

addition_result = a + b  # Addition
subtraction_result = a - b  # Subtraction
multiplication_result = a * b  # Multiplication
division_result = a / b  # Division (result is a float)

```

## Scientific Notation

Floating-point numbers can also be expressed in scientific notation, using the e character to represent powers of 10:

Scientific Notation
Floating-point numbers can also be expressed in scientific notation, using the e character to represent powers of 10:

```python

large_number = 1.23e6  # 1.23 x 10^6
small_number = 4.56e-3  # 4.56 x 10^-3

```

## Rounding and Precision

Floating-point numbers in Python may have limited precision due to the way they are stored in memory. This can lead to rounding errors in calculations. To round a floating-point number, you can use the round() function:

```python

rounded_number = round(3.14159, 2)  # Rounds to two decimal places (result is 3.14)

```

## Type Conversions

You can convert other data types to floating-point numbers using the float() function. For example, converting a string to a floating-point number:

```python

x = "3.14"  # A string
y = float(x)  # Convert to a float

```

Floating-point numbers are essential for scientific and mathematical calculations in Python, and understanding their characteristics and potential limitations is crucial for accurate computation.

## # Complex Numbers in Python

Complex numbers are a data type in Python that represent numbers in the form of `a + bj`, where `a` and `b` are real numbers, and `j` represents the imaginary unit. Complex numbers are used for advanced mathematical and engineering calculations. Here's an overview of complex numbers in Python:

## Complex Number Variables

You can assign complex values to variables:

```python
z = 3 + 4j  # A complex number with real part 3 and imaginary part 4
w = 2 - 5j  # Another complex number with real part 2 and imaginary part -5`

```

## Mathematical Operations

Python supports various mathematical operations on complex numbers, including addition, subtraction, multiplication, division, and complex conjugation:

```python

z = 3 + 4j
w = 2 - 5j

addition_result = z + w  # Addition
subtraction_result = z - w  # Subtraction
multiplication_result = z * w  # Multiplication
division_result = z / w  # Division

conjugate_of_z = z.conjugate()  # Complex conjugate of z (3 - 4j)

```

## Built-in Function

Python provides built-in functions for working with complex numbers, such as abs() and real() to get the magnitude and real part of a complex number, respectively:

```python

magnitude = abs(z)  # Magnitude of z
real_part = z.real  # Real part of z

```

## Type Conversionz

You can convert other data types to complex numbers using the complex() function. For example, converting two floating-point numbers to a complex number:

```python

a = 2.5
b = -1.2
c = complex(a, b)  # Convert a and b to a complex number (2.5 - 1.2j)

```

Complex numbers are a powerful tool for solving problems that involve imaginary quantities, such as in electrical engineering, physics, and signal processing.

## # Strings (str) in Python

Strings are a fundamental data type in Python that represent text data. They are used for working with text, characters, and sequences of characters. Here's an overview of strings in Python:

## String Variables

You can assign string values to variables:

```python
name = "Alice"  # A string variable
message = 'Hello, World!'  # Another string variable

```

## String Quoting

Strings can be enclosed in single quotes, double quotes, or triple quotes:

```python

single_quoted = 'This is a single-quoted string.'
double_quoted = "This is a double-quoted string."
triple_quoted = '''This is a triple-quoted string that can span
multiple lines.'''

```

## String Indexing

Individual characters within a string can be accessed using indexing. Python uses zero-based indexing, so the first character is at index 0:

```python

text = "Hello"
first_character = text[0]  # Accesses the first character, 'H'
second_character = text[1]  # Accesses the second character, 'e'

```

## String Slicing

You can extract a substring from a string using slicing. Slicing allows you to specify a range of indices:

```python

text = "Hello, World!"
substring = text[7:12]  # Extracts "World"

```

## String Concatenation

Strings can be concatenated using the + operator:

```python

greeting = "Hello, "
name = "Alice"
full_greeting = greeting + name  # Concatenates the two strings

```

## String Length

You can find the length of a string using the len() function:

```python

text = "Python is fun!"
length = len(text)  # Returns the length of the string

```

## String Methods

Python provides many built-in string methods for manipulating and working with strings, such as upper(), lower(), strip(), split(), and more:

```python

text = "   Python Programming   "
uppercase_text = text.upper()  # Converts to uppercase
lowercase_text = text.lower()  # Converts to lowercase
stripped_text = text.strip()  # Removes leading and trailing whitespace
words = text.split()  # Splits the string into a list of words

```

## Escape Sequences

Escape sequences are used to represent special characters within strings, such as newline characters (\n) or tab characters (\t):

```python

escaped_text = "This is a line\nThis is another line"
tabbed_text = "Column 1\tColumn 2\tColumn 3"

```

Strings are a versatile data type in Python, and understanding their features and methods is essential for working with text data in various applications.

## Lambda Expressions in Python

Lambda expressions, also known as lambda functions or anonymous functions, are a way to create small, unnamed functions in Python. They are often used for short, simple operations that can be defined in a single line of code. Here's an overview of lambda expressions in Python:

## Basic Syntax

The basic syntax of a lambda expression consists of the `lambda` keyword followed by one or more arguments and an expression. The result of the expression is the return value of the lambda function:

```python

lambda arguments: expression

```

For example, a simple lambda function that adds two numbers:

```python

add = lambda x, y: x + y
result = add(3, 5)  # Result is 8

```

## Use Cases

Lambda expressions are often used when you need a small function for a short period and don't want to define a full-fledged named function. They are commonly used with functions like map(), filter(), and sorted() for quick operations on iterable data:

map()
The map() function applies a function to each item in an iterable:

```python

numbers = [1, 2, 3, 4, 5]
squared = list(map(lambda x: x ** 2, numbers))  # Square each number

```

## filter()

The filter() function filters items from an iterable based on a condition:

```python

numbers = [1, 2, 3, 4, 5]
even_numbers = list(filter(lambda x: x % 2 == 0, numbers))  # Filter even numbers

```

## sorted()

The sorted() function allows custom sorting using a key function:

```python

names = ["Alice", "Bob", "Charlie", "David"]
sorted_names = sorted(names, key=lambda x: len(x))  # Sort by name length

```

## Limitations

Lambda expressions are limited to a single expression and cannot contain statements or multiple lines of code. They are best suited for simple and short operations.

While lambda expressions can be powerful and concise, readability should also be considered. For complex or longer operations, it's often better to define a named function for clarity.

Lambda expressions are a useful tool in Python for creating small, on-the-fly functions when needed.

## Conventions for Docstrings in Python

Docstrings serve as documentation for Python functions, classes, and modules. They provide information about their purpose, usage, and parameters. Adhering to conventions for the content and formatting of docstrings is essential for maintaining clean and understandable code. Here are the key conventions:

## 1. Triple Quotes

Use triple quotes (either single or double) to enclose docstrings:

```python
def example_function():
    """
    This is an example docstring.
    It describes the purpose and usage of the function.
    """
    pass

```

## 2. Content

2.1. Brief Description
The first line of the docstring should provide a brief, one-line description of the function or module's purpose. This is known as the "one-liner" or "summary" line:

```python

def example_function():
    """
    This function calculates and returns the sum of two numbers.
    """
    pass

```

2.2. Detailed Description
Following the one-liner, you can provide a more detailed description of the function or module, explaining its behavior, input parameters, and output. It's common to leave a blank line after the one-liner:

```python

def example_function(x, y):
    """
    This function calculates and returns the sum of two numbers.

    Parameters:
        x (int): The first number.
        y (int): The second number.

    Returns:
        int: The sum of x and y.
    """
    return x + y

```

## 3. Parameters

For functions, list the parameters, their types, and descriptions in the "Parameters" section. Use a consistent format such as:

```python

Parameters:
    parameter_name (parameter_type): Description of the parameter.

```

## 4. Returns

For functions, describe the return value in the "Returns" section:

```python

Returns:
    return_type: Description of the return value.

```

## 5. Other Sections

Depending on the complexity of the function or module, you can include additional sections such as "Raises" (for exceptions raised), "Examples," or "Notes."

## 6. PEP 257

Follow PEP 257 for more detailed guidance on docstring conventions.

By following these conventions, you ensure that your code is well-documented, making it easier for you and others to understand and maintain. Good documentation is essential for code readability and maintainability.
