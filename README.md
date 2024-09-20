

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

```md
## `range()` Function in Python

The format of the `range()` function:

```python
range(start=0, stop, step=1)
```

It is used to generate a sequence from `start` to `stop - 1` such that consecutive elements of the sequence are separated by the `step` value.

### Examples:

```python
print(list(range(5)))  # start = 0, stop = 5, step = 1 [0, 1, 2, 3, 4]
print(list(range(3, 5)))  # start = 3, stop = 5, step = 1 [3, 4]
print(list(range(2, 11, 2)))  # start = 2, stop = 11, step = 2 [2, 4, 6, 8, 10]
print(list(range(11, 1, -2)))  # start = 11, stop = 1, step = -2 [11, 9, 7, 5, 3]
```

---

## `for` Loop

The general format of the `for` loop:

```python
for var-name in sequence:
    body of loop
```

### Example:

```python
for i in range(5):
    print(i, end=' ')
print("\n")

for i in range(2, 10, 2):
    print(i, end=' ')
print("\n")

for i in range(50, 1, -5):
    print(i, end=' ')
print("\n")

for ch in 'Masai':
    print(ch, end=' ')
print("\n")
```

### Output:

```plaintext
0 1 2 3 4 

2 4 6 8 

50 45 40 35 30 25 20 15 10 5 

M a s a i 
```

### Explanation:

Everything inside double quotes is treated as a string, but `\n` is not. This is because `\n` is an **escape sequence**.

---

## Escape Sequences in Python

- `\n`: new line
- `\t`: tab
- `\b`: backspace
- `\a`: alarm

### Example:

```python
print("Masai", end='')
print("\n")  # \n is used to print in the next line
print("\\n")  # \\n is printed as \n
print("School", end='')
```

### Output:

```plaintext
Masai

\n
School
```

---

## Write a Program to Find Factorial of a Given Number

Factorial is the product of all integers from 1 to the given number.

- `factorial(5) = 5 x 4 x 3 x 2 x 1 = 120`
- `factorial(3) = 3 x 2 x 1 = 6`
- `factorial(7) = 7 x 6 x 5 x 4 x 3 x 2 x 1 = 5040`

### Using `for` Loop:

```python
n = 5  # Change to 7, 3
fact = 1
for i in range(2, n + 1):
    fact = fact * i
print("The factorial of", n, "is", fact)
```

### Execution Pattern:

- `n = 5`
- `fact = 1, 1, 2, 6, 24, 120`
- `i = 1, 2, 3, 4, 5, 6 (False)`

### Output:

```plaintext
The factorial of 5 is 120
```

### Another Logic Using `for` Loop:

```python
n = 5  # Change to 7, 3
fact = 1
for i in range(n, 1, -1):
    fact = fact * i
print("The factorial of", n, "is", fact)
```

### Using `while` Loop:

```python
n = 5  # Change to 7, 3
fact = 1
i = 1
while i <= n:
    fact = fact * i
    i += 1
print("The factorial of", n, "is", fact)
```

---

## Write a Program to Find Sum of Natural Numbers for a Given Range

### Example 1:

For `start = 1` and `end = 5`:  
Sum = `1 + 2 + 3 + 4 + 5 = 15`

### Example 2:

For `start = 10` and `end = 13`:  
Sum = `10 + 11 + 12 + 13 = 46`

### Using `for` Loop:

```python
start = 1
end = 5
sum = 0
for i in range(start, end + 1):
    sum = sum + i
print("The sum of natural numbers from", start, "to", end, "is", sum)
```

### Using `while` Loop:

```python
start = 1
end = 5
sum = 0
i = start
while i <= end:
    sum = sum + i
    i += 1
print("The sum of natural numbers from", start, "to", end, "is", sum)
```

---

## Write a Program to Find Sum of Digits of a Given Number

### Example 1:

For `n = 1574`:  
Sum = `1 + 5 + 7 + 4 = 17`

### Example 2:

For `n = 108`:  
Sum = `1 + 0 + 8 = 9`

### Explanation:

For `n = 1574`:

1. `1574 % 10 = 4`, `1574 // 10 = 157`
2. `157 % 10 = 7`, `157 // 10 = 15`
3. `15 % 10 = 5`, `15 // 10 = 1`
4. `1 % 10 = 1`, `1 // 10 = 0`

