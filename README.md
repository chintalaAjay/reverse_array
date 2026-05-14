# Reverse an Array - Java Solution

This repository contains my Java solution for the **Reverse an Array** problem from GeeksforGeeks.

---

## Problem Link

https://www.geeksforgeeks.org/problems/reverse-an-array/1

---

## Problem Statement

Given an array `arr[]`, reverse the array in-place.

The task is to reverse the elements of the array without using any extra array.

---

## Example

### Input

```text
[1, 4, 3, 2, 6, 5]
```

### Output

```text
[5, 6, 2, 3, 4, 1]
```

---

## Approach

### Two Pointer Technique

This solution uses the **Two Pointer Technique**.

- One pointer (`start`) begins from the start of the array.
- Another pointer (`end`) begins from the end of the array.
- Swap both elements.
- Move `start` forward and `end` backward.
- Repeat until both pointers meet.

This efficiently reverses the array in-place.

---

## Java Solution

```java
class Solution {
    public void reverseArray(int arr[]) {

        int start = 0;
        int end = arr.length - 1;

        while (start < end) {

            int temp = arr[start];
            arr[start] = arr[end];
            arr[end] = temp;

            start++;
            end--;
        }
    }
}
```

---

## Time Complexity

```text
O(n)
```

The array is traversed only once.

---

## Space Complexity

```text
O(1)
```

No extra space is used.

---

## Concepts Used

- Arrays
- Two Pointer Technique
- Swapping
- In-place Array Reversal

---

## Learning Outcome

Through this problem, I learned:

- Efficient array reversal
- How two pointers work
- In-place array manipulation
- Optimizing time and space complexity

---

## Author

Ajay Chintala

---

## GitHub Profile

https://github.com/chintalaAjay
