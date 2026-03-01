CSE 317: Design and Analysis of Algorithms
Homework 2. Due Date: 11:50pm, March 4, 2026.
Submission instructions will be shared on LMS.
All questions carry equal marks.
1. Consider a triangular array of integers with n rows, where the i-th row contains exactly i
positive numbers. Starting from the top element, you move downward row by row. At each
step, if you are at position j in row i, you may move to either position j or j + 1 in row
i + 1 (i.e., to one of the two adjacent entries directly below). Your task is to determine a
path from the top to the bottom such that the sum of the selected numbers is maximized.
For example, in the triangle, he maximum path sum is 23 given by the path of numbers
shown in red, i.e. 3 + 7 + 4 + 9 = 23.
3
7
4
2
4
6
8
5
9
3
Note that there are a total of 2n−1 paths (where n is the number of rows in the triangle)
from the top to the bottom of the triangle. It is not feasible to find the maximum sum using
brute force when n is large. Devise a dynamic programming solution to find the maximum
possible sum and analyze the running time of your solution.
2. Consider a set of coin denominations C = {c1, c2, . . . , cn} where each ci is a positive integer.
Assume that each coin denomination can be used an unlimited number of times. Given a
target value V , we wish to determine the minimum number of coins required to make the
value exactly equal to V . For example, if C = 1, 3, 4 and V = 6, then the minimum number
of coins required is 2, obtained by selecting coins 3 + 3 = 6.
Note that there may be multiple ways to form the value V . In general, the number of
possible combinations grows exponentially as V increases. Therefore, it is not feasible to
enumerate all possibilities when V is large.
Devise a dynamic programming algorithm to determine the minimum number of coins
required to form the value V , and analyze the running time complexity of your solution.
If it is not possible to form V using the given denominations, your algorithm should report
that no solution exists.
3. Consider five matrices of following sizes, respectively:
M1 : 1 × 5,
M2 : 5 × 2,
M3 : 2 × 3,
M4 : 3 × 9,
M5 : 9 × 4.
Using dynamic programming algorithm find the minimum number of scalar multiplications
required to compute the product Q5
j=1 Mj as well as an optimal parenthesization.
4. Find the edit distance between the following two strings s1 and s2 using dynamic program-
ming algorithm: s1 =INTENTION and s2 =EXECUTION.
5. Design a dynamic programming algorithm to test whether a given sequence S = ⟨s1, . . . , sn⟩
over some alphabet Σ of length n contains a palindromic subsequence.
A subsequence ⟨si1, si2, . . . , sik⟩of length k is called palindromic if si1 = sik, si2 = sik−1,
and so on. For example, ⟨1, 2, 3, 2, 1⟩is a palindromic subsequence of S = ⟨1, 2, 3, 4, 2, 1⟩.
Your algorithm should return the length of a longest palindromic subsequence in S. Also
analyze time complexity of your algorithm and show that it runs in O(n2) time and use
O(n2) space.
6. Given two sequences x = ⟨x1, . . . , xm⟩and y = ⟨y1, . . . , yn⟩over some alphabet Σ of lengths
m and n, respectively. A sequence z is called a common supersequence of x and y if both
x and y are subsequences of z.
For example, the shortest common supersequence of x = ⟨1, 2, 2, 3⟩and y = ⟨2, 3, 2⟩is the
sequence z = ⟨1, 2, 2, 3, 2⟩as both x and y are subsequences of z.
Design a dynamic programming algorithm to find the length of a shortest common super-
sequence of x and y using a dynamic programming algorithm. Also analyze time and space
complexity of your algorithm.
7. For a sequence X
=
⟨x1, x2, . . . , xn⟩, we define the mirror of X as the sequence
Y = ⟨xn, xn−1, . . . , x1⟩. We say that a sequence X is beautiful if the mirror of X is the
same as X. Design an O(n2) dynamic programming algorithm that finds the minimum
number of elements to add to a given sequence X to turn it into a beautiful sequence. [We
can add new elements anywhere in the sequence.]
8. Given a set of nonnegative integers S and a target integer t, design a dynamic programming
algorithm to find a subset of S whose sum is equal to t.
Also analyze time and space
complexity of your algorithm.
Page 2
