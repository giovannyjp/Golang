# algorithmTesting
Go lang research 
by: Giovanny Pacheco


Bubble sort works by walking through a list of numbers and comparing each consecutive pair of numbers. When we compare the numbers we will ask "is the first number greater than the second number?" and if the answer is yes, we swap the position of each number in the pair.

Regardless of whether or not we swap the numbers, we then move on to the next consecutive pair in the list and repeat the comparison and potential swap steps.

Walking through an example of comparing and swapping items
This is much clearer with an example, so lets go back to the original example of 5, 4, 2, 3, 1, 0.

Our bubble sort algorithm can be broken into roughly two pieces. Walking through the list comparing consecutive pairs of numbers. Every time we do a full pass of the list we will look at N - 1 pairs of numbers.

The second part is repeating this walk-through of the list. As we discussed early, in the worst case we would need to repeat this N times, so we end up doing N - 1 comparisons N times, giving us N * (N - 1).

In Big-O we drop the constants, so we get the complexity of O(N*N) or O(N^2). This means that as the size of our list grows, the number of operations we need to sort the list grows exponentially.
