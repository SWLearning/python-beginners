# 1. Syntax
What is syntax?! Well, syntax is a fancy word for how a language is structured! When we use this word, we simply 
mean: "the correct way to write something in that programming language".

## Contents
In this lesson, we will be covering the following topics and how we write them in Python:
1. Print
2. Variables
3. Data Types
4. Basic Operators

## 1. Print
We will start in Python with one of the most useful tools the language has to offer! That is the `print` statement. 
This will allow us to display text that we generate from our programs which will help us know that our code is working!

Below is an example for you to try to get you started with this feature:

```python3
print("Hello, World!")
```

Congratulations, you have written your first ever program! Did you notice that the program displayed some text back to 
us? That is our program output and this is something we will be using a lot of later on (and will go into more depth 
with too)!

## 2. Variables

### What is a variable?
- A variable is a way to save a useful piece of information so that we can come back to it later! For example, if 
  someone told us about a really funny website, we would want to write it down somewhere so that we don't forget! Then,
  whenever we want to look at that website, all we have to do is look at what we have written down!

### Example:
In Python, we "declare" (create) a variable with the following syntax:

```python3
funny_website = "https://xkcd.com/1739/"
```

A variable (as shown above) can be thought of as having two parts:
- **Name**: in this example, its name is `funny_website` and this is how we can refer to the variable later on.
- **Value**: in this example, the value of the variable has been set to `"https://xkcd.com/1739/"`.

### Let's create some variables!
Recreate the following code to see how variables work in Python! You can change the variable names and the variable 
values as much as you like!

```python3
# Let's create some variables
age = 12
name = "Alice"
is_student = True

# Print out the values
print("Name: ", name)
print("Age: ", age)
print("Is student? ", is_student)
```

### Why are they called variables?
Variables might seem like a strange name! But there is a reason for the name, and that is because the values can be 
changed while the program is running.

This means that the values can be thought of as "variable".

In the example below, you can see how we change a variable and then see the outcome of this:

```python3
# Sun is shining!
temperature = "25°C"
print("It's nice and warm today! What is the temperature?")
print(temperature)

# The clouds roll in!
temperature = "18°C"
print("Oh no, the sun's gone! What is the temperature?")
print(temperature)
```

In this example, the variable `temperature` is originally set to the value of `"25°C"`, but then later on we change 
the temperature to be `"18°C"`.

## 3. Data Types
In programming, variables can have different "types" of values. These types behave differently to each other because 
they represent different things! Below is a list of common data types that you will use when writing code in Python!

#### `string`
You have already been using strings without even knowing! Strings are used to represent any text, which could 
include words or numbers!

You can tell if a variable is a string if it has speech marks around it. Below are some examples:
- `"Hello!"`: this is a string because it has double speech marks around it!
- `'Goodbye!'`: this is also a string, you can use either `'` or `"` to create a `string`.
- `2`: this IS NOT a `string` because it doesn't have speech marks around it!
- `"2"`: this IS a `string` because even though it is a number, it has speech marks around it.

#### `integer` (or `int`)
Integer is a fancy name for a whole number! 40, 1, 36, and 100 are all examples of integers because they are whole 
numbers, but 2.5 is not an integer because it is a decimal number instead!

***Note:** because programmers are lazy, we usually refer to integers as ints because it is quicker and easier to say!*

Here are a few examples in Python:
- `2`: this IS an `integer`.
- `"2"`: this IS not an `integer` because it is surrounded with speech marks. Those speech marks make it a `string` 
  instead.

#### `float`
Float?! What is that supposed to be?!

Well, `float` is what is used to describe "decimal" or "non-whole" numbers in Python. A number like 1.5 would have 
the `float` data type because it is a decimal number instead.

- `2.5`: this is a `float`.
- `"2.5"`: this IS NOT a `float` because it has speech marks around it instead.
- `2`: this IS NOT a `float` because it is a whole number (this is an `integer`).
- `2.0`: Ahhh, so this must be an `int` because it is a whole number right? Ahh well, because we have written out 
  the `.0` at the end, Python will still treat this like a `float` instead of an `int`.

#### `boolean` (or `bool` for short!)
Ok, these data types are just getting silly now! `boolean` surely isn't a real word!!!

