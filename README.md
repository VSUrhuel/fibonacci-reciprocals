# Fibonacci Reciprocals
This exercise focuses on implementing functions related to the Fibonacci sequence and its reciprocals.

## Introduction:
The Fibonacci sequence, named after the 12th-century mathematician Leonardo Fibonacci, is a series of numbers characterized by the sum of the two previous integers, with seed values 0 and 1. The sequence starts as follows:
1, 2, 3, 5, 8, 13, 21, 34, 55, 89, 144

In recurrence relation form, it can be expressed as:
𝑓(𝑛) = 𝑓(𝑛 − 1) + 𝑓(𝑛 − 2)

With seed values:
𝑓(0) = 0, 𝑓(1) = 1

The Fibonacci series is so popular that it is used in various algorithms, such as Fibonacci search technique, Fibonacci cubes for distributed systems interconnection, Fibonacci heap, etc.

## Learning Outcomes:
- Implement a function to determine if a natural number is a Fibonacci number or not.
- Implement a function to display the sum of Fibonacci reciprocals within a range of natural numbers.

## Problem Description:
1. `bool isFib(int x);`
   - Determines if `x` is a Fibonacci number using an iterative structure.
   - Return 1 if `x` is a Fibonacci number, 0 otherwise.

2. `void dispFibsInRange(int s, int e);`
   - Displays the list of Fibonacci numbers in the range from `s` to `e`.
   - Uses the `isFib(int x)` function to identify Fibonacci numbers.

3. `void dispFibsReciprocalInRange(int s, int e);`
   - Displays the reciprocals of Fibonacci numbers in the range from `s` to `e`.
   - The reciprocals are displayed in decimal format (real numbers).
   - Uses the `isFib(int x)` function to identify Fibonacci numbers.

4. `double FibsReciprocalSumInRange(int s, int e);`
   - Returns the sum of Fibonacci reciprocals in the range from `s` to `e`.
   - Uses the `isFib(int x)` function to identify Fibonacci numbers.
   
## Usage:
Call all functions from the `main` function, using your preferred parameters, to see the results for different ranges of natural numbers.

```c
#include <stdio.h>

// Function prototypes (definitions are provided in the implementation)
bool isFib(int x);
void dispFibsInRange(int s, int e);
void dispFibsReciprocalInRange(int s, int e);
double FibsReciprocalSumInRange(int s, int e);

int main() {
    // Call the functions with your preferred parameters here.
    dispFibsInRange(1, 10);
    dispFibsReciprocalInRange(1, 10);
    double sum = FibsReciprocalSumInRange(1, 10);
    printf("Sum of Fibonacci reciprocals: %lf\n", sum);

    return 0;
}
```

Feel free to modify the range values in the `main` function to explore the Fibonacci reciprocals for different ranges of natural numbers.

## How to Contribute:
Contributions to this project are welcome! If you have any suggestions, bug fixes, or improvements, please follow these steps:
1. Fork this repository.
2. Create a new branch with a descriptive name.
3. Make your changes and commit them with clear commit messages.
4. Push your changes to your forked repository.
5. Submit a pull request explaining the changes you've made.

## Credits:
This problem was presented as a C++ Lab Exercise by Sir Michael Jay Anthony Regis.
