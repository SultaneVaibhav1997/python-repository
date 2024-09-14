

```markdown
## IPO Cycle

```
Input ----> Process ----> Output
             ^
             |
             |
           Memory
```

## CPU: Central Processing Unit

### Memory Classification

1. **Primary Memory**
   - A memory that is accessible by the CPU.
   - Fast and expensive.
   - Examples: ROM, RAM.

2. **Secondary Memory**
   - A memory that is not accessible by the CPU.
   - Slow and inexpensive.
   - Examples: HDD, SSD, Pen Drive, Memory Card, DVD, CD, Floppy.

### Classification by Content Retention

1. **Volatile Memory**
   - Power on: Content is in memory; Power off: Content is erased.
   - Example: RAM.

2. **Non-Volatile Memory**
   - Content remains in memory regardless of power status.
   - Examples: ROM, HDD, SSD, Pen Drive, Memory Card, DVD, CD, Floppy.

## Software Installation

When you install software like MS-Word, it resides in secondary storage.

```
CPU <-----> RAM <----> Secondary Storage
```

## CPU Language

The CPU understands only binary language (1 & 0).

- **Machine Language**
  - C: `0100 1101`
  - H: `0100 0001`
  - I: `0100 1111`
  - T: `0100 0001`
  - K: `0100 1001`
  - A: `0100 1111`
  - R: `0100 0101`
  - A: `0100 1000`

- **Assembly Language**
  - ADD: `10001010`
  - Assembly Language --> Assembler --> Machine Language

- **High-Level Languages (e.g., C/C++, Python)**
  - Source code in human-readable languages --> Compiler/Interpreter --> Machine Code

## Compiler vs Interpreter

### Compiler

1. Fast.
2. Generates binary code (machine code) that can be saved and reused.
3. Less secure.
4. Requires less memory.
5. Converts entire source code into machine code at once.
6. Compilation stops immediately if errors are present, and no compiled file is generated.

   Example: C, C++, Java

   ```
   C/C++ ---> Compilation ---> .exe/.bin (saved in HDD)
   ```

   Double-click on `.exe/.bin` file to run.

### Interpreter

1. Slow.
2. Generated binary code cannot be saved; the program must be interpreted each time.
3. More secure.
4. Requires more memory.
5. Converts source code into machine code line by line.
6. Stops immediately if errors are present, but the code before the error executes.

   Example: Java, Python, JavaScript

   ```
   python ---> Interpret ---> Output
   ```

## Python Introduction

- **`print()`**: Used to print content on the output window (console).
  - Example:
    ```python
    print("Hello World")
    print(10)
    print(1.5)
    print(True)
    ```

    **Output:**
    ```
    Hello World
    10
    1.5
    True
    ```

  - **Using `end` parameter**:
    ```python
    print("Chitkara", end="~")
    print("University", end=":")
    print("Punjab")
    print(2024)
    ```

    **Output:**
    ```
    Chitkara~University:Punjab
    2024
    ```

  - **Using `sep` parameter**:
    ```python
    print("bengaluru", "Karnataka", "India", sep = ", ")
    print(20, 24, sep = "")
    ```

    **Output:**
    ```
    bengaluru, Karnataka, India
    2024
    ```

  - **Code Example**:
    ```python
    print(1,2,3,4,5)
    print(6,7,8)
    ```

    **Output:**
    ```
    1 2 3 4 5
    6 7 8
    ```

  - **Code Example**:
    ```python
    print("A", 1, True, sep = " : ", end = "$")
    print(False, 9, "X", sep = " - ")
    ```

    **Output:**
    ```
    A : 1 : True$False - 9 - X
    ```

## Comments in Python

- Used for human understanding.
- Machine does not process comments.
- Comments start with `#`.
- Single-line comments.
- Multi-line comments can be done using `#` at the beginning of each line or multi-line strings (not officially comments).

## Variables in Python

