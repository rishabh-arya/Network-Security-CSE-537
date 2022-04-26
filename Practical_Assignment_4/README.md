## PRNG - 1 : Linear Congruential Generator 

This method is a class of Pseudo Random Number Generator (PRNG) algorithms used for generating sequences of random-like numbers in a specific range. This method can be defined as: 

X_new = (a*X_prev + c ) mod m

where, X, is the sequence of pseudo-random numbers
m, ( > 0) the modulus
a, (0, m) the multiplier
c, (0, m) the increment
X0,  [0, m) – Initial value of sequence known as seed

m, a, c, and X0 should be chosen appropriately to get a period almost equal to m.  
