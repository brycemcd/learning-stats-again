# Distributions

+ [Normal](#normal-distribution)

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

## Bernoulli Model

Describes a data set with two possible outcomes described as "success" or "failure." Success does not need to be a good thing. For example, a success in an experiment could be that someone dies of an overdose. The success is that one of the binary outcomes has been identified.

![probability of success](http://www.sciweavers.org/tex2img.php?eq=p%20%3D%20P%28success%29&bc=White&fc=Black&im=png&fs=12&ff=arev&edit=0)

mean = p

![standard deviation](http://www.sciweavers.org/tex2img.php?eq=%5Csigma%20%3D%20%20%5Csqrt%7B%20%5Crho%20%281-%5Crho%29%7D%20&bc=White&fc=Black&im=png&fs=12&ff=arev&edit=0)

## Geometric Distribution

"The waiting time until a success case occurs"

Probability generally descreases exponentially over time.

Follows a Bernoulli model

P(success) = (1 - p) exp(n-1) * p  where n = number of trials

![mean](http://www.sciweavers.org/tex2img.php?eq=%5Cmu%20%3D%20%20%5Cfrac%7B1%7D%7B%5Crho%7D&bc=White&fc=Black&im=png&fs=12&ff=arev&edit=0)

![variance](http://www.sciweavers.org/tex2img.php?eq=%5Csigma%5E2%20%3D%20%5Cfrac%7B1-%5Crho%7D%7B%5Crho%5E2%7D&bc=White&fc=Black&im=png&fs=12&ff=arev&edit=0)

![standard deviation](http://www.sciweavers.org/tex2img.php?eq=%20%5Csigma%20%3D%20%20%5Csqrt%7B%0A%5Cfrac%7B1-%5Crho%7D%7B%5Crho%5E2%7D%0A%7D%20&bc=White&fc=Black&im=png&fs=12&ff=arev&edit=0)
