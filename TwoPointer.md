# Two pointer algorithms

## My understanding

This is basically tracking two individual index or pointers in a given array to solve a problem so that we don't need to brute force our way out.

## From geeks for geeks

Two pointers is really an easy and effective technique that is typically used for searching pairs in a sorted array.

## Example 

Given a sorted array A (sorted in ascending order), having N integers, find if there exists any pair of elements (A[i], A[j]) such that their sum is equal to X.

## Illustration 
```
A[] = {10, 20, 35, 50, 75, 80}
X = 70

i = 0
j = 5

A[i] + A[j] = 10 + 80 = 90
Since A[i] + A[j] > X, j--
i = 0
j = 4

A[i] + A[j] = 10 + 75 = 85
Since A[i] + A[j] > X, j--
i = 0
j = 3

A[i] + A[j] = 10 + 50 = 60
Since A[i] + A[j] < X, i++
i = 1
j = 3
m
A[i] + A[j] = 20 + 50 = 70
```

Thus this signifies that Pair is Found.

## Advantages

This problem could be solved by going through every pair and checking their sum but that has a time complexity of O(n^2)
