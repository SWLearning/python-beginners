# Control Structures

## Introduction
When we write code, we want to control the flow of the program to ensure that it does what we want depending on
certain things! We make decisions every day based on different things, like if it is warm, we go outside! Control
structures help our programs do things and make decisions just like we would as humans!

## `if` statements
There are a few different parts to `if` statements:
- `if`
- `elif` (short for "else if")
- `else`

We will explain these in more detail below.

### `if`
If statements allow us to make decisions in our programs. They help our program choose what to do based on whether a
condition is true or false. For example:

```python3
sun_is_shining = True

if sun_is_shining: 
    print("Let's go outside!")
```

Here is a good example of when we might use a logical operator from the last lesson! Have a go at copying the example
below:

```python3
is_raining = True
you_are_outside = True

if is_raining and you_are_outside:
    print("Put up your umbrella!")
```

Play around with this and see what happens if you change the values of `is_raining` and `sun_is_shining` to `False`
instead!

### `elif`
`elif` (short for "else if") lets us check for other scenarios if the initial `if` statement wasn't `True`, for
example:

```python3
temperature = 5

if temperature == 100:
    print("Boiling Point!")
elif temperature == 28:
    print("Perfect temperature for sitting outside!")
elif temperature == 5:
    print("Fridge Cold!")
elif temperature == 0:
    print("Freezing Point!")
```

So what happens with this code? Well when it runs, it goes something like:
1. Is the temperature equal to 100?
   - No! Skip this line and move to the next `elif`.
2. Is the temperature equal to 28?
   - No! Skip this line and move to the next `elif`.
3. Is the temperature equal to 5?
    - Yes! So run this line and then exit the `if` statement!

When you build up an `if` statement like this, only one of the sections will run (or none!). So it would be impossible
for the program to say both "Boiling Point!" and "Fridge Cold!" at the same time!

### `else`
Sometimes, we want to do something particular under one condition, but want to do something else for any other
condition, for example if we were to say "Hello" to someone on their birthday, we might say "Hello, happy birthday!",
but if it isn't their birthday, we just want to say "Hello"!

See the example below for how `else` can help us with this:

```python3
birthday = "15/02"
today = "18/05"

if birthday == today:
    print("Hello, happy birthday!")
else:
    print("Hello!")
```

Try this and see what happens! And for bonus points, try and make the program output "Hello, happy birthday!" by 
changing the value in the `today` variable.