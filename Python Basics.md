# 🐍 Python Fundamentals: Variables, Expressions & Operators

A concise breakdown of data storage, expressions, and evaluation in Python.

---

### 1. Understanding Variables
A variable is a **named storage location in memory** used to hold data that can be updated or reused[cite: 13].

```python
age = 25              # Assigning an integer value to a variable
name = "Alice"        # Assigning a string value to a variable
pi = 3.14159          # Assigning a floating-point value to a variable
is_active = True      # Assigning a boolean value to a variable
```
*(Variable assignment examples[cite: 13])*

---

### 2. Understanding Expressions, Operands & Operators
An expression in Python is a **combination of values, variables, operators, and function calls** that the interpreter can evaluate to produce a result[cite: 11, 12].

- **Operands:** The values or variables on which operation is performed. In `5 + 3`, the operands are `5` and `3`[cite: 12].
- **Operator:** Symbols that represent specific operations. In `5 + 3`, the operator is `+`[cite: 12].

```python
5 + 3              # Adds 5 and 3
x * 7              # Multiplies the value of x by 7
(a + b) / 2        # Calculates the average of a and b
len("Hello")       # Finds the length of the string "Hello"
```
*(Common expression patterns[cite: 11, 12])*

---

### 3. Expression within Variables
Variables can hold the results of any valid expression, making Python programs dynamic, flexible, and maintainable[cite: 14].

#### Example 1: Storing the result of a simple expression[cite: 14]
```python
result = 5 + 3
print(result)       # Output: 8
```
*(Storing expression output[cite: 14])*

#### Example 2: Using variables in expressions[cite: 14]
```python
a = 10
b = 20
sum_value = a + b
print(sum_value)    # Output: 30
```
*(Evaluating expressions with existing variables[cite: 14])*

---

### Key Understanding:
- Variables can hold results of any valid expression[cite: 14].
- Expressions make Python programs dynamic and flexible[cite: 14].
- Reusing variables in expressions allows for concise and maintainable code[cite: 14].

- # 🐍 Python Fundamentals: Data Types & Type Casting

A comprehensive reference on Python's core data types and explicit type conversion methods.

---

### 1. Understanding Data Types
Data types define the **type of data a variable can hold**, specifying how the interpreter processes it[cite: 15].

- **Purpose:** Ensures efficient memory allocation and enables proper data manipulation[cite: 15].

| Data Type | Description | Example Values |
| :--- | :--- | :--- |
| **Integer (`int`)** | Whole numbers without decimals[cite: 15] | `5`, `-20`[cite: 15] |
| **Float (`float`)** | Fractional numbers with decimal points[cite: 15] | `3.14`, `-7.89`[cite: 15] |
| **String (`str`)** | Text data enclosed in quotes[cite: 15] | `"Hello"`, `'Python'`[cite: 15] |
| **Boolean (`bool`)** | Logical truth values[cite: 15] | `True`, `False`[cite: 15] |

---

### 2. What is Type Casting?
Typecasting is the **process of converting one data type into another**[cite: 16].

#### Core Conversion Functions:
- `int()` – Converts data to an integer[cite: 16].
- `float()` – Converts data to a float[cite: 16].
- `str()` – Converts data to a string[cite: 16].
- `bool()` – Converts data to a Boolean[cite: 16].

---

### 3. Practical Type Casting Examples

```python
# 1. Integer to Float
num = 10
num_float = float(num)
print(num_float)       # Output: 10.0

# 2. Float to Integer (Truncates decimal)
pi = 3.14
pi_int = int(pi)
print(pi_int)          # Output: 3

# 3. String to Integer
text = "123"
number = int(text)
print(number)          # Output: 123

# 4. Any Type to Boolean
is_empty = bool("")
print(is_empty)        # Output: False
```
*(Code examples demonstrating explicit type casting between integer, float, string, and boolean[cite: 17])*

