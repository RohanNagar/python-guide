## Printing

```python
# Print only a new line
print()

# Print a simple string message, followed by a new line
print('Hello World!')

# Print a string message with no newline at the end
print('No newline after this', end='')

# Print a string message with a space at the end
print('Put a space after this', end=' ')

# Print with an f-string
my_var = 10
my_second_var = 20
print(f'The value of variable one is {my_var} and the value of variable two is {my_second_var}')
```

## Operations

**Remember your order of operations!**

```
x = 3        # Assignment (set variable x to 3)
x += 1       # Add one to x (same as x = x + 1)
x -= 1       # Subtract one from x (same as x = x - 1)
x = 6 / 2    # Float division, will result in a float. Example 6 / 2 = 3.0)
x = 6 // 2   # Integer division, will result in an int. Example 6 // 2 = 3)
x *= 3       # Multiply x by 3 (same as x = x * 3)
x = 11 % 10  # Modulo operator. Gives you the remainder. Example 11 % 10 = 1)
x = 2 ** 3   # Power operator. 2 ** 3 is the same as 2 to the power of 3, which is 2*2*2 = 8)
```

## Types and Conversions

```python
# Find the type of something using the type() function

print(type(10))     # Prints <class 'int'>
print(type(22.0))   # Prints <class 'float'>
print(type('hi'))   # Prints <class 'str'>
print(type(True))   # Prints <class 'bool'>
```

```python
x = int("15")       # turns the str "15" into the int 15
x = int(15.7)       # turns the float 15.7 into the int 15 (throws away decimal)

x = float(5)        # turns the int 5 into the float 5.0
x = float("3.0")    # turns the str "3.0" into the float 3.0

x = str(3)          # turns the int 3 into the str "3"
x = str(7.0)        # turns the float 7.0 into the str "7.0"

x = chr(65)         # turns the int 65 into the character 'A' (uses the ASCII chart to map int to chr)
x = chr(97)         # turns the int 65 into the character 'a' (uses the ASCII chart to map int to chr)
```

## Importing Modules

```python
# Import a full module, then use "module.function()" syntax
import math

math.sqrt(25)
math.sin(30)
math.cos(30)

# Import select functions from a module, then just use "function()" syntax
from random import randint, random

randint(1, 30)
random()
```

## Boolean Logic

```
x > 2      # True if x is greater than 2, False if it is not
x >= 2     # True if x is greater than or equal to 2, False if it is not
x < 2      # True if x is less than 2, False if it is not
x <= 2     # True if x is less than or equal to 2, False if it is not
x == 2     # True if x is equal to 2, False if it is not
x != 2     # True if x is NOT equal to 2, False if it is equal to 2

x > 2 or y < 2     # True if either x > 2 or y < 2, or both. Only False if both of these are False
x > 2 and y < 2    # True only if BOTH x > 2 and y < 2. False if either one is False
not x > 2          # True if x is NOT greater than 2
```

## Input

```python
# Ask the user to input a string
user_input = input('Enter a string value: ')

# Ask the user to input an integer
user_input = int(input('Enter an integer value: '))

# Ask the user to input a float
user_input = float(input('Enter a decimal value: '))
```

## If/Else

```python
if boolean_expression:
  do_something()
elif some_other_expression:
  do_something_else()
else:
  do_another_thing()
```

Example:

```python
x = 100

if x > 0:
  print(f'The number {x} is positive!')
elif x < 0:
  print(f'The number {x} is negative!')
else:
  # Else we know that it was not greater than zero or less than zero, so it must be zero
  print(f'The number {x} is zero!')
```
