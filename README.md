IPO cycle

Input ----> Process ----> Output

^

|

|

Memory

CPU: Central Processing Unit

Memory:

First classification is on the behalf on accessibility by CPU

1\. Primary Memory

A memory that is accessible by the CPU

Fast and expensive

e.g. ROM, RAM

2\. Secondary Memory

A memory that is not accessible by the CPU

slow and in-expensive

e.g. HDD, SSD, Pen Drive, Memory Card, DVD, CD, floppy

Second classification is on the behalf of content retention w.r.t. power supply

1\. Volatile Memory

Power on, content is in memory; Power off, content is erased

e.g. RAM

2\. Non-Volatile Memory

No matter Power on/off, content is in the memory

e.g. ROM, HDD, SSD, Pen Drive, Memory Card, DVD, CD, floppy

Install a software MS-Word in my machine; It will be in secondary storage

CPU <-----> RAM <----> Secondary Storage

CPU understand only one language that is binary langauge (1 & 0)

Machine language

C: 0100 1101

H: 0100 0001

I: 0100 1111

T: 0100 0001

K: 0100 1001

A: 0100 1111

R: 0100 0101

A: 0100 1000

Assembly language

ADD ---- 10001010

Assembly language ----> Assembler ---> Machine Language

C/C++/Python

Source code in english like langauges ---> Compiler/Interpreter ---> Machine code

Compiler

1\. Fast

2\. Generated binary code (machine code) can be saved in the HDD so once compilation is done then the program can be run any number of times without compiling again

3\. Less secure

4\. require less memory

5\. compiler is used to convert entire source code in the machine code at once

6\. if error in code then compilation will stop immediately and no compiled file will be generated

e.g. C, C++, java

C/C++ ---> compilation ---> .exe/.bin (saved in HDD)

double click on .exe/.bin file

double click on .exe/.bin file

double click on .exe/.bin file

double click on .exe/.bin file

double click on .exe/.bin file

...

Interpreter

1\. Slow

2\. Generated binary code (machine code) can not be saved in the HDD to run program we have to interpret it again and again

3\. More secure

4\. Require more memory

5\. Interpreter is used to convert source code in the machine code line by line

6\. if error in code then interpretation stops immediately but the code before error will be executed.

e.g. java, python, javascript

python ---> interpret ---> output

python ---> interpret ---> output

python ---> interpret ---> output

python ---> interpret ---> output

python ---> interpret ---> output

...

Day-02

python intro: from notes

replit set up: from notes

print(): used to print content on output window (console)

Whatever we write in the print function is printed on the screen as it is.

After every print() statement automatically a new line is added i.e. next output will be available in the new line

print("Hello World")

print(10)

print(1.5)

print(True)

Output

Hello World

10

1.5

True

We can use end parameter to insert any symbol after printing

print("Chitkara", end="~")

print("University", end=":")

print("Punjab")

print(2024)

Output

Chitkara~University:Punjab

2024

We can add multiple arguments in the print function; all these arguments will be printed as it is on the screen but they will be space separated by default.

print("Chitkara", "University", 2024);

Output

Chitkara University 2024

To use any other symbol then default we have to specify sep argument.

print("bengaluru", "Karnataka", "India", sep = ", ");

print(20, 24, sep = "")

Output

bengaluru, Karnataka, India

2024

What is output of following code

print(1,2,3,4,5)

print(6,7,8)

Output

1 2 3 4 5

6 7 8

The above code is same as

print(1,2,3,4,5, sep = " ", end = "\\n")

print(6,7,8, sep = " ", end = "\\n")

Output

1 2 3 4 5

6 7 8

what is output of following code

print("A", 1, True, sep = " : ", end = "$")

print(False, 9, "X", sep = " - ")

Output

A : 1 : True$False - 9 - X

Comments in python

\- Inserted for human understading

\- Machine never process comments

\- comments in python starts with #

\- A comment is of single line only be default if comment if of multiple lines then with at the beginning of every line we have to put # symbol

