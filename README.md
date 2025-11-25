# LeetCode-problems
My notes while solving leetcode problems
## Two Sum - Array - Easy (LC No. 1)

### Problem:

Find the index of two number adding to a target in a list.

### Things I learnt:

Use hash maps to avoid nested loops.
Using nested loops → O(n^2).

Using one loop and hash map → O(n) + O(1), with extra space.

### Pattern to remember:

When you need to find a pair/match in an array and you’re using nested loops, ask, can I store what I have seen and check in O(1).

Calculate what you’ve need and check if it’s been seen before.

## Longest Common Prefix - Arrays, Strings - Easy (LC No. 14)

### Problem:

Find the longest common prefix among words in an array.

### Things to note

1. Sometimes nested loops are unavoidable.
2. In that case try to reduce the number of iterations by finding shortest length to loop on.

## Remove duplicate from sorted array - Array - Easy (LC No. 26)

### Similar Problems

- Remove Element (LC No. 27)

### Problem

From an int array, sorted in non-decreasing order, return the number of unique elements, ‘k’, using in place operations.

### Things I learnt

- Two pointers approach
- Fast, slow approach. Slow Writes, Fast Reads.

### Pattern

When you see “in-place array modification” with filtering & array is sorted think about two pointers.

Don’t use when you have to preserve the original array.

## Majority Element - Array - Easy (LC No. 169)

### Problem

Find the the majority element in an int array. Majority element → occurs more than half. Guarantees there is a majority element. Find in O(n) time and O(1) space.

### Things I learnt

- Moore’s Algorithm → Uses O(1), optimizing space. Instead of storing a hash map which in worst case will store n elements. This algo uses only two variable, one for tracking element and one for count. Works like this; when count = 0, current_element =element, if a element repeats, increase the count, if the element is different, reduce the count.

### Pattern

1. Used when finding majority element, and it is guaranteed.
2. An alternative to using hash maps.
3. Used when space is critical
4. Only finds the majority element, not the frequency. Also won’t work if want multiple elements for output.
