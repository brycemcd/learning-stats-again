# Distributions

+ [Normal](#normal)

+ [Geometric](#geometric)
  + [Bernoulli](#geom-bernoulli)
  
+ [Binomial](#binomial)

+ [Negative Binomial](#negative-biomial)

+ [Poisson](#poisson)

## Normal Distribution

By far the most referenced and most recognizable distribution.

Requires a normal distribution (TODO: tests for normality)

Standardized with a Z score for comparison of data with different means and standard deviations. Expressed as

![definition of Z statistic](http://www.sciweavers.org/tex2img.php?eq=Z%20%3D%20%5Cfrac%7B%28%20x%20-%20%5Cmu%20%29%7D%7B%20%5Csigma%20%20%7D&bc=White&fc=Black&im=png&fs=12&ff=arev&edit=0)

![mu = mean](http://www.sciweavers.org/tex2img.php?eq=%20%5Cmu%20%3D%20mean&bc=White&fc=Black&im=jpg&fs=12&ff=arev&edit=0)

![Standard Deviation](http://www.sciweavers.org/tex2img.php?eq=%20%5Csigma%20%3D%20Standard%20Deviation&bc=White&fc=Black&im=png&fs=12&ff=arev&edit=0)

### Is a data sample normal?

TODO: tests of normality

#### Histogram

Visually, inspect a histogram and decide if it "looks" normal. 

#### Q-Q plot

[A Q-Q graph](http://en.wikipedia.org/wiki/Q%E2%80%93Q_plot) displays a plot of two distributions for comparison. For a normal distribution, 
the data will fall along the x=y line. The data will be concentrated in the middle of the graph with few points falling outside the x=y line.

### Bell Curve

A rule of thumb for normal distributions:

+ 68% of observations fall within one standard deviation of the mean
+ 95% of observations fall within two standard deviations of the mean
+ 99.7% of observations fall within three standard deviations of the mean