Well yes, that is right! It is actually named after [George Boole](https://en.wikipedia.org/wiki/George_Boole) who 
came up with the idea long before computers even existed!

A `boolean` is simply a `True` or `False` value in Python. Although this is such a simple data type, they are 
greatly important in programming because of the way computers work! This is something we will cover more later on.

Examples:
- `True`: this IS a `boolean`.
- `False`: this IS a `boolean` as well!
- `"True"`: this IS NOT a `boolean` because it is surrounded be speech marks. This is instead a `string`!
- `3`: this also IS NOT a `boolean`, this is an `integer`.

### Code example!
Ok, wow that was a lot to get through! It's all well and good knowing what data types are, but let me write some 
code already!

Below is a demonstration of different data types in Python so you can see what they would look like in the wild and 
know how to spot them!

```python3
age = 12 # This is an int (integer)
pi = 3.14159 # This is a float
name = "John" # This is a string
is_raining = False # This is a bool
something = 2.0 # You tell me!
```

Ok, so now a quick test! Can you work out what the data type of the variable `something` in the example above is?
>! `float` is the answer! Did you work it out?

## 4. Operators
Nearly there! One more thing to cover in this first lesson, and that is the concept of operators! For now, let's 
think of an operator as something that we can use to put our variables from the last section to work!

There are a few different types of operators that we will cover now with some basic examples of how to use them!

- Assignment Operator
- Arithmetic Operators
- Comparison Operators
- Logical Operators

### Assignment Operator (`=`)
This one is nice and simple, and you have already been using it without even knowing! The assignment operator in 
Python is the single equals sign `=`.

This is used to save a value into a variable (remember that from all the way back in the variables section?). To 
recap, below is a quick example of this:

```python3
my_variable = "value"
```
 In this example, the assignment operator is "assigning" (fancy word for saving or storing) the value on the right 
 hand side (`"value"`) into the variable on the left hand side (`my_variable`).
 
### Arithmetic Operators (`+`, `-`, `*`, `/`)
Arithmetic is another super fancy word that has a really simple meaning. This one means manipulating numbers! Below 
are a list of the basic arithmetic operators to get you started:

- `+`: **add**.
- `-`: **subtract** (take away).
- `*`: **multiply** (times), you may know this one as ×.
- `/`: **divide**, you may know this one as ÷.

All of these operators are designed to be used with the number types (`integer` and `float`). Let's explore these by 
writing some code!

```python3
# Arithmetic on integers
addition_result = 1 + 2 # Equals 3
subtraction_result = 5 - 2 # Equals 3
multiplication_result = 2 * 3 # Equals 6
division_result = 10 / 5 # Equals 2

# Arithmetic on floats
addition_result = 1.2 + 2.3 # Equals 3.5
subtraction_result = 5.0 - 2.5 # Equals 2.5
multiplication_result = 1.2 * 3 # Equals 3.6
division_result = 9.0 / 2.0 # Equals 4.5
```

When a number (`int` or `float`) is stored in a variable, you can use these operators with those variables as well! 
See how we have done this in the example below:

```python3
first_number = 3
second_number = 5
result = first_number + second_number
```

Can you guess what value is stored in the variable `result`?
>! It is the number 8! Well done if you worked that out!

Also, can you remember what we can do to "output" something from our program? If we add the `print` statement to the 
above example, we can get our program to tell us what the result is!

```python3
first_number = 3
second_number = 5
result = first_number + second_number
print(result)
```

### Comparison Operators
One thing that comes up very often when programming is the comparison of two values, how else will we know if apples 
are the same as oranges?!

In python (and most other programming languages!), the following comparison operators are provided to us:

- `==`: This checks if one thing "is equal to" another.
- `!=`: This checks if on thing "is not equal to" another.
- `>`: This checks if a thing is "greater than" another.
- `<`: This checks if a thing is "less than" another.
- `>=`: This checks if a thing is "greater than or equal to" another thing.
- `<=`: This checks if a thing is "less than or equal to" another thing.

Ok, ok... but how do I actually use them?! Let's see them in action:

```python
var1 = 36
var2 = 36

# lets compare the two variables above and print the result
print(var1 == var2) # this prints True
```

In the example above, we create two variables (`var1` and `var2`) that are both given the same value: `36`. Then we 
compare the values with the "is equal to" operator and print the result!

Below are examples of all the operators in action!

```python
a = 10
b = 5

print("Equal to:", a == b)                  # Output: False
print("Not equal to:", a != b)              # Output: True
print("Greater than:", a > b)               # Output: True
print("Less than:", a < b)                  # Output: False
print("Greater than or equal to:", a >= b)  # Output: True
print("Less than or equal to:", a <= b)     # Output: False
```

### Logical Operators
No, not more operators! Yes, but don't worry, these are the last ones we need for now!

Logical operators are fundamental to how computers work, and when put together, can be very powerful! They allow us to
combine True and False statements. For now, I will list the logical operators below, and explain them after:

- `and`: returns true if both things are True.
- `or`: returns true if either thing is True.
- `not`: returns the opposite of what the thing is!

```python
# and statements
print(True and True) # prints True
print(True and False) # prints False
print(False and False) # prints False

# or statements
print(True or True) # prints True
print(True or False) # prints True
print(False or False) # prints False

# not statements
print(not True) # prints False
print(not False) # prints True
```

Wow, that's a lot of things to remember! But when would I use these operators??

Well, when you want to do something when more than one thing is true, for example:
- When do you want to put an umbrella up?
  - When it is raining **AND** you are outside!

If it was raining but you where inside, then you wouldn't need the umbrella! (Not unless you want bad luck!) But if 
you are outside and it is raining, then the umbrella would be very useful!

Don't worry if this doesn't all make sense yet, we will explore this more in the next lesson, but well done! You 
have reached the end of lesson 1! Now go hand have a well-earned break!!