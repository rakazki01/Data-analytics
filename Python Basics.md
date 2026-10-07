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