\- Multiline comments in other ways: Study String

Variables naming in python

CPU <-----> RAM <----> Secondary Storage

(Process) (Program)

\- RAM is a primary memory so whenever a program is to be executed first it has ti be loaded in the RAM

\- When a program is loaded in the RAM then it occupy some space in the RAM which is called address space i.e. address space is memory space that a program takes in RAM for execution.

\- The address spaces has two major parts

1\. Data Segment: Contains variables

Data segment has two important subparts

a. stack: used to contains reference to object, it is named location

b. heap: used to contains actual object that has value, it is unnamed location; accessed using reference.

2\. Code segment: Contains instructions

Smallest unit of memory is bit

8 bits: 1 byte

1024 bytes: 1 KB

1024 KB: 1 MB

1024 MB: 1 GB

1024 GB: 1 TB

Say a person 'Alex' has a laptop that has 4 GB RAM

4 GB = 2 x 2 x 1024 MB

4 GB = 2 x 2 x 1024 x 1024 KB

4 GB = 2 x 2 x 1024 x 1024 x 1024 B

4 GB = 2 x 2 x 2^10 x 2^10 x 2^10 B

4 GB = 2 x 2 x 2^10 x 2^10 x 2^10 B (a^b x a^c => a^(b+c))

4 GB = 2^(1 + 1 + 10 + 10 + 10) B

4 GB = 2^32 B

Each memory location has some physical address that physical address looks like 0X12AB:32FE

A variable is named memory location whose value can be changed.

\[python specific\] A variable is a reference to object such that variable is used to refer to object that has value actually.

syntax

var-name = value;

e.g.

name = "ABHAY"#variable-name: name value: ABHAY

age = 18#variable-name: age value: 18

percentage = 57.25#variable-name: percentage value: 57.25

isMarried = False#variable-name: isMarried value: False

print(name, age, percentage, sep = " : ")

#Output ABHAY : 18 : 57.25

stack heap

| 7485 |---->|\_ABHAY\_| 7485

name

| 9635 |---->|\_18\_| 9635

age

| 7485 |---->|\_57.25\_| 7485

percentage

Data types in python

A data type defines following properties of variables

1\. operations that can be applied

2\. Range of values of Set values

Note: type() function is used to get data type of a variable of value

print(type("Chitkara"))#

print(type(10))#

balance = 45.25

print(type(balance))#

classification of data types in python

Number Category

int: Any non-fractional number

float: Any fractional number

boolean: True or False

complex (Not in syllabus)

Sequence Category

String: Anything inside '' or "" is String

List: discuss Later

Tuple: discuss Later

Set Category

set: discuss Later

None Category

None: No value

Mapping Category

Dictionary: discuss Later

+-+-+-+-+-+-+-+-++-+-+-+-++-+-+-+-++-+-+-+-+-

\+ Discuss Later: Immutable and Mutable type +

+-+-+-+-+-+-+-+-++-+-+-+-++-+-+-+-++-+-+-+-+-

variable in python are dynamically typed means according to value, data type of variable is changed i.e. variables in python are not having any fixed data type

a = 10

print(type(a));//

a = 'Hello'

print(type(a));//

a = 4.5

print(type(a));//

Arithmetic operators

+

\-

\*

/

// floor division operator

%

\*\* exponential

print(10 / 3);//3.3333333333333

