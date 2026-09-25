# Time Conversion

## Problem Description

Given a time in 12-hour AM/PM format, convert it into 24-hour military time format.

For example:

12:01:00PM → 12:01:00

12:01:00AM → 00:01:00

## Approach

We examine the AM/PM portion of the given time and modify the hour accordingly.

### PM Case

- If the time is PM and the hour is not 12, add 12 to the hour.
- If the hour is already 12 PM, keep it as 12.

### AM Case

- If the time is AM and the hour is 12, change the hour to 00.
- Otherwise, keep the hour unchanged.

The minutes and seconds remain unchanged.

## Complexity Analysis

- **Time Complexity:** O(1)
- **Space Complexity:** O(1)

## Language

C++

## HackerRank

Problem: Time Conversion

Status: Accepted