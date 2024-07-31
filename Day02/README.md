# Day 2: Python Notes

## 1. **Data Types**
   - **Introduction**: Data types specify the type of data a variable can hold and determine the operations that can be performed on it. Python is dynamically typed, meaning you don’t need to declare the type of a variable explicitly.

   - **Common Data Types**:
     - **Integer**: Represents whole numbers. Example: `5`, `42`
       ```python
       age = 30
       ```
     - **Float**: Represents decimal numbers. Example: `3.14`, `0.99`
       ```python
       pi = 3.14159
       ```
     - **String**: Represents sequences of characters. Example: `"Hello"`, `'Python'`
       ```python
       greeting = "Hello, World!"
       ```
     - **Boolean**: Represents `True` or `False` values. Example: `True`, `False`
       ```python
       is_student = True
       ```

## 2. **Subscript Operator**
   - **Introduction**: The subscript operator (square brackets `[]`) is used to access elements in sequences like strings, lists, and tuples.

   - **Strings**:
     ```python
     text = "Hello"
     print(text[0])  # Output: H
     ```
     - **Explanation**: Accesses the character at index `0` of the string, which is `'H'`.

   - **Lists**:
     ```python
     numbers = [1, 2, 3, 4]
     print(numbers[2])  # Output: 3
     ```
     - **Explanation**: Accesses the element at index `2` of the list, which is `3`.

   - **Note**: Strings enclosed in double or single quotes are treated as strings. For example, `"123" + "456"` concatenates the strings to produce `"123456"`, not the mathematical sum.

## 3. **Mathematical Operators**
   - **Introduction**: Mathematical operators are used to perform arithmetic operations on numeric values.

   - **Operators**:
     - **Addition (`+`)**:
       ```python
       result = 5 + 3  # Output: 8
       ```
       - **Explanation**: Adds two numbers.

     - **Subtraction (`-`)**:
       ```python
       result = 10 - 4  # Output: 6
       ```
       - **Explanation**: Subtracts one number from another.

     - **Multiplication (`*`)**:
       ```python
       result = 7 * 6  # Output: 42
       ```
       - **Explanation**: Multiplies two numbers.

     - **Division (`/`)**:
       ```python
       result = 8 / 2  # Output: 4.0
       ```
       - **Explanation**: Divides one number by another, resulting in a float.

     - **Floor Division (`//`)**:
       ```python
       result = 9 // 4  # Output: 2
       ```
       - **Explanation**: Divides and returns the integer part of the quotient.

     - **Modulus (`%`)**:
       ```python
       result = 10 % 3  # Output: 1
       ```
       - **Explanation**: Returns the remainder of the division.

     - **Exponentiation (`**`)**:
       ```python
       result = 2 ** 3  # Output: 8
       ```
       - **Explanation**: Raises a number to the power of another.

## 4. **Round Function**
   - **Introduction**: The `round()` function is used to round a floating-point number to a specified number of decimal places.

   - **Syntax**:
     ```python
     rounded_value = round(number, [ndigits])
     ```

   - **Examples**:
     ```python
     print(round(3.14159, 2))  # Output: 3.14
     print(round(2.71828))     # Output: 3
     ```
     - **Explanation**:
       - `round(3.14159, 2)` rounds `3.14159` to two decimal places, resulting in `3.14`.
       - `round(2.71828)` rounds `2.71828` to the nearest integer, resulting in `3`.

## 5. **Assignment Operators**
   - **Introduction**: Assignment operators are used to assign values to variables and can be combined with arithmetic operations for shorthand assignments.

   - **Basic Assignment**:
     ```python
     x = 10
     ```
     - **Explanation**: Assigns the value `10` to the variable `x`.

   - **Shorthand Operators**:
     - **Addition Assignment (`+=`)**:
       ```python
       x += 5  # Equivalent to x = x + 5
       ```
       - **Explanation**: Increases the value of `x` by `5`.

     - **Subtraction Assignment (`-=`)**:
       ```python
       x -= 3  # Equivalent to x = x - 3
       ```
       - **Explanation**: Decreases the value of `x` by `3`.

     - **Multiplication Assignment (`*=`)**:
       ```python
       x *= 2  # Equivalent to x = x * 2
       ```
       - **Explanation**: Multiplies the value of `x` by `2`.

     - **Division Assignment (`/=`)**:
       ```python
       x /= 4  # Equivalent to x = x / 4
       ```
       - **Explanation**: Divides the value of `x` by `4`.

## 6. **F-Strings**
   - **Introduction**: F-strings (formatted string literals) allow you to embed expressions inside string literals using curly braces `{}`.

   - **Syntax**:
     ```python
     f"string {expression}"
     ```

   - **Examples**:
     ```python
     name = "Alice"
     age = 30
     print(f"Hello, {name}. You are {age} years old.")  # Output: Hello, Alice. You are 30 years old.
     ```
     - **Explanation**: The `f` before the string indicates that it is an f-string. Expressions inside `{}` are evaluated and formatted into the string.

## 7. **Tip Calculator Project**

## **Project Overview**

Welcome to the Tip Calculator! This Python program helps users calculate the amount each person should pay when splitting a bill with a tip. Users input the total bill amount, select a tip percentage, and specify the number of people sharing the bill. The program then computes and displays the amount each person needs to contribute.

## **Features**
- Input for the total bill amount.
- Option to choose a tip percentage (10%, 12%, or 15%).
- Input for the number of people sharing the bill.
- Calculation of the total tip amount.
- Computation of the total bill including tip.
- Division of the total bill by the number of people.
- Display of the amount each person should pay.

## **Code Explanation**

```python
print("Welcome to the Tip Calculator!")
print("What was the total bill? Rs.")
bill = float(input())
print("How much tip would you like to give? 10%, 12%, or 15%?")
tip = int(input())
while tip not in [10, 12, 15]:
    print("Please enter a valid tip percentage: 10%, 12%, or 15%")
    tip = int(input())
print("How many people to split the bill?")
people = int(input())
while people <= 0:
    print("The number of people must be greater than zero. Please enter a valid number.")
    people = int(input())

# Convert tip percentage to decimal
tip_as_percent = tip / 100

# Calculate total tip amount
total_tip_amount = bill * tip_as_percent

# Calculate total bill including tip
total_bill = bill + total_tip_amount

# Calculate amount each person should pay
bill_per_person = total_bill / people

# Display the result
print(f"Each person should pay: Rs. {bill_per_person:.2f}")