print(10 // 5);//2

print(10 // 3);//3

print(10 // 4);//2

print(10 % 5);//0

5)10(2

10

\--

0

\--

print(10 % 3);//1

3)10(3

9

\--

1

\--

print(10 % 4);//2

4)10(2

8

\--

2

\--

print(5\*\*2);//25

What is output of following

print(10\*3//4)

According to BODMAS

print(10\*0)

0

According to python, No BODMAS; Operator priority and associativity rule

1\. () Highest priority (left to right)

2\. \*\*: (right to left)

3\. \*, /, //, % (left to right)

4\. +, – (left to right)

5\. = Lowest priority (right to left)

https://www.geeksforgeeks.org/precedence-and-associativity-of-operators-in-python/

print(2\*\*4 \* 8 + 24 + (4//3));

Step-01: 2\*\*4 \* 8 + 24 + 1

Step-02: 16 \* 8 + 24 + 1

Step-03: 128 + 24 + 1

Step-04: 152 + 1

Step-05: 153

Output: 153

print(3 \* 6 / 5)

Step-01: 18 / 5

Step-02: 3.6

Output: 3.6

print(3 / 5 \* 6)

Step-01: 0.6 \* 6

Step-02: 3.6

Output: 3.6

print(3 \* 6 // 5)

Step-01: 18 // 5

Step-02: 3

Output: 3

print(3 // 5 \* 6 )

Step-01: 0 \* 6

Step-02: 0

Output: 0

What is output of following code

print(2\*\*3\*\*2);

Step-01: 2\*\*9#because \*\* is operated from right to left

Step-02: 512

\+ for concatenation & \* for repetition

If + is applied on String, list or tuple then it is used to perform concatenation

For concatenation operater; bpth left and right hand side parameter must be of same type.

print('Chitkara' + "University");#ChitkaraUniversity

print('Chitkara' + ' University');#Chitkara University

print('Chitkara' + 2024);#ERROR because str + int is not allowed

print('Chitkara' + str(2024));#Chitkara2024

If \* is applied on String, list or tuple then it is used to perform repetition

For repetition operater; one operater must be of int type; another can be sequence.

print('India' \* 3);#IndiaIndiaIndia

print('India' \* '3');#Error

print('India' \* 1.5);#Error

print('Chitkara' + 'University', sep = " : ")#ChitkaraUniversity

print('Chitkara' + 'University',2024, sep = " : ")#Chitkara University : 2024

Comparison operators: Output of Comparison operator is always a boolean value

\> greater than

< less than

\>= greater than or equal to

<= less than or equal to

!= inequality

\== equaity/comparison

print(10 < 10);#false

print(10 <= 10);#true

print(10 > 10);#false

print(10 >= 10);#true

print(10 != 10);#false

print(10 == 10);#true

What is difference between a = 10 and a == 10;

a = 10 means assigning value 10 to variable a

a == 10 means checking if the value of variable a is 10.

Types of statements

1\. Sequential statement: Any statement that executed for one time; neither it can be skipped not it can be executed for more than one time.

2\. Selection statement: Any statement that may be executed for zero or one time; They cannot be executed for more than one time.

e.g. if, if-else, nested-if, if-elif

3\. Iteration statement: Any statement that may be executed for zero or more time

e.g. while, for

All statement of the following code are sequential statement-

#WAP to print simple interest

principleAmount = 1000

timePeriod = 3

interestRate = 7.5

simpleInterest = (principleAmount \* timePeriod \* interestRate) / 100

print("The simple interest is " + str(simpleInterest))

Output:

The simple interest is 225.0

Let us discuss about the selection statements

1\. if statement

Syntax

if condition:

statement that are part of if body

statement that are outside if body

#WAP to compute bill amout such that all women customers are going to have 5% discount as this is women's week

#WAP to compute bill amout such that all women customers are going to have 5% discount as this is women's week

#create variable to hold quantity o product

quantity = 5

#create variable to hold price of a product

price = 25

#create variable to hold gender

gender = 'f' #'m'

#create variable to hold total bill amount

totalBill = quantity \* price

if gender == 'f':

totalBill = totalBill \* 0.95

print("The total bill amount is " + str(totalBill))

Output (When gender is 'm')

The total bill amount is 125

Output (When gender is 'f')

The total bill amount is 118.75

for the above code-

if gender == 'f':

totalBill = totalBill \* 0.95

is of selection statement; rest all part is of sequential statement

if-else

Synatx:

if condition:

statements of if body

else:

statements of else body

Execution pattern-01

when condition is true, statements of if body will be executed but statements of else body will be bypassed

Execution pattern-02

when condition is false, statements of if body will be bypassed but statements of else body will be executed

#WAP to check if a person is adult or minor such that if person's age is less than 18 then minor; adult otherwise

age = 15 #18, 23

if age < 18:

print("You are a minor")

else:

print("You are an adult")

Output (for age = 18)

You are an adult

Output (for age = 23)

You are an adult

Output (for age = 15)

You are a minor

if-elif

WAP to print grade of Student based on percentage

per >= 90.00 then A

per >= 75.00 then B

per >= 60.00 then C

per >= 45.00 then D

per >= 33.00 then E

per < 33.00 then F

#Using nested if: Not suitable for deep level of nesting because lot of indentation

per = 95.00#84.25, 72.25, 58.25, 42.25, 28.25

if per >= 90.00:

print("A")

else:

#you are here means per < 90.00

if per >= 75.00:

#you are here means per is between 75.00 and 89.99

print("B")

else:

#you are here means per < 75.00

if per >= 60.00:

#you are here means per is between 60.00 and 74.99

print("C")

else:

#you are here means per < 60.00

if per >= 45.00:

#you are here means per is between 45.00 and 59.99

print("D")

else:

#you are here means per < 45.00

if per >= 33.00:

print("E")

else:

print("F")

Note: Python is indentation oriented langauge means to define body of blocks (if, else, while, for, function etc) we have to use indentation, if the block if available at indentation level-N then its body will be available at indentation level N + 1

#Using if-elif: Better

if condition-01:

statement-x

else:

if condition-02:

statement-y

is same as

if condition-01:

statement-x

elif condition-02:

statement-y

#solution to same problem using if-elif statement

per = 72.25#95.00, 84.25, 58.25, 42.25, 28.25

if per >= 90.00:

print("A")

elif per >= 75.00:

#you are here means per is between 75.00 and 89.99

print("B")

elif per >= 60.00:

#you are here means per is between 60.00 and 74.99

print("C")

elif per >= 45.00:

#you are here means per is between 45.00 and 59.99

print("D")

elif per >= 33.00:

print("E")

else:

print("F")

Logical operator: Used to Join two or more conditions

print(10 > 5 > 2);#True

print(10 < 5 < 2);#False

We have three logical operaters

C1 C2 C1 and C2 C1 or C2 not C2

true true true true False

true false false true True

false true false true

false false false false

#WAP to check if a person is eligible for voting or not such that

#(i) person must be of 18 years old or more; and

#(ii) person must be of indian citizenship

#create a variable for age

age = 17 #19, 18

#create a variable for citizenship

citizenship = 'indian' #non-indian

#code to check if person is eligible for voting or not

if age >= 18 and citizenship == 'indian':

print("Welcome! Please cast your vote")

else:

print("Sorry! you are not able to vote")

print("Thanks for using our services")

condition-01: age >= 18

condition-02: citizenship == 'indian'

#WAP to check a student is eligible for scholarship such that

(i) All female students are eligible; or

(ii) All students whose percentage is 90% or more are also eligible

condition-01: gender == 'f'

condition-02: percentage >= 90.00

#WAP to check a student is eligible for scholarship such that

#(i) All female students are eligible; or

#(ii) All students whose percentage is 90% or more are also eligible

#create variables for gender and percentage

gender = 'm' #'f'

percentage = 89 #90

#logic to check eligibility

if gender == 'f' or percentage >= 90.00:

print("Eligible for scholarship")

else:

print("Not eligible for scholarship")

print("Good Luck for future")

#WAP to check if a person is eligible for marriage or not

(i) for male person age must be of 21 or more

(ii) for female person age must be of 18 or more

condition-01: gender == 'm' and age >= 21

condition-02: gender == 'f' and age >= 18

#create variable for gender and age

gender = 'm' #'f'

age = 21 #19

#check if the person is eligible for marriage

if (gender == 'm' and age >= 21) or (gender == 'f' and age >= 18):

print("Eligible for marriage")

else:

print("Not Eligible for marriage")

Note:

(i) From the table of and operator it can be concluded that if LHS condition is false then no matter what is the result of RHS condition ultimate result will be false so if LHS condition is false then RHS condition is not checked.

age = 18 #17

nationality = 'indian' #'non-indian'

print(age >= 18 and nationality == 'indian')

print(True and True)

print(True)

Output: True

age = 18 #17

nationality = 'non-indian' #'indian'

print(age >= 18 and nationality == 'indian')

print(True and False)

print(False)

Output: False

age = 17 #18

nationality = 'indian' #'non-indian'

print(age >= 18 and nationality == 'indian')

print(False and Not Checked)

print(False)

Output: False

age = 17 #18

nationality = 'non-indian' #'indian'

print(age >= 18 and nationality == 'indian')

print(False and Not Checked)

print(False)

Output: False

(ii) From the table of or operator it can be concluded that if LHS condition is true then no matter what is the result of RHS condition ultimate result will be true so if LHS condition is true then RHS condition is not checked.

gender = 'm' #'f'

percentage = 89 #90

print(gender == 'f' or percentage >= 90.00)

print(False or False)

print(False)

Output: False

gender = 'm' #'f'

percentage = 90 #89

print(gender == 'f' or percentage >= 90.00)

print(False or True)

print(True)

Output: True

gender = 'f' #'m'

percentage = 89 #90

print(gender == 'f' or percentage >= 90.00)

print(True or Not Checked)

print(True)

Output: True

gender = 'f' #'m'

percentage = 90 #89

print(gender == 'f' or percentage >= 90.00)

print(True or Not Checked)

print(True)

Output: True

A simple example of not operater

no = 45#78

if not (no % 2 == 0):

print("Odd")

else:

print("Even")

Output-01

no = 45

not (no % 2 == 0)

not (45 % 2 == 0)

not (1 == 0)

not (False)

True

Output: Odd

Output-02

no = 78

not (78 % 2 == 0)

not (78 % 2 == 0)

not (0 == 0)

not (True)

False

Output: Even

Ternary operator: useful when body of if and else both has one statement only. This provide a smaller way to write code then conventional if - else

Syntax:

body of if statement if condition else body of else statement

An Example

#WAP to check if a person is adult or minor such that age < 18 then minor

conventional way

if age < 18:

print('Minor')

else:

print('Adult')

::while loop::

Tip: No increment and decrement operator in python as it is available in other languages

Some real world analogy, chapati, cricket over

while loop

while condition:

body of while loop

execution pattern of while loop

condition (T) ---> body of while loop ---> condition (T) ---> body of while loop ---> condition (T) ---> body of while loop ---> condition (F)

An Example of while loop

#WAP to print Chitkara for 5 times

Approach-01

print("Chitkara")

print("Chitkara")

print("Chitkara")

print("Chitkara")

print("Chitkara")

This approach is very poor as it is not scalable and it has duplicacy also.

Approach-02

i = 1;

while i <= 5:

print("Chitkara")

i+=1#i = i + 1

i = 1 \[1 <= 5: T\]

i = 2 \[2 <= 5: T\]

i = 3 \[3 <= 5: T\]

i = 4 \[4 <= 5: T\]

i = 5 \[5 <= 5: T\]

i = 6 \[6 <= 5: F\]

Output

Chitkara

Chitkara

Chitkara

Chitkara

Chitkara

This approach is very smart as it is scalable and it has no duplicacy.

What is output of following code

i = 10

while i <= 10:

print("Python")

i+=1

i = 10 \[10 <= 10: T\]

i = 11 \[11 <= 10: F\]

Output

Python

What is output of following code

i = 11

while i <= 10:

print("Python")

i = i - 1

i = 11 \[11 <= 10: F\]

Output

No output

What is output of following code

i = 1

while i <= 10:

print("Python")

i = i - 1#outside body of while statement

Execution Pattern

i = 1 \[1 <= 10: T\]

i = 1 \[1 <= 10: T\]

i = 1 \[1 <= 10: T\]

...

Output

python will be printed for infinite times
