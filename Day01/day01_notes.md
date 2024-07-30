# Day 1: Python Notes

## 1. **Introduction to Python**
   - **What is Python?**
     - Python is a high-level, interpreted programming language designed for readability and ease of use. Its syntax is straightforward and resembles natural language, making it accessible for beginners and powerful for experts.
   - **Why Learn Python?**
     - Python is versatile and widely used in various domains such as web development, data science, artificial intelligence, automation, and more. Its extensive libraries and frameworks support rapid development and integration.

## 2. **Basic Syntax**
   - **Print Function**
     ```python
     print("Hello, World!")
     ```
     - **Purpose**: The `print()` function is used to display output to the console. The text inside the parentheses is printed exactly as it appears.
     - **How It Works**: The `print()` function takes one or more arguments and outputs them as a string to the standard output (usually the console).

## 3. **Print Modifiers**
   - **Using Quotes Inside Strings**
     - **Single Quotes Inside Double Quotes**:
       ```python
       print("Hi, my name is 'Snigdha.' I am 20 years old.")
       ```
       - **Explanation**: Double quotes are used to encapsulate the string, allowing single quotes to be included without escaping.
     - **Double Quotes Inside Single Quotes**:
       ```python
       print('Hi, my name is "Snigdha." I am 20 years old.')
       ```
       - **Explanation**: Single quotes are used to encapsulate the string, allowing double quotes to be included without escaping.
   - **Escape Sequences in Strings**
     - **Purpose**: Escape sequences are used to include special characters in strings that would otherwise be problematic or misinterpreted.
     - **Examples**:
       ```python
       print("He said, \"Python is amazing!\"")   # Escaping double quotes
       print('It\'s a great day to learn Python.') # Escaping single quote
       print("Path to the file is C:\\Users\\Name\\Documents") # Escaping backslashes
       ```
       - **Explanation**: 
         - `\"` - Escapes double quotes within double-quoted strings.
         - `\'` - Escapes single quotes within single-quoted strings.
         - `\\` - Escapes backslashes to include them in the string.

## 4. **New Line Character (`\n`)**
   - **Inserting New Lines**
     ```python
     print("Hello,\nWorld!")
     ```
     - **Purpose**: The `\n` character represents a new line in a string. It moves the cursor to the next line when printing.
     - **How It Works**: The `\n` escape sequence is interpreted by Python to break the string into multiple lines.

## 5. **String Concatenation Using `+`**
   - **Combining Strings**
     ```python
     first_name = "John"
     last_name = "Doe"
     full_name = first_name + " " + last_name
     print(full_name)
     ```
     - **Purpose**: String concatenation combines multiple strings into one.
     - **How It Works**: The `+` operator is used to join strings. Spaces or other separators must be explicitly added if needed.

## 6. **Spacing in Strings**
   - **Examples of Spacing**
     ```python
     print("Hi" + "World")        # Output: HiWorld
     print("Hi " + "World")        # Output: HiWorld
     print("Hi" + " World")        # Output: Hi World
     print("Hi" + " " + "World")   # Output: Hi World
     ```
     - **Explanation**:
       - `"Hi" + "World"`: Concatenates "Hi" with "World" without additional space.
       - `"Hi " + "World"`: Concatenates "Hi" with " World", which includes a space.    
       - `"Hi" + " World"`: Concatenates "Hi" with " World", which includes a space.
       - `"Hi" + " " + "World"`: Explicitly adds a space between "Hi" and "World".

## 7. **Input Function**
   - **Getting User Input**
     ```python
     name = input("Enter your name: ")
     print("Hello, " + name + "!")
     ```
     - **Purpose**: The `input()` function is used to collect data from the user.
     - **How It Works**: `input()` displays a prompt message and waits for the user to enter a response. The entered text is returned as a string.

## 8. **Comments**
   - **Single-Line Comments**
     ```python
     # This is a single-line comment
     print("Hello, World!")  # This is an inline comment
     ```
     - **Purpose**: Single-line comments are used to add notes or explanations within the code.
     - **How It Works**: Comments begin with `#` and extend to the end of the line. They are ignored during execution.

   - **Multi-Line Comments**
     ```python
     """
     This is a multi-line comment.
     It can span multiple lines.
     """
     print("Hello, World!")
     ```
     - **Purpose**: Multi-line comments are used for longer explanations or to temporarily disable parts of the code.
     - **How It Works**: Multi-line comments are enclosed in triple quotes (`"""` or `'''`). They span multiple lines and are ignored during execution.

## 9. **The `len()` Function**
   - **Determining Length**
     ```python
     length = len("Hello, World!")
     print(length)  # Output: 13
     ```
     - **Purpose**: The `len()` function returns the number of characters in a string or the number of items in other iterable objects.
     - **How It Works**: `len()` calculates the length of the object passed to it and returns an integer value.

## 10. **Variables**
   - **Creating Variables**
     ```python
     age = 25
     name = "Alice"
     ```
     - **Purpose**: Variables store data values that can be used and manipulated throughout the program.
     - **How It Works**: Variables are created by assigning a value to a name using the `=` operator. The data type of the variable is determined automatically.

   - **Naming Rules**
     - **Start with a Letter or Underscore**: Variable names must begin with a letter (a-z, A-Z) or an underscore (`_`).
     - **Followed by Letters, Digits, or Underscores**: After the initial character, names can include letters, digits, and underscores.
     - **Case-Sensitive**: Variable names are case-sensitive. For example, `variable`, `Variable`, and `VARIABLE` are different.
     - **No Reserved Keywords**: Variable names cannot be Python reserved keywords (e.g., `if`, `while`, `class`, `import`).
     - **Use Descriptive Names**: Choose meaningful names that indicate the purpose of the variable, improving code readability.
     - **Avoid Special Characters and Spaces**: Variable names cannot include spaces or special characters (other than underscores).

---