# 🔤 Python Fundamentals: Complete String Manipulation Guide

A comprehensive breakdown of string properties, indexing, slicing, escape formatting, and common built-in methods in Python.

---

### 1. String Definition & Formats
A string is a **sequence of characters enclosed in quotes**, representing text data in Python. Strings are **immutable**, meaning they cannot be modified after creation.

- **Word String:** Contains a single word (e.g., `"Python"`).
- **String with Spaces:** Contains multiple words separated by spaces (e.g., `"Learn Python Programming"`).
- **String with Numbers:** Includes numeric characters treated strictly as text (e.g., `"12345"`, `"Python3"`).

---

### 2. Forward & Backward Indexing
Each character in a string can be accessed using its numerical index position:
- **Forward Indexing:** Starts from `0` at the beginning of the string.
- **Backward (Negative) Indexing:** Starts from `-1` representing the last character, `-2` for the second to last, and so on.

| Character | P | y | t | h | o | n |
| :--- | :---: | :---: | :---: | :---: | :---: | :---: |
| **Forward Index** | `0` | `1` | `2` | `3` | `4` | `5` |
| **Negative Index** | `-6` | `-5` | `-4` | `-3` | `-2` | `-1` |

```python
my_string = "Python"

# Forward indexing
print(my_string[0])     # Output: 'P'
print(my_string[3])     # Output: 'h'

# Negative indexing
print(my_string[-1])    # Output: 'n'
print(my_string[-4])    # Output: 't'
```

---

### 3. Slicing & Striding
Extract subsets of characters using indexing boundaries:

- **Slicing Syntax:** `string[start : end]` *(Note: `end` index is exclusive)*.
- **Striding Syntax:** `string[start : end : step]` *(Defines step interval between characters)*.

```python
my_string = "Programming"

# Slicing: Extracts indices 0 through 5
sliced = my_string[0:6]
print(sliced)           # Output: 'Progra'

# Striding: Skips every second character
strided = my_string[0:11:2]
print(strided)          # Output: 'Pormig'
```

---

### 4. String Operations & Escape Sequences

#### String Length (`len()`):
Returns the total character count (including spaces and symbols).
```python
my_string = "Python"
print(len(my_string))   # Output: 6
```

#### Concatenation (`+`):
Joins two or more strings together using the `+` operator.
```python
string1 = "Hello"
string2 = "World"
result = string1 + " " + string2
print(result)           # Output: 'Hello World'
```

#### Escape Sequences:
Used to represent special formatting inside string literals:
- `\n`: Inserts a newline.
- `\t`: Inserts a horizontal tab.

```python
print("Hello\nWorld")          # Prints 'Hello' and 'World' on separate lines
print("Python\tProgramming")   # Prints with tab spacing between words
```

---

### 5. Essential Built-in String Methods

#### Case Conversion (`upper()` & `lower()`):
Converts all characters to uppercase or lowercase without altering the original string.
```python
my_string = "Python"
print(my_string.upper())   # Output: 'PYTHON'
print(my_string.lower())   # Output: 'python'
```

#### Replacing Substrings (`replace()`):
Replaces all occurrences of a specified substring with a new string.
- **Syntax:** `string.replace(old, new)`

```python
my_string = "I love Python"
replaced = my_string.replace("Python", "Programming")
print(replaced)            # Output: 'I love Programming'
```

---

### 💡 Key Takeaways
- Python strings use zero-based indexing for standard traversal and negative indices for reverse traversal.
- Slicing boundaries follow an open interval `[start, end)` where the stop index is excluded.
- Because strings are immutable, methods like `.upper()`, `.lower()`, and `.replace()` return new strings rather than altering the original variable in place.

---

### 💡 Key Takeaways
- Selecting the correct data type optimizes execution speed and memory usage[cite: 15].
- Converting between types via `int()`, `float()`, `str()`, and `bool()` is essential when handling raw inputs and structured datasets[cite: 16, 17].
