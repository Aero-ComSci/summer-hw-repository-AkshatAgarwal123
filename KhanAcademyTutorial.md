# Recursive Factorial Calculation in Python

This project demonstrates the use of a recursive function to calculate the factorial of a number and applies it to a dataset.

## Step 1: Understanding Recursion

Recursion is a technique where a function calls itself to solve smaller instances of the same problem until it reaches a base case. In the factorial problem, `n!` (n factorial) is defined as:
```sh
n! = n  × (n−1) × (n−2) × ... × 1
```

The recursive definition of the factorial is:
```sh
factorial(n)= { 1                 if n=0 }
              { n×factorial(n-1)  if n>0 }
```

## Step 2: Implementing the Recursive Algorithm in Python
Here is the Python code for a recursive function to calculate the factorial of a number:
```sh
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
```

## Step 3: Applying the Algorithm to a Dataset
Let's say you have a dataset of integers, and you want to calculate the factorial for each number in the dataset.
```sh
dataset = [3, 5, 7, 10]
factorials = []

for number in dataset:
    result = factorial(number)
    factorials.append(result)
    print(f"Factorial of {number} is {result}")

print("Factorials for the dataset:", factorials)
```

## Step 4: Reflecting on the Activity

What I Learned:

From this activity, I learned the power of recursion in solving problems that can be broken down into smaller, similar problems. The factorial example shows how recursion simplifies the process of handling repeated multiplication. However, I also learned that recursion, while elegant, can lead to issues such as stack overflow if not properly handled with a base case. Furthermore, applying recursion to a dataset demonstrates how algorithms can be scaled to handle multiple data points effectively.
