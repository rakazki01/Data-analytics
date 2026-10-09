# 🐍 Python Fundamentals: Variables, Expressions & Operators

A concise breakdown of data storage, expressions, and evaluation in Python.

---

### 1. Understanding Variables
A variable is a **named storage location in memory** used to hold data that can be updated or reused.

```python
age = 25              # Assigning an integer value to a variable
name = "Alice"        # Assigning a string value to a variable
pi = 3.14159          # Assigning a floating-point value to a variable
is_active = True      # Assigning a boolean value to a variable
```
*(Variable assignment examples)*

---

### 2. Understanding Expressions, Operands & Operators
An expression in Python is a **combination of values, variables, operators, and function calls** that the interpreter can evaluate to produce a result.

- **Operands:** The values or variables on which operation is performed. In `5 + 3`, the operands are `5` and `3`.
- **Operator:** Symbols that represent specific operations. In `5 + 3`, the operator is `+`.

```python
5 + 3              # Adds 5 and 3
x * 7              # Multiplies the value of x by 7
(a + b) / 2        # Calculates the average of a and b
len("Hello")       # Finds the length of the string "Hello"
```
*(Common expression patterns)*

---

### 3. Expression within Variables
Variables can hold the results of any valid expression, making Python programs dynamic, flexible, and maintainable.

#### Example 1: Storing the result of a simple expression
```python
result = 5 + 3
print(result)       # Output: 8
```
*(Storing expression output)*

#### Example 2: Using variables in expressions
```python
a = 10
b = 20
sum_value = a + b
print(sum_value)    # Output: 30
```
*(Evaluating expressions with existing variables)*

---

### Key Understanding:
- Variables can hold results of any valid expression.
- Expressions make Python programs dynamic and flexible.
- Reusing variables in expressions allows for concise and maintainable code.

# 🐍 Python Fundamentals: Data Types & Type Casting

A comprehensive reference on Python's core data types and explicit type conversion methods.

---

### 1. Understanding Data Types
Data types define the **type of data a variable can hold**, specifying how the interpreter processes it.

- **Purpose:** Ensures efficient memory allocation and enables proper data manipulation.

| Data Type | Description | Example Values |
| :--- | :--- | :--- |
| **Integer (`int`)** | Whole numbers without decimals | `5`, `-20` |
| **Float (`float`)** | Fractional numbers with decimal points | `3.14`, `-7.89` |
| **String (`str`)** | Text data enclosed in quotes | `"Hello"`, `'Python'` |
| **Boolean (`bool`)** | Logical truth values | `True`, `False` |

---

### 2. What is Type Casting?
Typecasting is the **process of converting one data type into another**.

#### Core Conversion Functions:
- `int()` – Converts data to an integer.
- `float()` – Converts data to a float.
- `str()` – Converts data to a string.
- `bool()` – Converts data to a Boolean.

---

### 3. Practical Type Casting Examples

```python
# 1. Integer to Float
num = 10
num_float = float(num)
print(num_float)       # Output: 10.0

# 2. Float to Integer 
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
*(Code examples demonstrating explicit type casting between integer, float, string, and boolean)*

---

### 💡 Key Understanding:
- Selecting the correct data type optimizes execution speed and memory usage.
- Converting between types via `int()`, `float()`, `str()`, and `bool()` is essential when handling raw inputs and structured datasets.


# 🐍 Python Fundamentals: Complete String Manipulation Guide

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

### 💡 Key Understanding:
- Python strings use zero-based indexing for standard traversal and negative indices for reverse traversal.
- Slicing boundaries follow an open interval `[start, end]` where the stop index is excluded.
- Because strings are immutable, methods like `.upper()`, `.lower()`, and `.replace()` return new strings rather than altering the original variable in place.

# 🐍 Python Hands-on: String Operations & Manipulations Practice

A practical implementation showcasing fundamental string operations, including positive and negative indexing, slicing, striding, string length evaluation, concatenation, escape character formatting, and built-in case and replace methods.

---

###  Code Implementations & Outputs

#### 1. Forward & Backward Indexing
Accessing characters using zero-based positive index and negative reverse index.

```python
python = "PYTHON"

