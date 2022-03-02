# For Loops and Range

## Quick Reference

```python
# For loops usually use the range function, which looks like this:
range(start, end, step)
```

```python
# Print every integer from 1 to 20 (inclusive)
for i in range(1, 20 + 1):
  print(i)
  
# Print every integer from 0 to 100 (inclusive)
for j in range(0, 100 + 1):
  print(j)

# Print all integers from 0 to 100 (inclusive) that are steps of 5
for num in range(0, 100 + 1, 5):
  print(num)

# Nested for loops - for each number from 1 to 10, print Hello that many times
# on the same line. Then, start a new line.
for i in range(1, 10 + 1):
  for k in range(i):
    print('Hello', end=' ')
    
  print()
```
