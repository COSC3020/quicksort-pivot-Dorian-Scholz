# Quicksort Pivots

in the lectures I only briefly mentioned strategies for determining a good pivot
for quicksort. The implementation on the slides simply picks the leftmost
element in the part of the array that we consider as a pivot. I also mentioned a
few other ways of picking a good pivot, e.g. randomly.

Median-of-three is also a good way of picking a pivot -- inspect the first,
middle, and last elements of the part of the array under consideration and
choose the median value. Using the probabilities for picking a pivot in a
particular part of the array (in the same way as we did on slide 34), argue
whether this method is more or less (or equally) likely to pick a good pivot
compared to simply choosing the first element. Assume that all permutations are
equally likely, i.e. the input array is ordered randomly.

Your answer must derive probabilities for choosing a good pivot and
quantitatively reason with them.

Add your answer to this markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

Answer: 

The median of three method for pivot selection in Quicksort examines the first, middle, and last elements of the current array segment and chooses the median value as the pivot. This approach increases the chances of picking a pivot closer to the center of the sorted order, which is more likely to create balanced partitions compared to simply choosing the first element. Since the input array is assumed to be random, selecting the first element as the pivot has an equal probability of being anywhere in the sorted array, making the likelihood of a good pivot around 1/3. In contrast, the median-of-three method reduces the chances of picking extreme values (smallest or largest) and improves the probability of a good pivot to approximately 5/9. This makes the median-of-three method more effective at maintaining balanced partitions and improving Quicksort’s performance.