# Extract character at index 3 (4th position)
python = python[3]
print(python)
# Output: 'H'

# Extract second-to-last character using negative indexing
python = "PYTHON"
secondlast_chr = python[-2]
print(secondlast_chr)
# Output: 'O'
```
*(Code and output based on notebook implementations)*

---

#### 2. Slicing & Striding
Extracting specific substrings and skipping characters with custom step sizes.

```python
python = "PYTHON"

# Extract substring "THON" using slicing
extract_thon = python[2:6]
print(extract_thon)
# Output: 'THON'

# Extract every second character starting from index 0
everysecond_chr = python[0:5:2]
print(everysecond_chr)
# Output: 'PTO'
```
*(Code and output based on notebook implementations)*

---

#### 3. Length Evaluation & String Concatenation
Measuring total string character count and merging string variables.

```python
python = "PYTHON"

# Evaluating string length
print(len("PYTHON"))
# Output: 6

# Combining string variables with a space separator
python_a = "hello"
python_b = "world"
complete = "hello" + " " + "world"
print(complete)
# Output: 'hello world'
```
*(Code and output based on notebook implementations)*

---

#### 4. Escape Sequences, Case Transformation & Replacement
Formatting layout with escape characters, altering string casing, and updating substrings.

```python
# Escape sequences: newline (\n) and tab (\t)
print("hello\n\tworld")
# Output:
# hello
# 	world

# Case conversion methods
python = "python"
print(python.upper())
# Output: PYTHON

python = "PYTHON"
print(python.lower())
# Output: python

# Substring replacement
python = "I LOVE FOOD"
python = python.replace("FOOD", "GYM")
print(python)
# Output: 'I LOVE GYM'
```
*(Code and output based on notebook implementations)*

---

###  Operations Summary chart:

| Category | Syntax / Method | Executed Example | Output |
| :--- | :--- | :--- | :--- |
| **Forward Indexing** | `str[i]` | `"PYTHON"[3]` | `'H'` |
| **Negative Indexing** | `str[-i]` | `"PYTHON"[-2]` | `'O'` |
| **Slicing** | `str[start:end]` | `"PYTHON"[2:6]` | `'THON'` |
| **Striding** | `str[start:end:step]` | `"PYTHON"[0:5:2]` | `'PTO'` |
| **Length** | `len(str)` | `len("PYTHON")` | `6` |
| **Concatenation** | `+` | `"hello" + " " + "world"` | `'hello world'` |
| **Escape Formatting**| `\n`, `\t` | `"hello\n\tworld"` | Multiline tabbed text |
| **Uppercase** | `.upper()` | `"python".upper()` | `'PYTHON'` |
| **Lowercase** | `.lower()` | `"PYTHON".lower()` | `'python'` |
| **Replace** | `.replace(old, new)` | `"I LOVE FOOD".replace("FOOD", "GYM")` | `'I LOVE GYM'` |

# 🐍 Python Data Structures: Hands-On Guide to Tuples & Lists

A complete reference combining theoretical concepts and practical Jupyter Notebook implementations covering creation, immutability, mutability, concatenation, indexing, slicing, striding, nested hierarchies, and list modifications.

---

### 1. Conceptual Breakdown: Tuples vs. Lists

| Feature | Tuples (`tuple`) | Lists (`list`) |
| :--- | :--- | :--- |
| **Mutability** | **Immutable** (read-only sequence) | **Mutable** (modifiable in place) |
| **Syntax** | Parentheses `()` | Square brackets `[]` |
| **Ordering** | Ordered sequence | Ordered sequence |
| **Duplicates** | Allowed | Allowed |
| **Element Types** | Heterogeneous (int, str, float, etc.) | Heterogeneous (int, str, float, etc.) |

---

### 2. Practical Tuples: Code & Notebook Outputs

#### A. Creation & Concatenation
Tuples store multiple items in a single variableand combine through concatenation (`+` operator).

```python
# Creating a tuple
tuples = ("snacks", "soda", "drink")
print(tuples)
# Output: ('snacks', 'soda', 'drink')

