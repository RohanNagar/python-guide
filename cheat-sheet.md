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
print(f'The value of var one is {my_var} and the value of var two is {my_second_var}')
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
x = 2 ** 3   # Power operator. Same as 2 to the power of 3, which is 2*2*2 = 8)
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

x = chr(65)         # turns the int 65 into the character 'A' (uses the ASCII chart)
x = chr(97)         # turns the int 65 into the character 'a' (uses the ASCII chart)

x = ord('A')        # turns the character 'A' into the int 65 (uses the ASCII chart)
x = ord('Z')        # turns the character 'Z' into the int 90 (uses the ASCII chart)
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

# Import all functions from a module, then just use "function()" syntax
from random import *

randint(1, 32)
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

x > 2 or y < 2     # True if either x > 2 or y < 2, or both
x > 2 and y < 2    # True only if BOTH x > 2 and y < 2
not x > 2          # True if x is NOT greater than 2
```

### Truth Tables

| **AND** | | | | | 
| --- | --- | --- | --- | --- |
| a | T | T | F | F |
| b | T | F | T | F |
| a and b | T | F | F | F |

| **OR** | | | | | 
| --- | --- | --- | --- | --- |
| a | T | T | F | F |
| b | T | F | T | F |
| a or b | T | T | T | F |

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

## Strings

```python
my_str = 'Hello There'

len(my_str)      -> 11      # Get the length of a string (number of characters in the str)
my_str[0]        -> 'H'     # Get the first character in a string
my_str[-1]       -> 'e'     # Get the last character in a string
my_str[1]        -> 'e'     # Get the second character in a string
my_str[-2]       -> 'r'     # Get the second to last character in a string

# To get a sub-string, do my_str[start:end] (remember end is not included!)
my_str[0:4]      -> 'Hell'
my_str[0:1]      -> 'H'
my_str[2:5]      -> 'llo'
my_str[:3]       -> 'Hel'          # start at beginning and end at index 2
my_str[3:]       -> 'lo There'     # start at index 3 and go to end
```

## String Functions

```python
my_str = "Hello" + " " + "World"     -> "Hello World"     # Add strings together
my_str = "Hey" * 3                   -> "HeyHeyHey"       # Can replicate strings too

my_str = "Hello World"

my_str.startswith('Hello')    -> True          # Returns a bool that is True if my_str starts with 'Hello'
my_str.endswith('Wrld')       -> False         # Returns a bool that is True if my_str ends with 'Wrld'

my_str.find('Wor')            -> 6             # Returns the index that 'Wor' first occurs in my_str
my_str.find('Not here')       -> -1            # find() returns -1 if the string is not found in my_str

my_str.index('Wor')           -> 6             # Similar to find(), index() returns index 'Wor' first occurs
my_str.index('Not here')      -> ValueError    # The difference with index() is it gives a ValueError
                                               #   if the string is not found

my_str.count('l')             -> 3             # Returns the number of times 'l' appears in my_str
my_str.upper()                -> 'HELLO WORLD' # Returns a new str that converted old string to all UPPER
my_str.lower()                -> 'hello world' # Returns a new str that converted old string to all lower

my_str.replace('o', 't')      -> 'Hellt Wtrld' # Returns a new str that replaced all 'o' with 't'
```

## Lists

```python
lst = ["Hello", 2, 4.0]       # Lists can have any types inside
lst = [[1, 2, 3], [4, 5, 6]]  # Even other lists

lst = [10, 20, 30, 40, 50]

len(lst)        -> 5          # Get the length of a list (number of elements in the list)
lst[0]          -> 10         # Get the first element in a list
lst[-1]         -> 50         # Get the last element in a list
lst[1]          -> 20         # Get the second element in a list
lst[-2]         -> 40         # Get the second to last element in a list

# To get a sub-list, do lst[start:end] (remember end is not included!)
lst[0:4]        -> [10, 20, 30, 40]
lst[0:1]        -> [10]
lst[2:5]        -> [30, 40, 50]
lst[:3]         -> [10, 20, 30]      # start at beginning and end at index 2
lst[3:]         -> [40, 50]          # start at index 3 and go to end
```

## List Functions

```python
lst = [1, 2] + [3, 4]     -> [1, 2, 3, 4]                # Add two lists together to make one longer list
lst = [1, 2] * 3          -> [1, 2, 1, 2, 1, 2]          # Replicate a list 3 times

lst = [1, 2, 3]
lst.append(4)           -> lst is now [1, 2, 3, 4]       # Add value 4 at the end of lst
lst.insert(1, 4)        -> lst is now [1, 4, 2, 3, 4]    # Insert at index 1 the value of 4,
                                                         #   and push everything else to the right
lst.count(4)            -> Returns 2                     # Count and return the amount of times 4 appears in lst
lst.index(4)            -> Returns 1                     # Return the index of the first occurance of 4
lst.remove(4)           -> lst is now [1, 2, 3, 4]       # Remove only the first value of 4 in lst
lst.pop()               -> lst is now [1, 2, 3]          # Remove the last item in lst
lst.pop(1)              -> lst is now [1, 4]             # Remove the item at index 1
lst.reverse()           -> lst is now [4, 1]             # Reverse the order of values in lst
lst.sort()              -> lst is now [1, 4]             # Sort the lst
lst.clear()             -> lst is now []                 # Removes all items from lst

x = min(lst)            # Find the minimum value in lst and return it (x is now equal to the min)
x = max(lst)            # Find the maximum value in lst and return it (x is now equal to the max)
x = sum(lst)            # Add up everything in lst and return it (x is now equal to
                        #   the sum of all the values in lst)
```

## Range

```python
range(start, end, step)  # end is not included, step default is 1, start default is 0

range(5)         -> 0 1 2 3 4
range(3, 8)      -> 3 4 5 6 7
range(2, 12, 3)  -> 2 5 8 11
range(20, 5, -5) -> 20 15 10
range(len(lst))  -> 0 1 2 .... length of lst - 1
```

## For Loops

**Use for loops when you know how many times to do something.**

**For example when you want to look at every value in a list**

```python
for i in range(...):
  do_something()
```

```python
# Do something 10 times:
for i in range(10):
  print(i)
```

```python
# Loop over all indexes in a list:
lst = [1, 2, 3]

for i in range(len(lst)):
  if lst[i] > 2:
    lst[i] = 2            # Replaces any value > 2 in the lst with the value 2
```

```python
# Loop over all values in a list (without the index):
lst = [1, 2, 3]

for value in lst:
  print(value)            # Prints all values in the list
```

## While Loops

**Use while loops when you are not sure how many times to do something**

**In other words, to do something until something is not true**

```python
while bool_expression:
  do_something()
```

```python
x = 10

while x < 100:
  x += 10       # Adds 10 to x until x is >= 100
```

## Function Definition

```python
def my_func(param_one, param_two):
  result = 0
  
  do_stuff_to_compute_result()
  
  return result
```

**Remember that variables defined within a function, including its parameters, only exist within that function**

## Calling a Function

```python
the_result = my_func(3, 100)
```

**If the function returns something, you have to save the return value into a variable**

**If it does not return something, you can just call it without saving the result:**

```python
my_other_func('hello', [1, 3, 7])
```

Also remember, **when naming functions or variables**, the name **has to start with a letter**, and then **must only
contain of letters, numbers, and underscores**.
