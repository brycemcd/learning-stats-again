# Test Statistics

+ [Z](#z)
+ [T](#t)
+ [Anova](#anova)

## Z

## T

The T statistic is describes the area under the t distribution curve at
a given point with a described degrees of freedom. It's very much like
the Z score with the exception that it should be used when sample sizes
are small.

### One sample

![t statistic](https://s3-us-west-2.amazonaws.com/bryce-statistics/stats-equations/one_sample_t_test.png)

### Two Sample

![standard error](https://s3-us-west-2.amazonaws.com/bryce-statistics/stats-equations/standard_error_for_difference_of_two_means.png)

## ANOVA
### or F statistic

ANOVA = analysis of variance

Used to test if many means are equal. Often:

`H0 = the mean outcome is the same across many groups`
`Ha = the mean in at least one group is different than the rest`

It's possible to conclude that one mean in a group is different than the
rest and then run pairwise tests on each permutation of groups to find
there is no statistically different difference in any pairs. ANOVA
concludes that not all means are equal, not which means are different.

Assumptions:

+ Observations are independent within and across groups
+ data within each group are close to normal (a Q-Q plot can visually
  inspect this)
+ variability across groups is approximately the same (boxplots can
  visually inspect this)