# Combining two tuples using '+'
item1 = (1, 2, 3)
item2 = (4, 5, 6)
total = item1 + item2
print(total)
# Output: (1, 2, 3, 4, 5, 6)
```
*(Code and console outputs executed in workbook)*

#### B. Slicing Tuples
Extracting subsets using `tuple[start:end]` (start inclusive, end exclusive).

```python
item = (1, 2, 3, 4, 5, 6)
sliced_item = item[0:5]
print(sliced_item)
# Output: (1, 2, 3, 4, 5)
```
*(Code and console outputs executed in workbook)*

#### C. Nested Tuples
Tuples containing inner tuples accessed via coordinate indexing.

```python
nested = (("a", "b", "c"), (1, 2, 3), ("zz", "bc", "kk"))

# Accessing inner tuple at index 1
print(nested[1])
# Output: (1, 2, 3)

# Accessing inner tuple at index 2
print(nested[2])
# Output: ('zz', 'bc', 'kk')
```
*(Code and console outputs executed in workbook)*

---

### 3. Practical Lists: Code & Notebook Outputs

#### A. Creation & Backward Slicing
Lists are defined with square brackets and support negative indices for reverse traversal.

```python
# Creating a list
my_list = [1, 2, 3]
print(my_list)
# Output: [1, 2, 3]

# Backward slicing with negative indexing
fruits_list = ["apple", "orange", "guava"]
sliced_list = fruits_list[-2:-1]
print(sliced_list)
# Output: ['orange']
```
*(Code and console outputs executed in workbook)*

#### B. List Striding
Skipping items along an index boundary using `list[start:end:step]`.

```python
num_list = [10, 20, 30, 40, 50, 60]

# Slicing from index 0 to 3 with step 2
strided_list = num_list[0:3:2]
print(strided_list)
# Output: [10, 30]
```
*(Code and console outputs executed in workbook)*

#### C. Nested List Slicing
Sub-setting collections of lists within parent lists.

```python
nested_list = [[0, 1, 2], ["a", "b", "c"], [0.1, 0.2, 0.3]]

# Extracting first two sub-lists
sliced_nested_list = nested_list[0:2]
print(sliced_nested_list)
# Output: [[0, 1, 2], ['a', 'b', 'c']]
```
*(Code and console outputs executed in workbook)*

#### D. Dynamic Modifications (Append & Remove)
Modifying mutable list instances directly in memory.

```python
# Appending an item to the end
items = [1, 2, 3]
items.append(4)
print(items)
# Output: [1, 2, 3, 4]

# Removing a specific value
nums = [0, 1, 2, 3, 4]
nums.remove(3)
print(nums)
# Output: [0, 1, 2, 4]
```
*(Code and console outputs executed in workbook)*

---

### KEY UNDERSTANDING: 
- **Tuples** guarantee data integrity for fixed reference collections where accidental modification must be prevented.
- **Lists** provide flexible dynamic collections for data cleaning, transformation pipelines, and runtime updates.
- Both support multi-dimensional **nesting**, bounded **slicing**, and **striding**.


# 🐍 Python Data Structures: Hands-On Guide to Sets

A complete reference combining theoretical concepts and practical Jupyter Notebook implementations covering set definition, uniqueness, list-to-set deduplication, element addition, removal methods, union, and intersection operations.

---

### 1. Conceptual Breakdown: What is a Set?

A **set** is a built-in Python data structure used to store collections of data:
- **Unique Elements:** Duplicate entries are automatically stripped out.
- **Unordered:** Elements have no fixed position; indexing and slicing are **not** supported.
- **Mutable Structure:** While the set itself can be modified (elements added or removed), it only holds immutable, hashable items like numbers, strings, or tuples.
- **Syntax:** Defined using curly brackets `{}` or the `set()` constructor.

---

### 2. Practical Implementations & Notebook Outputs

#### A. Creation & Automatic Deduplication
Duplicate values passed into a set are automatically collapsed into unique entries.

```python
# Direct set creation with duplicate values
my_set = {1, 2, 2, 3, 4, 5}
print(my_set)
# Output: {1, 2, 3, 4, 5}
```
*(Duplicate values like `2` are discarded immediately)*

#### B. Deduplicating a List (`list` to `set`)
Passing any sequence into `set()` removes duplicates efficiently.

```python
# Convert a list containing duplicates into a set
my_list = [1, 2, 2, 3, 4, 4, 5]
my_set = set(my_list)

