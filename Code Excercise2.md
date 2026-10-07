#  Practice: Explicit Type Casting & Type Verification in Python

A hands-on implementation demonstrating explicit type conversion (typecasting) and validating variable data types using the built-in `type()` function in Python.

---

###  Problem Context
In data processing and pipeline development, raw incoming records often arrive in mismatched formats (e.g., numeric values stored as text strings). Explicit casting ensures values are parsed correctly before performing mathematical operations or database commits.

---

###  Python Implementation

```python
# 1. Convert string representation of an integer to a numerical int
string_number = "25"
int_number = int(string_number)
print(int_number, type(int_number))

# 2. Convert a floating-point number to a string
float_number = 3.149
str_pi = str(float_number)
print(str_pi, type(str_pi))

# 3. Convert a boolean state to a string representation
is_active = True
str_bool = str(is_active)
print(str_bool, type(str_bool))
```

---

###  Console Output

```text
25 <class 'int'>
3.149 <class 'str'>
True <class 'str'>
```

---

###  Technical Breakdown

| Original Value | Target Type | Constructor | Output Value | Data Class |
| :--- | :--- | :--- | :--- | :--- |
| `"25"` | Integer | `int()` | `25` | `<class 'int'>` |
| `3.149` | String | `str()` | `'3.149'` | `<class 'str'>` |
| `True` | String | `str()` | `'True'` | `<class 'str'>` |

---

###  Key Points:
- The `type()` function outputs the object class (e.g., `<class 'int'>`, `<class 'str'>`), confirming whether conversion was successful.
- Converting strings to numbers enables arithmetic operations, while converting values to strings allows concatenation and text-based logging.
