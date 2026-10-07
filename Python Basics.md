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

### Key Takeaways
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

---

### 💡 Key Takeaways
- Selecting the correct data type optimizes execution speed and memory usage[cite: 15].
- Converting between types via `int()`, `float()`, `str()`, and `bool()` is essential when handling raw inputs and structured datasets[cite: 16, 17].