### Code:

```python
n = 1574
sum = 0
while n != 0:
    sum = sum + n % 10  # sum += (n % 10)
    n = n // 10  # n //= 10
print("The sum of digits is", sum)
```

### Execution Pattern:

- `n = 1574 [True]`, `157 [True]`, `15 [True]`, `1 [True]`, `0 [False]`
- `sum = 0, 4, 11, 16, 17`

### Output:

```plaintext
The sum of digits is 17
```
```markdown
## Nested Loop: Loop inside Another Loop

A loop inside another loop is called a nested loop. For each iteration of the outer loop, the inner loop is executed from the beginning.

```python
i = 1
while i <= 3:  # Outer loop
    j = 1
    while j <= 3:  # Inner/Nested loop
        print(i + j, end=' ')
        j += 1
    print()  # Inserts a new line
    i += 1
print("Bye Bye")
```

### Execution

- `i = 1` [1 <= 3: True]
  - `j = 1` [1 <= 3: True]
  - `j = 2` [2 <= 3: True]
  - `j = 3` [3 <= 3: True]
  - `j = 4` [4 <= 3: False]
- `i = 2` [2 <= 3: True]
  - `j = 1` [1 <= 3: True]
  - `j = 2` [2 <= 3: True]
  - `j = 3` [3 <= 3: True]
  - `j = 4` [4 <= 3: False]
- `i = 3` [3 <= 3: True]
  - `j = 1` [1 <= 3: True]
  - `j = 2` [2 <= 3: True]
  - `j = 3` [3 <= 3: True]
  - `j = 4` [4 <= 3: False]
- `i = 4` [4 <= 3: False]

**Output:**
```
2 3 4 
3 4 5 
4 5 6 
Bye Bye
```

### Another Example

```python
i = 3
while i >= 1:
    j = 1
    while j <= i:
        print(j, end=' ')
        j += 1
    print()
    i -= 1
```

**Output:**
```
1 2 3 
1 2 
1 
```

---

## Pattern Drawing Example 1

Print the following pattern:
```
1
12
123
1234
12345
```

### Explanation

- Outer loop handles the rows.
- Inner loop handles the columns, printing numbers from 1 to the current row number.

```python
r = 1  # Variable for rows
while r <= 5:  # Outer loop for rows
    c = 1  # Variable for columns
    while c <= r:  # Inner loop for columns
        print(c, end='')
        c += 1
    print()  # New line after each row
    r += 1
```

### Execution

- `r = 1` [1 <= 5: True]
  - `c = 1` [1 <= 1: True], `c = 2` [2 <= 1: False]
- `r = 2` [2 <= 5: True]
  - `c = 1` [1 <= 2: True], `c = 2` [2 <= 2: True], `c = 3` [3 <= 2: False]
- ...

**Output:**
```
1
12
123
1234
12345
```

### Solution Using `for` Loop

```python
for r in range(1, 6):  # r = 1, 2, 3, 4, 5
    for c in range(1, r + 1):
        print(c, end='')
    print()
```

---

## Pattern Drawing Example 2

Print the following pattern:
```
12345
1234
123
12
1
```

### Explanation

- Outer loop handles the rows.
- Inner loop prints numbers from 1 to `(6 - row)`.

```python
r = 1  # Variable for rows
while r <= 5:  # Outer loop for rows
    c = 1
    while c <= (6 - r):  # Inner loop for columns
        print(c, end='')
        c += 1
    print()
    r += 1
```

### Solution Using `for` Loop

```python
for r in range(1, 6):
    for c in range(1, 7 - r):
        print(c, end='')
    print()
```

---

## Example: Alternating 0s and 1s

Print the following pattern:
```
0
01
010
0101
01010
```

### Explanation

- Outer loop controls the rows.
- Inner loop prints `0` or `1` based on whether the column number is odd or even.

```python
for r in range(1, 6):  # Rows from 1 to 5
    for c in range(1, r + 1):  # Columns from 1 to row number
        print(0, end='') if c % 2 == 1 else print(1, end='')
    print()
```

### Explanation of `print()` statement

The statement:
```python
print(0, end='') if c % 2 == 1 else print(1, end='')
```
is equivalent to:
```python
if c % 2 == 1:
    print(0, end='')
else:
    print(1, end='')
```

