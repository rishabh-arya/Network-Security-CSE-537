## PRNG - 1 : Linear Congruential Generator 

This method is a class of Pseudo Random Number Generator (PRNG) algorithms used for generating sequences of random-like numbers in a specific range. This method can be defined as: 

X_new = (a*X_prev + c ) mod m

where, 

       X, is the sequence of pseudo-random numbers
       m, ( > 0) the modulus
       a, (0, m) the multiplier
       c, (0, m) the increment
       X0,  [0, m) – Initial value of sequence known as seed

       m, a, c, and X0 should be chosen appropriately to get a period almost equal to m.  

### Approach: 

- Choose the seed value X0, Modulus parameter m, Multiplier term a, and increment term c.
- Initialize the required amount of random numbers to generate (say, an integer variable noOfRandomNums).
- Define a storage to keep the generated random numbers (here, vector is considered) of size noOfRandomNums.
- Initialize the 0th index of the vector with the seed value.
- For rest of the indexes follow the Linear Congruential Method to generate the random numbers.

       randomNums[i] = ((randomNums[i – 1] * a) + c) % m 

- Finally, return the random numbers.



## PRNG - 2 : Mersenne Twister 

The Mersenne Twister is a general-purpose pseudorandom number generator (PRNG) developed in 1997 by Makoto Matsumoto [ja] and Takuji Nishimura . Its name derives from the fact that its period length is chosen to be a Mersenne prime.
The Mersenne Twister was designed specifically to rectify most of the flaws found in older PRNGs.
The most commonly used version of the Mersenne Twister algorithm is based on the Mersenne prime 219937 – 1. The standard implementation of that, MT19937, uses a 32-bit word length. There is another implementation (with five variants) that uses a 64-bit word length, it generates a different sequence.
