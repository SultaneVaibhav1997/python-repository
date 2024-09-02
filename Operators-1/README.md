### Student Notes for Mathematical Operators & Comparison Operator

Operators are used to perform operations on variables and values.

## What are the basic mathematical operations?

![Screenshot (308).png](<Mathematical%20Operators%20&%20Comparison%20Operator%205d2a6496214946488eb4ebc5d08758e6/Screenshot_(308).png>)

The common operators in Javascript are :

- **Addition**
- **Subtraction**
- **Multiplication**
- **Division**

Problem: Given a = 15, b = 25 . Calculate sum, difference, product, and division.

### Real-world example

![Untitled](Mathematical%20Operators%20&%20Comparison%20Operator%205d2a6496214946488eb4ebc5d08758e6/Untitled.png)

- Visit amazon.com, and add some products to the cart.
- Adding products leads to an increase in the cart price.
- Manipulating the quantity or Adding the items affects the total price. This is how Mathematical operators are used behind the picture.

## Modulo Operator(%) [Remainder]

![Untitled](Mathematical%20Operators%20&%20Comparison%20Operator%205d2a6496214946488eb4ebc5d08758e6/Untitled%201.png)

- When we divide a number into another, there are 4 terms that we need to understand
  - **quotient**
  - **divisor**
  - **dividend**
  - **remainder**
- Looking at the above picture, you will get clear about the above terms
- The remainder represents by **%**.
  - For Ex: var result = 75 % 4 [ Read as 75 Modulus 4 ]

### Explaining Modulus

**Let's take the analogy**:

- There are many candidates who came to the company office to give interviews.
- Since there are more than **100 candidates**, **4 interview panel setups** where one interviewer is used to take the interviews.
- A **unique Id** is assigned to each candidate, starting from 1,2,3........to 100. If Interview Panel 1 is assigned to ID 1, Interview Panel is assigned to ID 2, and so on.
- Now, the question is Which Interview Panel will be assigned to Candidate 25?

  - The Solution Lies in Modulus: Just calculate **25 % 4** [ Since there are 4 Interview Panel]
  - Result = 25 % 4 = 1
  - Candidate 25 is assigned to Interview Panel 1.

  ![Screenshot (304).png](<Mathematical%20Operators%20&%20Comparison%20Operator%205d2a6496214946488eb4ebc5d08758e6/Screenshot_(304).png>)

- **The power of % lies in distributing**

![Untitled](Mathematical%20Operators%20&%20Comparison%20Operator%205d2a6496214946488eb4ebc5d08758e6/Untitled%202.png)

### Google Server Analogy

Also, Using the same analogy of 4 Google servers and more than 1000 requests coming in a sequence.

Which server will process the 63rd request?

## Exponentiation Operator(\*\*)

### Explain the exponentiation operator with examples, Also discuss the difference between \* and \*\*

- It is used to compute the power of any number
  - a = 4
  - b = 2
  - c = a**b = 4**2 = 4\*4 = 16

### **Difference between \* and \*\***

![Screenshot (305).png](<Mathematical%20Operators%20&%20Comparison%20Operator%205d2a6496214946488eb4ebc5d08758e6/Screenshot_(305).png>)

### Find Square root using Exponentiation Operator

     Find the  Square root of 3 using the Exponentiation Operator

     **Solution :** result = 3**0.5

## How to Solve long expression?

![How.png](Mathematical%20Operators%20&%20Comparison%20Operator%205d2a6496214946488eb4ebc5d08758e6/How.png)

###  Discuss the steps to solve long expressions using brackets

- If you want to solve long expressions containing multiple operations then use brackets.
- Putting brackets also gives readability to code.
- For Ex :
  - **expr = ((a+b)\*(c+d))/e**

### Solve the Expression

- **For Ex** :
  **a = 3;**
  **b = 2;**
  **c = 4;**
  **sum = (a*2) + (b*2) + (c*2); #(3*2)+(2*2)+(4*2)**
  **print(sum) # 18 is the sum**

## String Concatenation

###  Discuss examples of how to concatenate multiple strings

- Concatenation means a series of interconnected things.
- Use + to join two or more string

**Example 1 :**

```objectivec
name = "Maddy";
print("Hello "+name+" Welcome To Masai");
```

**Example 2 :**

```objectivec
a = "Masai"
b="School";
line = a+" "+b;
print(line);
```

- The problem statement is to store the following information into a unique variable i.e.
  - **House No**
  - **Area**
  - **City**
- The task is to print the complete address.

**Concatenation with Numbers**

```coffeescript
num1 = 2;
num2 = 3;
sum = num1 + num2;
print("Sum is ",sum);
```

### If you could write a book, what would it be about?

## What are Comparison Operators?

Comparison operators are used for comparing two values.

- There are 6 comparison operators:
  - **> (Greater Than)**
  - **>= (Greater Than Equal To)**
  - **< (Less Than)**
  - **<= (Less Than Equal To)**
  - **== (Equal)**
  - **!= (not Equal)**
- The result of a comparison operator is always a boolean value.

### Greater Than Operator ( > )

![Untitled](Mathematical%20Operators%20&%20Comparison%20Operator%205d2a6496214946488eb4ebc5d08758e6/Untitled%203.png)

- The first value is strictly greater than the second value. For ex-
  ```python
              a = 5;
              b = 4;
              print(a>b);     # Outputs True
  ```
- The first value is less than or equal to the second value. For ex-

  ```python
             a = 5;
             b = 5;
             print(a>b);      # Outputs False
  ```

       **Code 1: Check whether the Ram age is greater than Mohan or not**

