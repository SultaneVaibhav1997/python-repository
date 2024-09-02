### Student Notes for Introduction to Python & Variables, Data Types

## What is Python?

![Screenshot (282).png](<Introduction%20to%20Python%20&%20Variables,%20Data%20Types%20a89a3114c1884ef7b6ed3d7df17d2d4a/Screenshot_(282).png>)

- Python is an **interpreted**, **object-oriented**, **high-level** programming language with dynamic semantics.
- It was created by **Guido van Rossum** and released in **1991** at **CWI [Centrum Wiskunde and Informatica] Research Center, Netherlands**.

![Guido van Rossum](Introduction%20to%20Python%20&%20Variables,%20Data%20Types%20a89a3114c1884ef7b6ed3d7df17d2d4a/Untitled.png)

Guido van Rossum

![CWI Research Center, Netherlands, Amsterdam](Introduction%20to%20Python%20&%20Variables,%20Data%20Types%20a89a3114c1884ef7b6ed3d7df17d2d4a/Untitled%201.png)

CWI Research Center, Netherlands, Amsterdam

- It is a general-purpose language, meaning **it can be used to create a variety of different programs and isn't specialized for any specific problems.**
  - It can be used for Machine Learning and Artificial Intelligence.
  - It is the number 1 language for Data Science Projects.
  - It is popular in Web Development. Using the Django framework, you can build amazing websites.
  - Four Websites powered by **Python** & **Django**➖
    **Youtube, Spotify, Pinterest, Instagram, Dropbox**
    ![Screenshot (283).png](<Introduction%20to%20Python%20&%20Variables,%20Data%20Types%20a89a3114c1884ef7b6ed3d7df17d2d4a/Screenshot_(283).png>)
  - It is used in Automation.

## Why the name Python?

- **Guido van Rossum** was reading the script of a popular BBC comedy series "**Monty Python's Flying Circus**". It was late on-air 1970s.
  ![Untitled](Introduction%20to%20Python%20&%20Variables,%20Data%20Types%20a89a3114c1884ef7b6ed3d7df17d2d4a/Untitled%202.png)
- Van Rossum wanted to select a name that said unique, sort, and mysterious. So, he decided to select naming **Python** after **"Monty Python's Flying Circus"** for their newly created programming language.
- The comedy series was **creative** and **well random**. It talks about everything. Thus, it is slow and unpredictable, which made it very interesting.

## Why Python?

- **Simple and Easy to Learn**
- **Dynamic**
- **Platform Independent**
- **Free and Open Source**
- **Interpreted (bytecode-compiled)**
- **Rich Library Support (more than 1,37,000 third-party python libraries)**
- **Embeddable and Extensible**
- **Portable**
- **Robust**
- **Exception Handling**

![Untitled](Introduction%20to%20Python%20&%20Variables,%20Data%20Types%20a89a3114c1884ef7b6ed3d7df17d2d4a/Untitled%203.png)

## [Instructor task: 5min] Discuss Indentation

discuss briefly with examples.

## Setup Replit[2-3 min]