- **Memory Structure**:
  - RAM is a primary memory, and programs are loaded into RAM for execution.
  - Address space in RAM is divided into:
    1. **Data Segment**:
       - **Stack**: Contains references (named location).
       - **Heap**: Contains actual objects (unnamed location; accessed using references).
    2. **Code Segment**: Contains instructions.

## Variables in Python

- **Syntax**:
  ```python
  var_name = value
  ```

- **Examples**:
  ```python
  name = "ABHAY"    # variable-name: name, value: ABHAY
  age = 18          # variable-name: age, value: 18
  percentage = 57.25 # variable-name: percentage, value: 57.25
  isMarried = False # variable-name: isMarried, value: False
  print(name, age, percentage, sep = " : ")
  ```

  **Output:**
  ```
  ABHAY : 18 : 57.25
  ```

## Data Types in Python

- A data type defines:
  1. Operations that can be applied.
  2. Range of values.

- **Examples**:
  ```python
  print(type("Chitkara"))   # <class 'str'>
  print(type(10))           # <class 'int'>
  balance = 45.25
  print(type(balance))     # <class 'float'>
  ```

- **Classification**:
  - **Number Category**:
    - `int`: Any non-fractional number.
    - `float`: Any fractional number.
    - `boolean`: True or False.
    - `complex` (Not covered in syllabus).

  - **Sequence Category**:
    - `String`: Anything inside '' or "".

  - **Set Category**:
    - `set` (Discussed later).

  - **None Category**:
    - `None`: No value.

  - **Mapping Category**:
    - `Dictionary` (Discussed later).

  - **Dynamic Typing**:
    ```python
    a = 10
    print(type(a))    # <class 'int'>
    a = 'Hello'
    print(type(a))    # <class 'str'>
    a = 4.5
    print(type(a))    # <class 'float'>
    ```

Sure, here is the converted content in Markdown format:

---

## Arithmetic Operators

- **Addition (`+`)**
- **Subtraction (`-`)**
- **Multiplication (`*`)**
- **Floor Division (`//`)**
  ```python
  print(10 // 5)  # 2
  print(10 // 3)  # 3
  print(10 // 4)  # 2
  ```
- **Modulo (`%`)**
  ```python
  print(10 % 5)  # 0
  # 10 divided by 5 gives a remainder of 0
  print(10 % 3)  # 1
  # 10 divided by 3 gives a remainder of 1
  print(10 % 4)  # 2
  # 10 divided by 4 gives a remainder of 2
  ```
- **Exponentiation (`**`)**
  ```python
  print(5 ** 2)  # 25
  ```

### Examples

```python
print(10 / 3)  # 3.3333333333333335
print(10 * 3 // 4)  # 7
print(2 ** 4 * 8 + 24 + (4 // 3))  # 153
print(3 * 6 / 5)  # 3.6
print(3 / 5 * 6)  # 3.6
print(3 * 6 // 5)  # 3
print(3 // 5 * 6)  # 0
print(2 ** 3 ** 2)  # 512
```

## String Operators

- **Concatenation (`+`)**
  ```python
  print('Chitkara' + "University")  # ChitkaraUniversity
  print('Chitkara' + ' University')  # Chitkara University
  print('Chitkara' + str(2024))  # Chitkara2024
  ```
  
- **Repetition (`*`)**
  ```python
  print('India' * 3)  # IndiaIndiaIndia
  ```

- **With `sep` argument**
  ```python
  print('Chitkara' + 'University', sep=" : ")  # ChitkaraUniversity
  print('Chitkara' + 'University', 2024, sep=" : ")  # Chitkara University : 2024
  ```

## Comparison Operators

- **Greater than (`>`)**
- **Less than (`<`)**
- **Greater than or equal to (`>=`)**
- **Less than or equal to (`<=`)**
- **Not equal to (`!=`)**
- **Equal to (`==`)**

```python
print(10 < 10)  # False
print(10 <= 10)  # True
print(10 > 10)  # False
print(10 >= 10)  # True
print(10 != 10)  # False
print(10 == 10)  # True
```

**Difference Between `a = 10` and `a == 10`:**

