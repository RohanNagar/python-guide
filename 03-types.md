# Data Types

All variables in python have a data type. These are some of the common data types:

- int
- float
- bool
- str
- NoneType

You can figure out the type of something using the `type()` function. For example:

```python
# Prints: <class 'str'>
my_string = 'Hello'
print(type(my_string))

# Prints: <class 'int'>
my_num = 100
print(type(my_num))

# Prints: <class 'float'>
my_num_with_decimal = 32.5
print(type(my_num_with_decimal))

# Prints: <class 'bool'>
my_boolean = True
print(type(my_boolean))
```

Sometimes you need to convert things between different types. For example, maybe you want to add a decimal to an integer.

You can do this by using that type's function. For example:

```python
# To turn an int into a float
my_num = 10
my_float_num = float(my_num)

print(my_float_num) # Prints 10.0

# To turn a string into an integer
my_str = '40'
my_parsed_int = int(my_str)

my_parsed_int = my_parsed_int + 10 # Now you can add since my_parsed_int is the integer 40 instead of a string
print(my_parsed_int) # Prints 50
```

