#### Please add your answers to the ***Analysis of  Algorithms*** exercises here.

## Exercise I

a) This algorithm runs in `O(n)` time. This is because the first operation is n^3  and we are building up to n^3 by performing n^2 operations which means we are dividing n^3 by n^2 which is `(n^ (3 - 2)) = n`


b) We are starting at n and increasing the comparitor j by 2 each time until it reaches n. Technically this means that it would run `O(.5n)` time but we can drop the 0.5, so this runs in `O(n)` time.


c) This is a recursive algorithm that is testing to run down to 0 from bunnies or `n` and subtracting one at a time while adding 2 to it each time. This is effetive `O(n)` runtime in order to get from bunnies (n) to 0;

## Exercise II

In order to minimize the number of drops that take place, we want to minimize the number of "search" operations that we're doing for the value of the floor `(f)`. We can assume that the floors are already sorted from lowest to highest (as most buildings are), so we can attempt a binary search algorithm to find the floor. Start at the middle floor and if the egg breaks at that floor move to the bottom 1/2 of floors below that middle floor and go to the middle floor. If the egg doesn't break at that point, then move to the top 1/2 of floors left between the first middle and second middle. Keep performing this operation until you find the floor at which the egg doesn't break. This would run in O(log(n)) time. 


