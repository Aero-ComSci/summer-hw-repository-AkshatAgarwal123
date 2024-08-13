# Recursive Factorial Calculation in Python

This project demonstrates the use of a recursive function to calculate the factorial of a number and applies it to a dataset.

## Step 1 Understanding Recursion

Recursion is a technique where a function calls itself to solve smaller instances of the same problem until it reaches a base case. In the factorial problem, `n!` (n factorial) is defined as:
```sh
n!=n×(n−1)×(n−2)×…×1
```

The recursive definition of the factorial is:
```sh
factorial(n)= { 1    if n=0
                n×factorial(n-1)    if n>0             }

​
  
if n=0
if n>0
​


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
