# 2769. Find the Maximum Achievable Number

LeetCode: https://leetcode.com/problems/find-the-maximum-achievable-number/

## Tags

Math, Simulation

## Question

You are given two integers, num and t. Return the maximum possible value after performing exactly t operations.

## My approach

I used a mathematical observation instead of simulating every operation. In one operation, the distance between the current value and num can increase by 2: one value moves up by 1 while the other moves down by 1. Therefore, after t operations, the maximum achievable value is:

    num + 2 * t

This directly produces the answer.

## Technique

- Mathematical observation
- Direct formula
- No loops or extra memory required

## Complexity

- Time: O(1)
- Space: O(1)

## C

    int theMaximumAchievableX(int num, int t) {
        return num + 2 * t;
    }

## C++

    class Solution {
    public:
        int theMaximumAchievableX(int num, int t) {
            return num + 2 * t;
        }
    };

## Python

    class Solution:
        def theMaximumAchievableX(self, num: int, t: int) -> int:
            return num + 2 * t
