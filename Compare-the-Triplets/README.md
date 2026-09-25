# Compare the Triplets

## Problem Description

Alice and Bob each have three scores.

For each corresponding score:

- If Alice's score is greater, Alice receives 1 point.
- If Bob's score is greater, Bob receives 1 point.
- If both scores are equal, nobody receives a point.

Return the final scores of Alice and Bob.

## Approach

Store Alice's and Bob's three scores in arrays.

Compare the corresponding elements one by one:

- `a[i] > b[i]` → increment Alice's score.
- `a[i] < b[i]` → increment Bob's score.
- Otherwise → no score is added.

Finally, return the two scores.

## Complexity Analysis

- **Time Complexity:** O(1)
- **Space Complexity:** O(1)

Since there are always exactly three scores, the number of operations remains constant.

## Language

C++

## HackerRank

Problem: Compare the Triplets

Status: Accepted