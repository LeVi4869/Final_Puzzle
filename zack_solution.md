# Zack's Solution

## Solution
ABCD = 2178

## Reasoning
The first thing to do is you need to establish A, D, and E, since they're the most restricted.  

You can observe the following restrictions:
1. A < D
1. A * E &le; D

With that in mind, the only possible values for A, D, and E that fit this is A = 2, D = 8, and E = 4.  

This results in 2BC8 * 4 = 8CB2.  Since 2 * 4 = 8, we know that B*4 &le; 10.  Since A = 2, this means that B = 1.  

To find C, we observe that (3+4C) mod 10 = 1.  Of the possible remaining values for C (5,6,7,9), only 7 fulfills this, resulting in C = 7.

## Comments
I thought this looked somewhat familiar, took me until I figured out the solution (from scratch) to realize this is the same one I went over in class, just replacing the 4 with its own variable.  This actually makes the problem more interesting, I like it!  It also makes sense that this only has 1 unique solution, since the same is true for the 4 * RATS = STAR problem.
