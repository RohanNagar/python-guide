# Input

You can get user input from the keyboard in python with the `input()` function. The `input()` function always provides a string
of whatever the user entered.

It is the programmer's responsibility to convert that string into the type that is needed. Remember, you can easily convert between
types! See [03 Types](./03-types.md)

## Quick Reference

```python
# Ask the user to "Enter some text: " and store that string in a variable
user_entered_string = input('Enter some text: ')

# Ask the user to "Enter an integer: ", convert the provided string into an integer, and store it in a variable
user_entered_string = input('Enter an integer: ')
user_entered_integer = int(user_entered_string)

# OR, a better way without an extra variable:

user_entered_integer = int(input('Enter an integer: '))

# Ask the user to "Enter a decimal: ", convert the provided string into a float, and store it in a variable
user_entered_num = float(input('Enter a decimal: '))
```
