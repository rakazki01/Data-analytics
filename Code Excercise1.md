#  Practice Problem: Inventory Tracking with Variables & Expressions

A beginner friendly practical demonstration showing how to manage incoming supplies, daily usage, and inventory balances using Python variables and arithmetic expressions.

---

###  Problem Statement
A small kitchen tracks egg consumption over three consecutive days:
- Calculate total units purchased.
- Calculate total units consumed.
- Determine the remaining inventory at the end of Day 3.

---

###  Python Implementation

```python
# Daily purchases
egg_day1 = 12
egg_day2 = 10
egg_day3 = 8

# Total inventory acquired
total_eggs_bought = egg_day1 + egg_day2 + egg_day3
print("Total eggs bought in 3 days:", total_eggs_bought)

# Daily consumption
used_day1 = 5
used_day2 = 6
used_day3 = 4

# Total inventory used
total_eggs_used = used_day1 + used_day2 + used_day3
print("Total eggs used in 3 days:", total_eggs_used)

# Remaining stock calculation
remaining_eggs = total_eggs_bought - total_eggs_used
print("Remaining eggs after 3 days:", remaining_eggs)
```

---

###  Console Output

```text
Total eggs bought in 3 days: 30
Total eggs used in 3 days: 15
Remaining eggs after 3 days: 15
```

---

### The Concept Breakdown

| Component | Code Reference | Description |
| :--- | :--- | :--- |
| **Operands** | `12`, `10`, `8` / `used_day1`, etc. | Data values fed into mathematical operations. |
| **Operators** | `+`, `-` | Arithmetic symbols computing cumulative totals and differences. |
| **Variable Reuse** | `total_eggs_bought - total_eggs_used` | Evaluates new expressions using previously defined variable results. |
