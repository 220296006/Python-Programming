# Objects and Classes

## Classes

A class in Python is a blueprint for creating objects. It defines a data structure that contains data members (variables) and methods (functions) that operate on those data members. Objects are instances of a class.

```python

class Dog:
    def __init__(self, name, age):
        self.name = name
        self.age = age

    def bark(self):
        print(f"{self.name} says Woof!")

# Creating an object (instance) of the Dog class
my_dog = Dog("Buddy", 3)

# Accessing attributes and calling methods
print(f"{my_dog.name} is {my_dog.age} years old.")
my_dog.bark()

```

## Inheritance

Inheritance is a mechanism in which a new class inherits properties and behaviors from an existing class. The existing class is called the base class or parent class, and the new class is called the derived class or child class.

```python

class Animal:
    def __init__(self, species):
        self.species = species

    def make_sound(self):
        print("Some generic sound")

class Cat(Animal):
    def __init__(self, name, breed):
        super().__init__("Cat")
        self.name = name
        self.breed = breed

    def make_sound(self):
        print(f"{self.name} says Meow!")

# Creating an object of the derived class
my_cat = Cat("Whiskers", "Siamese")

# Accessing attributes and calling methods
print(f"{my_cat.name} is a {my_cat.breed} {my_cat.species}.")
my_cat.make_sound()

```

## Private Classes

In Python, there's no strict enforcement of access modifiers like private or public. However, a convention is used to indicate that a variable or method should be treated as private.

A name prefixed with an underscore (e.g., _variable or _method()) implies that it is a non-public part of the API and should be used with caution.

```python

class Car:
    def __init__(self, make, model):
        self._make = make  # _make is considered internal, but can still be accessed
        self._model = model

    def _start_engine(self):
        print("Engine started")

# Creating an object of the class
my_car = Car("Toyota", "Camry")

# Accessing internal attributes (not recommended)
print(f"Make: {my_car._make}")
print(f"Model: {my_car._model}")

# Accessing internal method (not recommended)
my_car._start_engine()

```

I this example, '_make` and `_start_engine` are considered internal, but it's important to note that this is a convention, and the variables/methods can still be accessed. It's a signal to other developers that these parts of the class are intended for internal use.

## Private Variables

In Python, there's no strict concept of private variables, but a naming convention is used to indicate that a variable should be treated as private. By convention, a variable or method intended for internal use is prefixed with a single underscore (e.g., _variable).

Here's an example demonstrating the use of private variables:

```python
class BankAccount:
    def __init__(self, account_number, balance):
        self._account_number = account_number  # Private variable (by convention)
        self._balance = balance

    def get_account_number(self):
        return self._account_number

    def get_balance(self):
        return self._balance

    def deposit(self, amount):
        self._balance += amount

    def _withdraw(self, amount):  # Private method (by convention)
        if amount <= self._balance:
            self._balance -= amount
            print(f"Withdrawal of {amount} successful.")
        else:
            print("Insufficient funds.")

# Creating an object of the class
my_account = BankAccount(account_number="12345", balance=1000)

# Accessing private variables (not recommended)
print(f"Account Number: {my_account._account_number}")
print(f"Balance: {my_account._balance}")

# Accessing methods
print(f"Current Balance: {my_account.get_balance()}")
my_account.deposit(500)
print(f"Updated Balance after deposit: {my_account.get_balance()}")

# Attempting to access a private method (not recommended)
# This will work, but it's against the convention
my_account._withdraw(200)


```

In this example, `_account_number` and `_balance` are considered private variables, and `_withdraw` is a private method. However, it's important to note that this is a convention, and the variables/methods can still be accessed. It serves as a signal to other developers that these parts of the class are intended for internal use.
