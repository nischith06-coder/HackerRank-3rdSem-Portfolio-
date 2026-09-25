# Sparse Arrays

## Problem Description

Given a collection of strings and a set of query strings, determine how many times each query string occurs in the original collection.

For every query, return its frequency.

## Approach

We use a hash map to store the frequency of every string.

### Step 1

Traverse all strings and store their frequencies:

```text
frequency[string]++