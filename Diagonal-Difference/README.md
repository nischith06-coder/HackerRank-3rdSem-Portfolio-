# Diagonal Difference

## Problem Description

Given a square matrix, calculate the absolute difference between the sums of its primary diagonal and secondary diagonal.

### Example

For the matrix:

1 2 3
4 5 6
9 8 9

Primary diagonal:
1 + 5 + 9 = 15

Secondary diagonal:
3 + 5 + 9 = 17

Absolute difference:
|15 - 17| = 2

## Approach

We traverse the matrix only once.

- The primary diagonal contains elements where `row == column`.
- The secondary diagonal contains elements where `row + column == n - 1`.
- Add the elements of both diagonals while traversing the matrix.
- Return the absolute difference between the two sums.

## Complexity Analysis

- **Time Complexity:** O(N)
- **Space Complexity:** O(1)

## Language

C++

## HackerRank

Problem: Diagonal Difference

Status: Accepted