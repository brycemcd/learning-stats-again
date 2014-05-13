# Distributions

+ [Normal](#normal-distribution)
+ [Bernoulli](#bernoulli-model)
+ [Geometric](#geometric-distribution)
+ [Binomial](#binomial-distribution)
+ [Negative Binomial](#negative-binomial-distribution)
+ [Poisson](#poisson-distribution)

## Normal Distribution

By far the most referenced and most recognizable distribution.

Requires a normal distribution (TODO: tests for normality)

Standardized with a Z score for comparison of data with different means and standard deviations. Expressed as

![definition of Z statistic](http://www.sciweavers.org/tex2img.php?eq=Z%20%3D%20%5Cfrac%7B%28%20x%20-%20%5Cmu%20%29%7D%7B%20%5Csigma%20%20%7D&bc=White&fc=Black&im=png&fs=12&ff=arev&edit=0)

![mean](http://www.sciweavers.org/tex2img.php?eq=%20%5Cmu%20%3D%20mean&bc=White&fc=Black&im=jpg&fs=12&ff=arev&edit=0)

![Standard Deviation](http://www.sciweavers.org/tex2img.php?eq=%20%5Csigma%20%3D%20Standard%20Deviation&bc=White&fc=Black&im=png&fs=12&ff=arev&edit=0)

### Is a data sample normal?

TODO: tests of normality

#### Histogram

Visually, inspect a histogram and decide if it "looks" normal. 

#### Q-Q plot

[A Q-Q graph](http://en.wikipedia.org/wiki/Q%E2%80%93Q_plot) displays a plot of two distributions for comparison. For a normal distribution, 
the data will fall along the y=x line. The data will be concentrated in the middle of the graph with few points falling outside the y=x line.

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

Probability generally decreases exponentially over time.

Follows a Bernoulli model

P(success) = (1 - p) exp(n-1) * p  where n = number of trials

![mean](http://www.sciweavers.org/tex2img.php?eq=%5Cmu%20%3D%20%20%5Cfrac%7B1%7D%7B%5Crho%7D&bc=White&fc=Black&im=png&fs=12&ff=arev&edit=0)

![variance](http://www.sciweavers.org/tex2img.php?eq=%5Csigma%5E2%20%3D%20%5Cfrac%7B1-%5Crho%7D%7B%5Crho%5E2%7D&bc=White&fc=Black&im=png&fs=12&ff=arev&edit=0)

![standard deviation](http://www.sciweavers.org/tex2img.php?eq=%20%5Csigma%20%3D%20%20%5Csqrt%7B%0A%5Cfrac%7B1-%5Crho%7D%7B%5Crho%5E2%7D%0A%7D%20&bc=White&fc=Black&im=png&fs=12&ff=arev&edit=0)

## Binomial Distribution

Describes k success in n Bernoulli trials

![probability](http://www.sciweavers.org/tex2img.php?eq=P%28k%3E%3D1%29%20%3D%20%5Crho%20%5E%20k%20%281-%20%5Crho%20%29%5E%7B%28n-k%29%7D&bc=White&fc=Black&im=png&fs=12&ff=arev&edit=0)

number of ways to choose k successes: ![n choose k](http://www.sciweavers.org/tex2img.php?eq=%20%5Cbig%28%5Cfrac%7Bn%7D%7Bk%7D%5Cbig%29%20%20%3D%20%5Cfrac%7Bn%21%7D%7Bk%21%28n-k%29%21%7D&bc=White&fc=Black&im=png&fs=12&ff=arev&edit=0)

General Formula: ![n choose k general](http://www.sciweavers.org/tex2img.php?eq=%20%5Cbig%28%5Cfrac%7Bn%7D%7Bk%7D%5Cbig%29%20%20%3D%20p%5Ek%281-p%29%5E%7Bn-k%7D%20%3D%20%5Cfrac%7Bn%21%7D%7Bk%21%28n-k%29%21%7Dp%5Ek%281-p%29%5E%7Bn-k%7D&bc=White&fc=Black&im=png&fs=12&ff=arev&edit=0)

mean: u = np
variance: np(1-p)
![standard deviation](http://www.sciweavers.org/tex2img.php?eq=%20%5Csigma%20%20%3D%20%5Csqrt%7Bn%5Crho%281-%5Crho%29%7D%20&bc=White&fc=Black&im=png&fs=12&ff=arev&edit=0)

4 conditions of a binomial distribution:

+ Each trial is independent
+ n = # of trials = fixed number of trials
+ boolean outcome of each trial
+ P(success) = same for each trial

## Negative Binomial Distribution

Models the probability that the _k_th success will occur on the _n_th trial

Useful for a specific trial vs needle in a haystack approach like the regular binomial distribution. Answers the question "What's the likelihood the 4th attempt will be successful?

Conditions for distribution:

+ Same as binomial distribution plus:
+ last trial is a success
+ All trials are independent!

P(success | last trial) = ![negative binomial probability](http://www.sciweavers.org/tex2img.php?eq=%28%5Cfrac%7Bn-1%7D%7Bk-1%7D%29%5Crho%5Ek%281-%5Crho%29%5E%7Bn-k%7D&bc=White&fc=Black&im=png&fs=12&ff=arev&edit=0)

## Poisson Distribution

Estimates the number of rare events in a large population over time. Great for modeling rare cases like heart attacks.

![probability](http://www.sciweavers.org/tex2img.php?eq=P%28k%20events%29%20%3D%20%5Cfrac%7B%0A%20%5Clambda%20%5E%20k%20e%5E%7B-%5Clambda%7D%0A%7D%7Bk%21%7D%20&bc=White&fc=Black&im=png&fs=12&ff=arev&edit=0)

for all k in a real number set

![mean](http://www.sciweavers.org/tex2img.php?eq=%5Cmu%20%3D%20%5Clambda&bc=White&fc=Black&im=png&fs=12&ff=arev&edit=0)

![standard deviation](http://www.sciweavers.org/tex2img.php?eq=%5Csigma%20%3D%20%20%5Csqrt%7B%5Clambda%7D%20&bc=White&fc=Black&im=png&fs=12&ff=arev&edit=0)

lambda is the rate of the rare occurrence

## t Distribution

Meant for small (< 30-40) observations. As observation numbers grow, t
approximates a normal distribution.

Degrees of freedom are equal to 1 - the number of observations

## F Distribution