- Go to [https://replit.com](https://replit.com/)
- Sign up with your Gmail account.
- Choose **Python** and it will open a window asking you to create a repl.
- Press create repl.
- A new window will open, On the **left side**, you will find the **code editor** and on the **right side** is the **terminal** where we can see our **output**.

## How to print or get output in Python?

### **_print( )_**➖

The `print()` function prints the specified message to the screen or other standard output device.

The message can be **a string** or **any other object**, the object will be converted into a string before being written to the screen.

![Untitled](Introduction%20to%20Python%20&%20Variables,%20Data%20Types%20a89a3114c1884ef7b6ed3d7df17d2d4a/Untitled%204.png)

## **Python Comments**

- Comments can be used to explain Python code.
- They make the code more readable.
- They prevent execution when testing code.
- Comments are of two types:
  - **Single line Comment** (comments start with a #)
  - **Multiline Comment** ( place your comment inside triple quotes (’’’ ‘’’))

## Variables

Variables are containers for storing data values.

### Creating Variables

Python has no command for declaring a variable.

A variable is created when you first assign a value to it.

![Untitled](Introduction%20to%20Python%20&%20Variables,%20Data%20Types%20a89a3114c1884ef7b6ed3d7df17d2d4a/Untitled%205.png)

### Instructor Task (3 mins): Show how we can print variables and values,

Show live demo on Replit

- To know what is present inside the box, we need to use **print()**.

### Get the Type

You can get the data type of a variable with the `type()` function.

![Untitled](Introduction%20to%20Python%20&%20Variables,%20Data%20Types%20a89a3114c1884ef7b6ed3d7df17d2d4a/Untitled%206.png)

## Variables

### Instructor Task (10 mins): Talk about variables

- Let's try to understand with a story

  - There was a child who once decided to leave his home and move to a different place. He does his packing.
  - There was a lot of stuff that needs to be packed. So, What he did, He arrange some boxes and In each box, he used to put some set of things For ex: Pictures, Shoes, Shirts, pillows, books, toys, etc.
    ![Untitled](Introduction%20to%20Python%20&%20Variables,%20Data%20Types%20a89a3114c1884ef7b6ed3d7df17d2d4a/Untitled%207.png)

- For Identification, He marked each box with a name Like a box containing pictures has the name pictures, the box which contains books marked as books, etc.
- We relate this story to the concept of variables,
  - The boxes are considered as variables where you can put your set of things.
    ![Untitled](Introduction%20to%20Python%20&%20Variables,%20Data%20Types%20a89a3114c1884ef7b6ed3d7df17d2d4a/Untitled%208.png)
  - It is used to **_hold data_** that you can choose later.
  - The variable is **_storage locations with assigned names_**.

## Need of Variable

### Instructor Task (3 mins): Talk about why we need it and how is it used in real life.

- Different customers who log in to Amazon, Flipkart, or Facebook should see their name on the top, not a fixed name.
- The variable *"custName"* can be used to store the customer's name.

![Untitled](Introduction%20to%20Python%20&%20Variables,%20Data%20Types%20a89a3114c1884ef7b6ed3d7df17d2d4a/Untitled%209.png)

- It is like a box holding different values depending on who is visiting and logged in to the website.
- In the front end, Using Forms we use to take the values for different variables like Facebook signup forms carrying different variables like name, age, etc.

## Rules for Declaring Variables

- A variable name must start with a letter or underscore character ( \_ ).
- A variable name cannot start with a number.
- A variable name can only contain alphanumeric letters ( A-Z, a-z, 0-9 ) and an underscore ( \_ ).
- Variable names are case-sensitive. (age ≠ Age ≠ AGE)

## **Multi Words Variable Names**

Variable names with more than one word are difficult to read.

**Various ways by which you can use to make them more readable**:

- **Camel Case**➖ Each word, except the first, starts with a capital letter.
  Examples➖ myCar, firstPriceValue, etc.
- **Pascal Case**➖ Each word starts with a capital letter:
  Examples➖ MyCar, FirstPriceValue, etc.
- **Snake Case**➖ Each word is separated by an underscore character.
  Examples➖ my_car , first_price_value, etc.

### Instructor Task (2 mins): Introduce Data types

Apart from the customer's name,  a website may also need to know the customer's age. This would be another variable "_custAge"._

While *custAge is* also a variable but it holds a number, not a word (called a *string* in Python). Variables can have different "data types".

## Datatype

### Instructor Task (10 mins): Talk about different Data types

![Screenshot (293).png](<Introduction%20to%20Python%20&%20Variables,%20Data%20Types%20a89a3114c1884ef7b6ed3d7df17d2d4a/Screenshot_(293).png>)

As we discussed earlier, **variables are like boxes/containers**.

Above are three containers - What type of things will we store in the pencil holder? What type of things will we store in a water bottle?

Can you store milk in a basket or can you use a bottle to store fruits?

We are using different types of containers to store different things.

While the bottle can hold milk or water or juice, it will hold only liquids.

Similarly,

- A variable of type **_string_** (like the variable - *custName*), can store only strings.
- A variable of type **int** (like the variable - *custAge)* can store only integers.
- A variable of type **boolean** (like the variable - *custMaritalStatus)* can store either true or false.
- A variable of type **float** (like the variable - fruitWeight*)* can store only decimal values.

*The type of data a variable can hold is called its* **Data type**. It may be **int**, **string, boolean, float,** etc. (A variable of type Boolean can either be *True* or *False).*

## Int

![Screenshot (295).png](<Introduction%20to%20Python%20&%20Variables,%20Data%20Types%20a89a3114c1884ef7b6ed3d7df17d2d4a/Screenshot_(295).png>)

![Screenshot (294).png](<Introduction%20to%20Python%20&%20Variables,%20Data%20Types%20a89a3114c1884ef7b6ed3d7df17d2d4a/Screenshot_(294).png>)

## **String**

![String.png](Introduction%20to%20Python%20&%20Variables,%20Data%20Types%20a89a3114c1884ef7b6ed3d7df17d2d4a/String.png)

![str2.png](Introduction%20to%20Python%20&%20Variables,%20Data%20Types%20a89a3114c1884ef7b6ed3d7df17d2d4a/str2.png)

### Can they think of any other example like the car number plate, where a sequence of numbers is not important for their value?

One common example could be the Aadhaar card number. It is full of numbers but their “numerical value” is not how its used. We don’t say my Aadhaar number is "5 billion, 350 million …." We say it’s "5350…".

_var aadhaarNum = “535067543542”;_

vs

_var aadhaarNum = 535067543542;_

## Boolean

This datatype has only two values i.e. **True and False;**

- Some Questions are only answered in True or False :
  - For Ex :
    - Whether Student is Pass or Fail: Either True or False
    - Whether the Age is above 18 or not
- For Ex :
  - `driving = true;`
  - `smoke = false;`

### Real-World Example [5 min]

- When the user logged in to any platform like Amazon, Facebook, Gmail, etc. then the user needs to log in.
- When the user gets logged_in then in the backend the logged_in flag got true.

  - If user logged_in, then logged_in = true
  - If user logged_out , then logged_in = false

- During Shopping on the e-commerce platform. Some platform offers a 10% discount on the product only when you will use a credit card.
- Thus, the Credit card flag is set to true, only when you use a credit card.

![Screenshot (299).png](<Introduction%20to%20Python%20&%20Variables,%20Data%20Types%20a89a3114c1884ef7b6ed3d7df17d2d4a/Screenshot_(299).png>)

![Screenshot (297).png](<Introduction%20to%20Python%20&%20Variables,%20Data%20Types%20a89a3114c1884ef7b6ed3d7df17d2d4a/Screenshot_(297).png>)

### Task to print the following information [ 5 min ]

- Name
- Age
- Gender
- has_driving_license
- citizen_of_india

## Float

![Screenshot (298).png](<Introduction%20to%20Python%20&%20Variables,%20Data%20Types%20a89a3114c1884ef7b6ed3d7df17d2d4a/Screenshot_(298).png>)

![Screenshot (296).png](<Introduction%20to%20Python%20&%20Variables,%20Data%20Types%20a89a3114c1884ef7b6ed3d7df17d2d4a/Screenshot_(296).png>)

## How to declare a variable?

### Instructor Task (3 mins): Discuss how to declare a variable, Show them a live demo on Replit.

- In python, the variable is declared is as follows
  - x = 2;
  - y = "Masai";
  - z = 4.5 ;
  - w=True;
- **(CASE SENSITIVE)**
  x=2
  X=3
  X ≠ x

### **Python is a fantastic language that automatically identifies the type of data for us**.

![Screenshot (300).png](<Introduction%20to%20Python%20&%20Variables,%20Data%20Types%20a89a3114c1884ef7b6ed3d7df17d2d4a/Screenshot_(300).png>)

### Perform the task

- Give a task to create a variable of their name, age, and gender and print the type of it on Replit.

## Many Values to Multiple Variables

Python allows you to assign values to multiple variables in one line.

Ex➖

```cpp
x,y,z= "box", "pencil", "eraser"

print(x)    # box
print(z)    # pencil
print(y)    # eraser
# The number of variables matches the number of values, or else you will get an error
```

## One Value to Multiple Variables

Python allows you to assign the *same* value to multiple variables in one line.

Ex➖

```cpp
a=b=c="Maggi"
print(a)    # Maggi
print(b)    # Maggi
print(c)    # Maggi
```

## Type **Casting in Python**

Type Casting is the method to convert the variable data type into a certain data type in order to the operation required to be performed by users.

There can be two types of Type Casting in Python –

- Implicit Type Casting
- Explicit Type Casting

### Implicit Type Casting

In this, Python **converts the data type** into another data type **automatically**. In this process, users don’t have to involve in this process.

### Explicit Type Casting

In this, Python needs **user involvement to convert the variable data type** into a certain data type in order to the operation required.

Mainly type casting can be done with these data type functions:

- i**nt(): i**nt() function take float or string as an argument and return int type object.
- **float():** float() function takes int or string as an argument and returns float type object.
- **str():** str() function take float or int as an argument and return string type object.
- **bool():** str() function take float or int as an argument and return a boolean-type object.

![Screenshot (302).png](<Introduction%20to%20Python%20&%20Variables,%20Data%20Types%20a89a3114c1884ef7b6ed3d7df17d2d4a/Screenshot_(302).png>)
