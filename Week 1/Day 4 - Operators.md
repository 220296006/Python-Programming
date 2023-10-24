# Operators in Python

Operators are special symbols in Python used to perform operations on variables and values. Python supports a wide range of operators for various operations, such as arithmetic, comparison, logical, and more. Here's an overview of operators in Python:

## Arithmetic Operators

Arithmetic operators are used for mathematical calculations:

```python
x = 10
y = 5

addition = x + y  # Addition
subtraction = x - y  # Subtraction
multiplication = x * y  # Multiplication
division = x / y  # Division
modulo = x % y  # Modulo (remainder)
exponentiation = x ** y  # Exponentiation
floor_division = x // y  # Floor Division (result is rounded down)

```

## Comparison Operators

Comparison operators are used to compare values and return Boolean results:

```python

x = 10
y = 5

equal = x == y  # Equal
not_equal = x != y  # Not Equal
greater_than = x > y  # Greater Than
less_than = x < y  # Less Than
greater_than_or_equal = x >= y  # Greater Than or Equal
less_than_or_equal = x <= y  # Less Than or Equal

```

## Logical Operators

Logical operators are used for combining Boolean values:

```python

x = True
y = False

logical_and = x and y  # Logical AND
logical_or = x or y  # Logical OR
logical_not = not x  # Logical NOT

```

## Assignment Operators

Assignment operators are used to assign values to variables:

```python

x = 10

x += 5  # Equivalent to x = x + 5
x -= 5  # Equivalent to x = x - 5
x *= 5  # Equivalent to x = x * 5
x /= 5  # Equivalent to x = x / 5
x %= 5  # Equivalent to x = x % 5
x **= 5  # Equivalent to x = x ** 5
x //= 5  # Equivalent to x = x // 5

```

## Identity Operators

Identity operators are used to compare the memory locations of objects:

```python

x = [1, 2, 3]
y = [1, 2, 3]

is_operator = x is y  # True if x and y are the same object
is_not_operator = x is not y  # True if x and y are different objects

```

## Membership Operators

Membership operators are used to test if a sequence is present in an object:

```python

sequence = [1, 2, 3, 4, 5]

in_operator = 3 in sequence  # True if 3 is in the sequence
not_in_operator = 6 not in sequence  # True if 6 is not in the sequence

```

## Bitwise Operators

Bitwise operators are used for binary operations on integers:

```python

x = 5
y = 3

bitwise_and = x & y  # Bitwise AND
bitwise_or = x | y  # Bitwise OR
bitwise_xor = x ^ y  # Bitwise XOR
bitwise_not = ~x  # Bitwise NOT
bitwise_left_shift = x << 2  # Bitwise Left Shift
bitwise_right_shift = x >> 1  # Bitwise Right Shift

```

Understanding and using operators is fundamental to performing a wide range of operations and calculations in Python.

#