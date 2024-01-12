# Big O Chart

## Examples of Complexities

### Constant Time: O(1)

```python
def get_first_element(lst):
    return lst[0]

# No matter how large the list is, the time complexity is constant.

```
### Linear Time: O(n)

```python
def print_elements(lst):
    for element in lst:
        print(element)

# The time complexity grows linearly with the size of the list.

```

### Logarithmic Time: O(n log n)

```python
def binary_search(lst, target):
    low, high = 0, len(lst) - 1

    while low <= high:
        mid = (low + high) // 2
        if lst[mid] == target:
            return mid
        elif lst[mid] < target:
            low = mid + 1
        else:
            high = mid - 1

# Binary search divides the search space in half, resulting in logarithmic time.
```

### Quadratic Time: O(n^2)

```python
def print_pairs(lst):
    for i in range(len(lst)):
        for j in range(len(lst)):
            print(lst[i], lst[j])

# Nested loops result in quadratic time complexity.
```

### Exponential Time: O(2^n)
```python
def fibonacci_recursive(n):
    if n <= 1:
        return n
    else:
        return fibonacci_recursive(n-1) + fibonacci_recursive(n-2)

# The recursive Fibonacci algorithm has exponential time complexity.

```
### Factorial Time: O(n!)

```python
def factorial_recursive(n):
    if n == 0 or n == 1:
        return 1
    else:
        return n * factorial_recursive(n-1)

# The recursive factorial function has factorial time complexity.
```
