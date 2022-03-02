# If Statements

If statements are very important when writing code! In order for your program to behave differently based
on input or some information, you need to use if statements. They look like this:

```python
if something_is_true:
  do_something()
elif something_else_is_true:
  do_something_else()
else:
  do_a_different_thing()
```

You can almost read it like english. Think of it translating like this:

```python
if "this thing is true",
  then do all of the code here.
else if that was not true, but "this other thing is true",
  then do all of the code here.
else if none of the above were true,
  then do all of the code here.
```

## Examples

1. Write a program that asks the user to enter an integer and prints if it is positive, negative, or zero.

Based on this problem, we want to do something different in our program based on what the user enters. Let's see how to do it:

```python
# Get the input
user_val = int(input('Enter a number: '))

if user_val > 0:
  # If the number is greater than zero, print that is it positive
  print(f'The number {user_val} is positive!')
elif user_val < 0:
  # Else if it was not greater than zero, but it is less than zero, print that is is negative
  print(f'The number {user_val} is negative!')
else:
  # Else we know that it was not greater than zero or less than zero, so it must be zero
  print(f'The number {user_val} is zero!')
```

2. Write a program that asks the user to enter an interger and prints if the number is even or odd

```python
# Get the input
user_val = int(input('Enter a number: '))

if user_val % 2 == 0:
  # If dividing by 2 gives no remainder, then it is even
  print(f'The number {user_val} is even!')
else:
  # Else the number is not even, so it is odd
  print(f'The number {user_val} is odd!')
```

3. Write a program that asks the user to enter an interger and prints 'YES' if the number is even and greater than 100. Otherwise it prints 'NO'

```python
# Get the input
user_val = int(input('Enter a number: '))

# Notice how we can use "and" to make sure more than one thing is true
if user_val % 2 == 0 and user_val > 100:
  print('YES')
else:
  print('NO')
```

4. Write a program that asks the user to enter an interger and prints 'YES' if the number is even OR less than 100. Otherwise it prints 'NO'

```python
# Get the input
user_val = int(input('Enter a number: '))

# Notice how we can use "or" to run code if either of two things are true
if user_val % 2 == 0 or user_val > 100:
  print('YES')
else:
  print('NO')
```