```python
age_of_ram = 25;
age_of_mohan = 30;
print(age_of_ram > age_of_mohan);  # Outputs False
```

      **Code 2: Check whether Sunil is passed or not, where the passing mark is 35**

```python
sunil_marks = 36;
passing_marks = 35;

is_passed = sunil_marks>passing_marks;
print(is_passed);                  # true : Sunil is passed
```

There is some problem with the above solution, what if the Sunil mark is 35

In that case, the above code will give the result false but in reality, it should be true

```python
sunil_marks = 35;
passing_marks = 35;

is_passed = sunil_marks>passing_marks;
print(is_passed);                # false : Sunil is failed

```

thus, we will use ≥ **(greater than or equal to)** to solve this problem

```python
sunil_marks = 35;
passing_marks = 35;

is_passed = sunil_marks>=passing_marks;
print(is_passed);                # true : Sunil is passed

```

**Note :**

- **3 > 3 is False**
- **2 > -3 is True**

### Greater Than Equal To Operator ( >= )

- The first value is greater than or equal to the second value. For ex :
  ```python
  			 a = 5;
         b = 5;
         print(a>=b);     #   True
  ```
- The first value is less than the second value. For ex :

  ```python
  			 a = 3;
         b = 5;
         print(a>=b);     #  False

  ```

  **Code 3: Try these questions on Replit**

  ```python
  '''**Questions:**
   10>6, 10>=6, 10>=10, 10>10, -9>-8'''

  # **Solutions:**
  print(10>6);
  print(10>=6);
  print(10>=10);
  print(10>10);
  print(-9>-8);
  ```

  **Note :**

  - **3 >= 3 is True**
  - **2 >= -3 is True**

### Less Than Operator ( < )

![Untitled](Mathematical%20Operators%20&%20Comparison%20Operator%205d2a6496214946488eb4ebc5d08758e6/Untitled%204.png)

- The first value is strictly less than the second value. For ex :
  ```python
  			 a = 4;
         b = 5;
         print(a<b);    # True
  ```
- The first value is greater than or equal to the second value. For ex :
  ```python
  				 a = 5;
  		     b = 2;
           print(a<b);   # False
  ```
  **Code 4: Check whether Sunil failed or not, where the passing mark is 35**
  ```python
  		sunil_marks = 34;
  		passing_marks = 35;
  		is_failed = sunil_marks<passing_marks;
  		print(is_failed);                # true : Sunil is failed
  ```
  **Note:** In the above code, we can not use ≤ (lesser than or equal to), it will give the wrong result

### Less Than Equal to Operator ( <= )

- The first value is strictly less than or equal to the second value. For ex :
  ```python
  			 a = 4;
         b = 5;
         print(a<=b);         # True
  ```
- The first value is greater than the second value. For ex :
  ```python
  				a = 6;
  	      b = 5;
          print(a<=b);      #  False
  ```

[Untitled design (1).mp4](<Mathematical%20Operators%20&%20Comparison%20Operator%205d2a6496214946488eb4ebc5d08758e6/Untitled_design_(1).mp4>)

### Problems

**Code 5: Those customers will be eligible for the amazon discount whose spending is equal to or above 4000. Check whether a customer Sam is eligible for a discount or not**

**Wrong Code**

```python
minimum_purchase = 4000;
sam_purchase = 5000;
eligible_for_discount = sam_purchase>minimum_purchase;
print(eligible_for_discount);

```

- The problem with the above code, we have used only greater than but in the question it was given that “**eligible for the amazon discount whose spending is equal to or above 4000”.**

**Correct Code**

```python
minimum_purchase = 4000;
sam_purchase = 5000;
eligible_for_discount = sam_purchase>=minimum_purchase;
print(eligible_for_discount);

```

**Code 6: Check whether Heeralal is eligible for driving a vehicle in India.**

- The legal age in India for driving a vehicle is 18 +.
  ```python
  age_of_heeralal = 18;
  legal_age = 18;
  drive_vehicle = age_of_heeralal>=legal_age;
  print(drive_vehicle);
  ```

### Equal ( == )

It checks whether the two operands are identical or not.

![Screenshot (309).png](<Mathematical%20Operators%20&%20Comparison%20Operator%205d2a6496214946488eb4ebc5d08758e6/Screenshot_(309).png>)

**For Ex :**

**5 == 5 is True,**

**"b" == "b" is True,**

**5 == "5" is False**

**Code 7: On Replit**

```python
	ram = "ram";
	print(5==5);
	print("masai"=="masai");
	print(5=="5");
	print(ram == "ram");
	print(5=="ram");

```

**Code 8: Find the output**

```python
		a = 5;
		b = 6;
		c = "6";
		d = -2;
		e = "m";
		print(b==c);
		print(c==e);
		print(a>=c);
		print(d<=a);
```

### Not Equal ( ! = )

**!=** opposite of **==**

![Screenshot (310).png](<Mathematical%20Operators%20&%20Comparison%20Operator%205d2a6496214946488eb4ebc5d08758e6/Screenshot_(310).png>)

**For Ex :**

**5 != 4 is True,**

**"a" != "A" is True,**

**"a" == "A" is False**

**Code 9: Find the output**

```python
print(5==5);
print(5!=5);
print(6=="6");
print(6!=7);
print("a"=="a");
print("a"!="a");

```

**Code 10: Find the output**

```python
	masai = 5;
	a = "masai";
	b = masai;
	print(a==b);
	print(a!=b);
```

**Happy Coding!**
