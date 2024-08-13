# Recursive Factorial Calculation in Python

This project demonstrates the use of a recursive function to calculate the factorial of a number and applies it to a dataset.

## Code

```python
def factorial(n):
    # Base case: when n is 0 or 1
    if n == 0 or n == 1:
        return 1
    else:
        # Recursive case: n * factorial of (n-1)
        return n * factorial(n - 1)

# Example usage:
n = 5
print(f"The factorial of {n} is {factorial(n)}")

# Applying the algorithm to a dataset
dataset = [3, 5, 7, 10]
factorials = []

for number in dataset:
    result = factorial(number)
    factorials.append(result)
    print(f"Factorial of {number} is {result}")

print("Factorials for the dataset:", factorials)
