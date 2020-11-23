# Solution

## Summary  

We are given  

ABCD * E = DCBA  

## Fix number E  

It's a good idea to try to solve the problem with a fixed number E first.  

## Try to solve (A, B, C, D)  

We try E = 4:  
    D * E % 10 = A  
    A * E < 10 (at least)  
    A > 0, D > 0 (first digits)  
We try all values for D  
D | 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 | 9  
A | 4 | 8 | 2 | 6 | 0 | 4 | 8 | 2 | 6  

We have A * E < 10, so A < 10 / E = 2.5 => A = 1 or A = 2  
From the table, we can see (A, D) = (2, 3) or (A, D) = (2, 8)  

Let's try with (A, D) = (2, 8):  
    A * E = D (2 * 4 = 8), so there should not be any number added from the calculation of less significant digits(1)  
    D * E = 32 => 3 will be added to C * E  
    We then have:  
        (C * E + 3) % 10 = B   
        (B * E + (C * E + 3) / 10) = C (due to (1))  
Similarly, we then try all values for C  
C | 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 | 9  
B | 7 | 1 | 5 | 9 | 3 | 7 | 1 | 5 | 9  

From the table, there is a pair (B, C) = (1, 7) satisfy our requirements (1).  

## Final Answer  

As a result, we have found a solution: (A, B, C, D, E) = (2, 1, 7, 8, 4).

