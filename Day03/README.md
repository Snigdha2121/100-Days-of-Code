# Day 3: Python Notes

## 1. Conditional Statements

### Syntax of Conditional Statements
The basic syntax for conditional statements is as follows:
### `if` Statement

The `if` statement allows you to execute a block of code if a specified condition is `True`.

**Syntax:**

```python
if condition:
    # code to execute if the condition is True
```


### `if-else` Statement

The `if-else` statement allows you to execute one block of code if a condition is `True` and another block if the condition is `False`.

**Syntax:**

```python
if condition:
    # code to execute if the condition is True
else:
    # code to execute if the condition is False
```

### `if-elif-else` Statement


The `if-elif-else` statement allows you to check multiple conditions sequentially and execute code blocks based on which condition is `True`.

**Syntax:**

```python
if condition1:
    # code to execute if condition1 is True
elif condition2:
    # code to execute if condition1 is False and condition2 is True
else:
    # code to execute if none of the above conditions are True
```

### Nested `if` Statement


Nested `if` statements are used when you need to evaluate multiple conditions within another `if` statement.

**Syntax:**

```python
if condition1:
    if condition2:
        # code to execute if both condition1 and condition2 are True
    else:
        # code to execute if condition1 is True and condition2 is False
else:
    # code to execute if condition1 is False

```

### Multiple `if` Statements

In Python, multiple `if` statements are used when you want to check more than one condition independently. Each `if` statement is evaluated separately, and the code blocks associated with each condition will execute if their respective conditions are `True`.

### **Syntax**

```python
if condition1:
    # code to execute if condition1 is True

if condition2:
    # code to execute if condition2 is True

if condition3:
    # code to execute if condition3 is True
```


## 2. Comparison Operators
Comparison operators are used to compare values in conditional statements:


- `==` : Equal to
- `!=` : Not equal to
- `>`  : Greater than
- `<`  : Less than
- `>=` : Greater than or equal to
- `<=` : Less than or equal to


## 3. Logical Operators

Logical operators are used to combine multiple conditions.
### `and` Operator

The `and` operator returns `True` if both conditions being evaluated are `True`. If any of the conditions are `False`, the result will be `False`.

**Syntax:**

```python
if condition1 and condition2:
    # code to execute if both condition1 and condition2 are True
```

### `or` Operator
The `or` operator returns `True` if at least one of the conditions being evaluated is `True`. It returns `False` only if all conditions are `False`.

**Syntax:**

```python
if condition1 or condition2:
    # code to execute if at least one of condition1 or condition2 is True
```

### `not` Operator
The `not` operator inverts the boolean value of a condition. It returns `True` if the condition is `False`, and `False` if the condition is `True`.

**Syntax:**

```python
if not condition:
    # code to execute if condition is False
```



# 4. Project: Treasure Island Adventure Game

### Description

The "Treasure Island" game is an interactive text-based adventure where the player makes choices to navigate through various scenarios in search of a treasure. The game tests decision-making skills and provides different outcomes based on user input.

### How It Works

1. **Welcome Message:**
   The game starts by greeting the player and outlining the mission to find the treasure.

2. **Initial Choice:**
   The player encounters a crossroads and must choose a direction: 'left' or 'right'.

3. **Lake Scenario:**
   If the player chooses 'left', they come to a lake with an island. They must decide to 'wait' for a boat or 'swim' across.

4. **Island Choices:**
   If the player decides to 'wait' and reaches the island, they find a house with three doors: red, yellow, and blue. They must choose one door.

5. **Treasure Outcome:**
   Based on the door choice:
   - **Yellow Door:** The player finds the treasure and wins the game.
   - **Red Door:** The player encounters a room full of fire and loses the game.
   - **Blue Door:** The player faces a room of beasts and loses the game.
   - **Invalid Choice:** The player chooses a non-existent door and loses the game.

6. **Alternate Outcomes:**
   If the player decides to 'swim' or chooses 'right', they encounter obstacles leading to a game over.

### Summary

The game uses nested `if` statements to create a branching narrative based on player choices, resulting in different scenarios and outcomes. This interactive adventure challenges the player to make strategic decisions to successfully find the treasure.
