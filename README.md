simplega
========

This is the simplest (but not shortest) genetic algorithm implementation I can think of. It is a bit
verbose but that is to make it clear what is going on. The problem
that we are trying to solve is the "onemax" problem. Basically our
individuals consist of ones and zeros and we are trying to find an
individual consisting entirely of ones.

this is what a random individual looks like:
[0,0,0,1,1,0,1,0,1,1,1,0,0,0,0,0,1,0,0]
you compute the fitness by summing the ones, the individual above has
a fitness of 7 as it has 7 ones in it.

and this is what we are looking for:
[1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1]

There are 5 parts to a Genetic algorithm:
1: initialisation (create the first generation of random guesses)
2: evaluation (assign a fitness value to the individuals)
3: selection (stochastically select the best individuals from the population)
4: mutation (flip a bit in the individual with a certain probability)
5: crossover (split two good individuals in half and recombine them)

repeat steps 2 to 5 until you get the answer. simple as.
