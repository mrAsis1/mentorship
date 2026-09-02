# Problem: Abundant Number Checker

Write a C program that determines whether a given positive integer is an abundant number or not. An abundant number is a positive integer for which the sum of its proper divisors (excluding the number itself) is greater than the number.

Your program should:

- Accept a positive integer as input from the user.

## Sample Input and Output

**Input 1:** `Enter a positive integer: 12`

**Output 1:** `12 is an abundant number.`

**Input 2:** `Enter a positive integer: 10`

**Output 2:** `10 is not an abundant number.`

**Input 3:** `Enter a positive integer: 18`

**Output 3:** `18 is an abundant number.`

## Explanation

- For 12, the proper divisors are 1, 2, 3, 4, and 6. Their sum is 16, which is greater than 12.
- For 10, the proper divisors are 1, 2, and 5. Their sum is 8, which is not greater than 10.
- For 18, the proper divisors are 1, 2, 3, 6, and 9. Their sum is 21, which is greater than 18.