# Problem: Ignore Negativity

Write a program where the user first inputs an integer `n`, representing the number of inputs they will provide. The program will then take `n` numbers as input, which may include both positive and negative values. However, the catch is that the program should treat negative numbers as positive when determining the highest and lowest values. For example, `-69` should be considered as `69` when comparing with other values.

## Input

- First, an integer `n` (number of inputs).
- Then, `n` integers, which may include negative numbers.

## Output

The highest and lowest values, ignoring the negativity.

## Example

**Input:**

```text
5
10 -20 -30 -40 15
```

**Output:**

```text
Highest: 40
Lowest: 10
```

Make sure that the program can handle cases where all numbers are negative or mixed.