# Dynamic Array

## Problem Description

Given a sequence of queries, maintain a collection of dynamic sequences and process two types of queries.

The problem uses the last answer to determine which sequence should be accessed.

For a Type 1 query:
- Calculate the sequence index using XOR.
- Append the given value to that sequence.

For a Type 2 query:
- Calculate the sequence index using XOR.
- Access an element from that sequence.
- Update `lastAnswer`.

## Approach

We use a vector of vectors to represent the dynamic sequences.

For each query:

### Type 1

The sequence index is calculated as:

`idx = (x ^ lastAnswer) % n`

Then the value `y` is appended to that sequence.

### Type 2

Again calculate:

`idx = (x ^ lastAnswer) % n`

Then access:

`seq[idx][y % seq[idx].size()]`

The retrieved value becomes the new `lastAnswer`.

## Complexity Analysis

- **Time Complexity:** O(N + Q) overall
- **Space Complexity:** O(N)

## Data Structure Used

- Vector
- Vector of vectors
- Bitwise XOR

## Language

C++

## HackerRank

Problem: Dynamic Array

Status: Accepted