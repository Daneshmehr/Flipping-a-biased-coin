# Project-2
Project 1 had a simply fixed values.
For example, given two integers N and R. The task was to calculate the probability of getting exactly r heads in n successive tosses. 
A fair coin has an equal probability of landing a head or a tail on each toss.
The probability of getting K heads in N coin tosses can be calculated using the below formula of binomial distribution of probability: 
[^{n}C_{k} * p^{k} * q^{n-k}]   where p = probability of getting head and q = probability of getting tail. p and q both are 1/2. So the equation becomes
[\frac{1}{2^n} * \frac{n!}{ r! * (n-r)!}]  

# Python3 program to find probability of getting K heads in N coin tosses
 
# Function to calculate factorial
def fact(n):
     
    res = 1
    for i in range(2, n + 1):
        res = res * i
    return res
 
# Applying the formula
def count_heads(n, r):
     
    output = fact(n) / (fact(r) * fact(n - r))
    output = output / (pow(2, n))
    return output
 
# Driver code
n = 4
r = 3
 
# Call count_heads with n and r
print (count_heads(n, r))

For project 2, the binomial distribution with parameters n and p is the discrete probability distribution of the number of successes in a sequence of n independent experiments. It takes different values in coin tosses which it has not simply fixed values.
We know form Bayesian statistics, Posterior = Likelihood × Prior ÷ Evidence.

Python 3 computes analytical expression for the posterior in our experiment (coin tosses).

Python3 computes it and plot the results.
