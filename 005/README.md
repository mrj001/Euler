# Problem number 5
This code finds the minimum set of prime factors of the least common multiple of 1..20.
For each number in the range of 2 through 20
   Try to divide each larger number.
   If it divides even replace the larger number with the quotient.
Multiply all the remaining numbers together.

This runs in about half a second on the C64.

Contrast this with a brute force approach:
  candidate = 2520
  try to divide by all numbers in the range 2..20
  If all succeed, this is the answer.
  Otherwise, add one and try again.

The brute force approach took about 5.5 seconds on a 3GHz 4th Generation i7.

I think this nicely illustrates that the choice of algorithm is the most important factor in performance.