- `a = 10` assigns the value 10 to the variable `a`.
- `a == 10` checks if the value of variable `a` is 10.

## Types of Statements

1. **Sequential Statement:** Executed once.
   ```python
   principleAmount = 1000
   timePeriod = 3
   interestRate = 7.5

   simpleInterest = (principleAmount * timePeriod * interestRate) / 100

   print("The simple interest is " + str(simpleInterest))
   ```
   **Output:**
   ```
   The simple interest is 225.0
   ```

2. **Selection Statement:** Executed zero or one time.
   ```python
   quantity = 5
   price = 25
   gender = 'f'
   totalBill = quantity * price
   if gender == 'f':
     totalBill = totalBill * 0.95

   print("The total bill amount is " + str(totalBill))
   ```

   **Output:**

   - For `gender = 'm'`:
     ```
     The total bill amount is 125
     ```
   - For `gender = 'f'`:
     ```
     The total bill amount is 118.75
     ```

3. **Iteration Statement:** Executed zero or more times.

   ```python
   i = 1
   while i <= 5:
     print("Chitkara")
     i += 1
   ```

   **Output:**
   ```
   Chitkara
   Chitkara
   Chitkara
   Chitkara
   Chitkara
   ```

## Selection Statements

- **`if` Statement**

   ```python
   if age < 18:
     print("You are a minor")
   else:
     print("You are an adult")
   ```

- **`if-else` Statement**

   ```python
   age = 15
   if age < 18:
     print("You are a minor")
   else:
     print("You are an adult")
   ```

   **Output:**
   ```
   You are a minor
   ```

- **`if-elif` Statement**

   ```python
   per = 72.25
   if per >= 90.00:
     print("A")
   elif per >= 75.00:
     print("B")
   elif per >= 60.00:
     print("C")
   elif per >= 45.00:
     print("D")
   elif per >= 33.00:
     print("E")
   else:
     print("F")
   ```

   **Output:**
   ```
   C
   ```

## Logical Operators

- **`and` Operator**
  ```python
  age = 17
  nationality = 'indian'
  print(age >= 18 and nationality == 'indian')  # False
  ```

- **`or` Operator**
  ```python
  gender = 'm'
  percentage = 89
  print(gender == 'f' or percentage >= 90.00)  # False
  ```

- **`not` Operator**
  ```python
  no = 45
  if not (no % 2 == 0):
    print("Odd")
  else:
    print("Even")
  ```

## Ternary Operator

```python
age = 15
print('Minor' if age < 18 else 'Adult')
```

## `while` Loop

```python
i = 1
while i <= 10:
  print("Python")
  i += 1
```

**Output:**

```
Python
Python
Python
...
(repeats until i > 10)
```

**Examples:**

```python
i = 10
while i <= 10:
  print("Python")
  i += 1
```

**Output:**
```
Python
```

```python
i = 11
while i <= 10:
  print("Python")
  i -= 1
```

**Output:**
```
(No output)
```

```python
i = 1
while i <= 10:
  print("Python")
i -= 1
```

**Output:**
```
Python
Python
Python
...
(infinite loop)
```

---

Here's your provided content, formatted in Markdown for GitHub:

```md
## Program to Print Sequence: 1 3 5 7 9 11 13 15 17 19

```python
i = 1
while i <= 19:
    print(i, end=' ')
    i += 2
```

### Execution Pattern:
- `i = 1` [1 <= 19: True]
- `i = 3` [3 <= 19: True]
- `i = 5` [5 <= 19: True]
- `i = 7` [7 <= 19: True]
- `i = 9` [9 <= 19: True]
- ...
- `i = 21` [21 <= 19: False]

### Output:
`1 3 5 7 9 11 13 15 17 19`

---

## Another Solution:

```python
i = 1
while i <= 10:
    print((2 * i - 1), end=' ')
    i += 1