print("orignal list:", my_list)
# Output: orignal list: [1, 2, 2, 3, 4, 4, 5]

print("set:", my_set)
# Output: set: {1, 2, 3, 4, 5}
```
*(Demonstration of list-to-set type conversion)*

#### C. Adding Elements (`add()` vs. `update()`)
- `add()`: Appends a **single** element.
- `update()`: Inserts **multiple** elements from an iterable (e.g., list or tuple).

```python
my_set = {1, 2, 3, 4, 5}

# Adding a single items
my_set.add(6)

# Adding multiple items at once
my_set.update([7, 8])

print("new_set:", my_set)
# Output: new_set: {1, 2, 3, 4, 5, 6, 7, 8}
```
*(Expanding set elements using single and batch methods)*

#### D. Removing Elements (`remove()` vs. `discard()`)
- `remove()`: Deletes the item, but **raises a `KeyError`** if the item does not exist.
- `discard()`: Deletes the item if present, but **fails silently without error** if absent.

```python
# Using remove()
my_set = {1, 2, 3, 4, 5, 6}
my_set.remove(1)
print("removed set:", my_set)
# Output: removed set: {2, 3, 4, 5, 6}

# Using discard()
my_set = {1, 2, 3, 4, 5}
my_set.discard(2)
print("new set:", my_set)
# Output: new set: {1, 3, 4, 5}

# Discarding a non-existent element raises no error
my_set.discard(10)
print("After discard(10):", my_set)
# Output: After discard(10): {1, 3, 4, 5}
```
*(Safe versus strict item removal behaviors)*

#### E. Set Operations: Union & Intersection
- **Union (`|` or `.union()`):** Merges all unique items across sets.
- **Intersection (`&` or `.intersection()`):** Filters only shared common elements.

```python
set_1 = {1, 2, 3}
set_2 = {3, 4, 5}

# Intersection using & operator
new_set = set_1 & set_2
print("new_set:", new_set)
# Output: new_set: {3}

# Union using | operator or .union()
union_set = set_1 | set_2
print("Union:", union_set)
# Output: Union: {1, 2, 3, 4, 5}
```
*(Venn diagram set operations implemented via operators)*

---

### 📋 Methods & Syntax Reference

| Operation | Syntax / Method | Behavior | Error Handling |
| :--- | :--- | :--- | :--- |
| **Deduplication** | `set(iterable)` | Extracts unique values from sequence | N/A |
| **Add Single** | `set.add(item)` | Inserts single element | N/A |
| **Add Multiple** | `set.update(iterable)` | Inserts all elements from iterable | N/A |
| **Strict Delete** | `set.remove(item)` | Deletes specified item | Raises `KeyError` if item missing |
| **Safe Delete** | `set.discard(item)` | Deletes specified item | Silent (no error if item missing) |
| **Union** | `s1 \| s2` or `s1.union(s2)` | Combines all unique items across sets | N/A |
| **Intersection** | `s1 & s2` or `s1.intersection(s2)` | Extracts only elements present in both sets | N/A |

---

### KEY UNDERSTANDING:
- Sets provide average time complexity for membership testing (`in`), making them faster than lists for lookup tasks.
- Perfect for **data cleaning pipelines** when filtering out duplicate patient IDs, batch records, or categorical labels.

