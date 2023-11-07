# Control Flow in Python

Control flow structures are fundamental in programming, allowing you to control the flow and execution of your code based on conditions. Python provides various control flow statements and structures to help you achieve this. Here's an overview of control flow in Python:

## Conditional Statements

### 1. `if` Statements

The `if` statement is used to execute a block of code if a condition is true:

```python

x = 10
if x > 5:
    print("x is greater than 5")

```

### 2. `if-else` Statements

The if-else statement allows you to specify an alternative block of code to execute when the condition is false:

```python
x = 3
if x > 5:
    print("x is greater than 5")
else:
    print("x is not greater than 5")

```

### 3. `if-elif-else` Statements

The if-elif-else statement is used when you have multiple conditions to check:

```python
x = 5
if x > 5:
    print("x is greater than 5")
elif x < 5:
    print("x is less than 5")
else:
    print("x is equal to 5")


```

## Loops

### 4. `for` Loop

The for loop is used to iterate over a sequence (e.g., a list or string) or any iterable:

```python

fruits = ["apple", "banana", "cherry"]
for fruit in fruits:
    print(fruit)

```

### 5. `while` Loop

The while loop is used to repeatedly execute a block of code as long as a condition is true:

```python

count = 0
while count < 5:
    print("Count is", count)
    count += 1

```

### 6. break Statement

The break statement is used to exit a loop prematurely based on a condition:

```python

count = 0
while count < 5:
    print("Count is", count)
    count += 1

```

### 7. `continue` Statement

The continue statement is used to skip the current iteration of a loop and move to the next:

```python

fruits = ["apple", "banana", "cherry"]
for fruit in fruits:
    if fruit == "banana":
        continue
    print(fruit)

```

## Control Flow in Functions

### 8. `return` Statement

The return statement is used in functions to return a value to the caller:

```python

def add(x, y):
    return x + y
result = add(3, 4)  # result is 7

```

Control flow structures are essential for building complex programs and implementing decision-making and repetition. They allow you to control the logic and flow of your code.