```

### Execution Pattern:
- `i = 1` [1 <= 10: True]
- `i = 2` [2 <= 10: True]
- `i = 3` [3 <= 10: True]
- `i = 4` [4 <= 10: True]
- ...
- `i = 11` [11 <= 10: False]

### Output:
`1 3 5 7 9 11 13 15 17 19`

---

## Program to Print Series: 21 15 10 6 3 1

```python
i = 21
d = 6
while i >= 1:
    print(i, end=' ')
    i -= d  # i = i - d
    d -= 1  # d = d - 1
```

### Execution Pattern:
- `i = 21` [21 >= 1: True]
- `i = 15` [15 >= 1: True]
- `i = 10` [10 >= 1: True]
- `i = 6` [6 >= 1: True]
- `i = 3` [3 >= 1: True]
- `i = 1` [1 >= 1: True]
- `i = 0` [0 >= 1: False]
- `d = 6, 5, 4, 3, 2, 1`

### Output:
`21 15 10 6 3 1`

---

## Program to Print Series: 21 15 10 6 3 1 0

```python
i = 21
d = 6
while i >= 0 and d >= 0:
    print(i, end=' ')
    i -= d  # i = i - d
    d -= 1  # d = d - 1
```

### Iterations:
- First iteration: `21, i = 15, d = 5`
- Second iteration: `15, i = 10, d = 4`
- Third iteration: `10, i = 6, d = 3`
- Fourth iteration: `6, i = 3, d = 2`
- Fifth iteration: `3, i = 1, d = 1`
- Sixth iteration: `1, i = 0, d = 0`
- Seventh iteration: `0, i = 0, d = 0`

### Output:
`21 15 10 6 3 1 0`

---

## `break` Statement Example:

The `break` statement is used to exit the loop immediately, without waiting for the loop condition to become false.

```python
i = 1
while i <= 5:
    print(i, end=' ')
    if i == 3:
        break
    i += 1
print("\nBye Bye; I am out of loop")
```

### Output:
```
1 2 3 
Bye Bye; I am out of loop
```

---

## Program to Find the First Three Factors of a Given Number

Sample Input: 12  
Sample Output: `1, 2, 3`

Sample Input: 65  
Sample Output: `1, 5, 13`

```python
no = 65  # 12
i = 1
fc = 0
while i <= no:
    if no % i == 0:
        # i is a factor of no
        print(i, end=' ')
        fc += 1
        if fc == 3:
            break
    i += 1
```

---

## `continue` Statement Example:

The `continue` statement is used to skip particular iterations when a specific condition is met.

```python
i = 1
while i <= 12:
    if i % 5 == 0:
        i += 1
        continue
    print(i, end=' ')
    i += 1
```

### Output:
`1 2 3 4 6 7 8 9 11 12`

---

## `else` with `while` Loop:

In Python, the `else` block can be used with loops. The body of the `else` block will be executed when the loop condition becomes false. However, if the `break` statement is used to exit the loop, the `else` block will be skipped.

### Example 1:

```python
i = 1
while i <= 5:
    print(i, end=' ')
    i += 1
else:
    print("bye bye")
```

### Output:
`1 2 3 4 5 bye bye`

### Example 2:

```python
i = 1
while i <= 5:
    print(i, end=' ')
    if i == 3:
        break
    i += 1
else:
    print("bye bye")
```

### Output:
`1 2 3`

---

## Program to Check if a Number is Prime

A prime number is a number that has exactly two factors: 1 and the number itself.

### Example of Prime Numbers:
`2, 3, 5, 7, 11, 13, 17, 19, 23, 29`

A number `n` is a prime number if it is not divisible by any number from 2 to `n - 1`.

```python
no = 7  # 9
d = 2
while d < no:  # 2 3 4 5 6
    if no % d == 0:
        print(no, "is not a prime number")
        break
    d += 1
else:
    print(no, "is a prime number")
print("Bye bye")
```

### Output 1:
```plaintext
no = 9
d = 2, 3
9 is not a prime number
Bye bye
```

### Output 2:
```plaintext
no = 5
d = 2, 3, 4, 5
5 is a prime number
Bye Bye
```
```


