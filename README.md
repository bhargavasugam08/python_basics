# Python Fundamentals

This repository contains a beginner-friendly Jupyter Notebook that explains the basic concepts of Python with simple examples.

Notebook: [`python_fundamentals.ipynb`](./python_fundamentals.ipynb)

## What This Notebook Teaches

### 1. Variables and Data Types

A variable is a name used to store a value.

```python
name = "name"
age = 27
cgpa = 9.8
is_student = True
```

Python automatically identifies the type of each value:

- `int` — whole numbers, such as `27`
- `float` — decimal numbers, such as `9.8`
- `str` — text, such as `"name"`
- `bool` — either `True` or `False`

The `type()` function can be used to check the type of a value.

```python
print(type(age))
print(type(name))
```

### 2. User Input and Type Casting

The `input()` function allows a user to enter a value. Input is always received as text, even when the user enters a number.

```python
age = "27"
print(type(age))  # string
```

To use the value as a number, it must be converted:

```python
new_age = int(age) + 1
print(new_age)  # 28
```

Common conversion functions include:

- `int()` — converts a value to an integer
- `float()` — converts a value to a decimal number
- `str()` — converts a value to text

The notebook also demonstrates the difference between explicit conversion and automatic conversion by Python.

### 3. Strings

A string is a sequence of characters used to represent text.

```python
name = "name"
```

The notebook demonstrates common string operations:

```python
print(name.upper())              # NAME
print(name.lower())              # name
print(name.find("n"))            # position of n
print(name.replace("n", "g"))    # game
print("a" in name)               # True
```

Strings are immutable. This means that string methods return a new string instead of changing the original string.

### 4. Operators

Operators are symbols used to perform calculations and comparisons.

#### Arithmetic Operators

```python
print(5 + 5)   # addition
print(5 - 2)   # subtraction
print(5 * 4)   # multiplication
print(5 / 3)   # division
print(5 // 3)  # floor division
print(5 % 3)   # remainder
print(5 ** 3)  # power
```

#### Assignment Operators

Assignment operators update the value of a variable.

```python
x = 1
x += 5  # same as x = x + 5
print(x)
```

The notebook also introduces `-=`, `*=`, and other assignment operators.

#### Comparison Operators

Comparison operators compare two values and return either `True` or `False`.

```python
print(3 > 2)   # True
print(2 == 2)  # True
print(2 != 5)  # True
```

The notebook explains the difference between `=` and `==`:

- `=` assigns a value
- `==` checks whether two values are equal

#### Logical Operators

Logical operators combine conditions:

- `and` — both conditions must be true
- `or` — at least one condition must be true
- `not` — changes `True` to `False` and `False` to `True`

```python
print(True and False)  # False
print(True or False)   # True
print(not True)        # False
```

#### Operator Precedence

Python follows an order when evaluating expressions. Parentheses are evaluated first, followed by powers, multiplication or division, and then addition or subtraction.

```python
print(2 + 5 * 3)      # 17
print((2 + 5) * 3)    # 21
```

### 5. Conditional Statements

Conditional statements allow a program to make decisions using `if`, `elif`, and `else`.

```python
age = 14

if age >= 18:
    print("adult")
elif age < 18:
    print("not adult")
```

Python uses indentation to show which statements belong to a condition.

The notebook also demonstrates how conditions can be used to assign grades based on marks.

### 6. Loops

Loops repeat a block of code multiple times.

#### The `range()` Function

`range()` generates a sequence of numbers. The ending value is not included.

```python
print(list(range(5)))  # [0, 1, 2, 3, 4]
```

#### `while` Loop

A `while` loop continues as long as its condition is true.

```python
counter = 1

while counter <= 5:
    print("name")
    counter += 1
```

The counter must be updated so that the loop eventually stops.

#### `for` Loop

A `for` loop is used to go through a sequence of values.

```python
for i in range(5):
    print(i)
```

The notebook also shows how to print even numbers and how to use the step value in `range()`.

#### `break` and `continue`

- `break` stops a loop completely.
- `continue` skips the current repetition and continues with the next one.

```python
for i in range(1, 31):
    if i == 21:
        continue
    print(i)
```

### 7. Data Structures

Data structures are used to store multiple values.

- **List** — ordered and changeable collection
- **Tuple** — ordered collection that cannot be changed
- **Set** — collection of unique values
- **Dictionary** — stores data as key-value pairs

Examples:

```python
numbers = [1, 2, 3]                 # list
coordinates = (10, 20)              # tuple
unique_numbers = {1, 2, 3}          # set
student = {"name": "Alex", "age": 20}  # dictionary
```

### 8. Functions

A function is a reusable block of code. Functions help prevent repeated code and make programs easier to organize.

```python
def greet(name):
    print("Hello", name)


greet("Alex")
```

The notebook introduces how to define functions with `def` and how to call them with different values.

## In Simple Words

The notebook explains the main building blocks of Python:

- Variables store information.
- Data types describe the kind of information being stored.
- Operators perform calculations and comparisons.
- Conditions help programs make decisions.
- Loops repeat instructions.
- Data structures organize collections of values.
- Functions group reusable instructions together.

Together, these concepts form the foundation for writing Python programs.

## Running the Notebook

You can open the notebook directly on GitHub or run it locally with Jupyter Notebook or JupyterLab.

```bash
git clone https://github.com/bhargavasugam08/python_basics.git
cd python_basics
python -m pip install notebook
jupyter notebook
```

Then open `python_fundamentals.ipynb` and run the cells from top to bottom.
