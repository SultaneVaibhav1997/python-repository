

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

- **Memory Units**:
  - Smallest unit: Bit
  - 8 bits = 1 byte
  - 1024 bytes = 1 KB
  - 1024 KB = 1 MB
  - 1024 MB = 1 GB
  - 1024 GB = 1 TB

  Example: 4 GB RAM

  ```
  4 GB = 2 x 2 x 1024 MB
  4 GB = 2 x 2 x 1024 x 1024 KB
  4 GB = 2 x 2 x 1024 x 1024 x 1024 B
  4 GB = 2^(1 + 1 + 10 + 10 + 10) B
  4 GB = 2^32 B
  ```

- Each memory location has a physical address, e.g., `0X12AB:32FE`.

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

```

