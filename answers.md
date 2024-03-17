# CMPS 2200 Reciation 5
## Answers

**Name:**Ivo Tomasovich


Place all written answers from `recitation-05.md` here for easier grading.







- **1b.**
For Quicksort fixed and random, the asymptotic bound O(nlogn) on average case. The runtimes are as expected with this upperbound, and the runtimes increase proportionally with the size of the input list.

For selection sort, the asymptotic upper bound is n^2 in all cases. The running time alligns with this, and it also significantly increases with larger lists.

Quicksort tends to be quicker on random permutation compared to random ones, as we see when we use the print function to get a list of the values. The difference is especially noticable at larger list sizes. For selection sort, the performance remains pretty constant, but that constant is quite slow, since it always iterates through the entire list. Overall, changing the type of inputs list affects the performance of quicksoft much more than selection sort.

- **1c.**
With the fastest one being random pivot, its actually barely faster than timsort, but the difference
is negligible even on higer inputs:

|        |         |       n |   timsort           |   qsort-random-pivot |
|--------|---------|---------|---------------------|----------------------|
|    100 |   0.218 |   0.276 |               0.009 |                0.005 |
|    200 |   0.430 |   0.492 |               0.015 |                0.011 |
|    500 |   1.049 |   1.225 |               0.055 |                0.036 |
|   1000 |   2.327 |   2.590 |               0.084 |                0.076 |
|   2000 |   4.205 |   4.870 |               0.164 |                0.159 |
|   5000 |  11.227 |  12.522 |               0.440 |                0.429 |
|  10000 |  23.155 |  25.002 |               0.967 |                0.927 |
|  20000 |  49.019 |  53.122 |               2.081 |                2.020 |
|  50000 | 127.537 | 140.184 |               5.867 |                5.780 |
| 100000 | 273.341 | 311.143 |              12.497 |               12.437 |