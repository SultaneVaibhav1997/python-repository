```markdown
### IPO Cycle
The Input-Process-Output (IPO) cycle is a framework for understanding how computers handle tasks.
```
**Input → Process → Output**
```
             ^
             |
             |
           Memory
```

**CPU:** Central Processing Unit

**Memory:**
- Classified based on accessibility by the CPU:
  1. **Primary Memory:** Accessible by the CPU, fast, and expensive (e.g., ROM, RAM).
  2. **Secondary Memory:** Not accessible by the CPU, slower, and inexpensive (e.g., HDD, SSD, Pen Drive, Memory Card, DVD, CD, floppy).

- Classified based on content retention w.r.t. power supply:
  1. **Volatile Memory:** Content is lost when power is off (e.g., RAM).
  2. **Non-Volatile Memory:** Content persists regardless of power (e.g., ROM, HDD, SSD, Pen Drive, Memory Card, DVD, CD, floppy).

**Example:**
When you install MS Word, it resides in secondary storage.

**System Architecture:**
```
CPU <-----> RAM <----> Secondary Storage
```

### Machine & Assembly Language
- The CPU understands **binary language** (1 & 0), also called **machine language**:
  ```
  C: 0100 1101
  H: 0100 0001
  I: 0100 1111
  T: 0100 0001
  K: 0100 1001
  A: 0100 1111
  R: 0100 0101
  A: 0100 1000
  ```

- **Assembly Language** is closer to machine language, using symbolic representations like `ADD`. It's converted into machine code using an **assembler**.

### High-Level Languages (HLL)
Languages like C, C++, and Python are written in English-like syntax. They are converted into machine code using either a **compiler** or an **interpreter**.

#### Compiler:
1. Converts the entire source code to machine code at once.
2. Faster but less secure.
3. Compilation stops if an error is encountered.
4. Machine code can be saved and executed multiple times.
   - E.g., C, C++, Java.

#### Interpreter:
1. Converts code line-by-line.
2. Slower but more secure.
3. Code before an error can still be executed.
4. Requires interpretation every time.
   - E.g., Python, JavaScript.

### Python Programming Basics

#### `print()` Function:
- Displays content on the console.
- Adds a new line automatically after each statement.

**Examples:**
```python
print("Hello World")
print(10)
print(1.5)
print(True)
```
Output:
```
Hello World
10
1.5
True
```

**Using `end` Parameter:**
```python
print("Chitkara", end="~")
print("University", end=":")
print("Punjab")
```
Output:
```
Chitkara~University:Punjab
```

**Using `sep` Parameter:**
```python
print("bengaluru", "Karnataka", "India", sep=", ")
```
Output:
```
bengaluru, Karnataka, India
```

### Comments in Python
- Start with `#` and are ignored by the machine.
- For multiline comments, use `#` at the beginning of each line or use string literals.

### Variables in Python
- A variable is a **named memory location** whose value can change.
- In Python, variables are dynamically typed, meaning their type is assigned based on the value.

**Examples:**
```python
name = "ABHAY"
age = 18
percentage = 57.25
isMarried = False
```

### Data Types in Python
- **int**: Whole numbers.
- **float**: Decimal numbers.
- **bool**: `True` or `False`.
- **str**: String (text).
- Other types like List, Tuple, Set, and Dictionary are covered later.

### Arithmetic Operators:
- `+`, `-`, `*`, `/`, `//`, `%`, `**`

**Examples:**
```python
print(10 // 3)  # Floor division, output: 3
print(10 % 3)   # Modulo, output: 1
print(5 ** 2)   # Exponentiation, output: 25
```

### Operator Precedence in Python
1. `()`: Parentheses (highest)
2. `**`: Exponentiation (right to left)
3. `*`, `/`, `//`, `%`: Multiplication, Division, Floor Division, Modulo (left to right)
4. `+`, `-`: Addition, Subtraction (left to right)
5. `=`: Assignment (lowest)

**Example:**
```python
print(2**4 * 8 + 24 + (4 // 3))
# Output: 153
```

### Comparison Operators
- `>`, `<`, `>=`, `<=`, `!=`, `==`
- Output of these operators is always boolean (`True` or `False`).

**Examples:**
```python
print(10 > 5)   # True
print(10 == 10) # True
```

### Logical Operators
- **and**: Both conditions must be true.
- **or**: At least one condition must be true.
- **not**: Negates the condition.

**Example:**
```python
if age >= 18 and citizenship == 'indian':
  print("Welcome! Please cast your vote")
else:
  print("Sorry! you are not able to vote")
```

### If-Else Statements
Python uses indentation to define blocks of code. Conditional statements execute blocks based on the result of a condition.

**Syntax:**
```python
if condition:
  # if block
else:
  # else block
```

### Sequential, Selection, and Iteration Statements
- **Sequential:** Statements executed in order.
- **Selection (if, if-else):** Conditions determine which block to execute.
- **Iteration (while, for):** Repeated execution of code blocks.

