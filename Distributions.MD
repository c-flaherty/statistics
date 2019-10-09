# Distributions

This file consists of descriptions, references, and examples for common distributions (both discrete and continuous).

## Continuous Distributions

### Poisson Distribution
- The Poisson distribution is the binomial distribution as the number of trials approaches infinity.

### Exponential Distribution
- The exponential distribution is the geometric distribution as the number of trials approaches infinity. In its most common use case, it models the probability that a certain amount of time elapses before an event occurs, where the probability of the event occuring at one instance is independent of the probability of that event occuring at a prior instance.
- It can be alternatively defined as modeling the time until 1 success in a Poisson process
- A good description of the distribution as well the intuition behind it can be found here: https://www.probabilitycourse.com/chapter4/4_2_2_exponential.php

### Gamma Distribution
- The Gamma distribution is a modification of the exponential distribution, where the rate of decay varies at different values of the r.v. It takes two inputs: shape (α) and rate (λ), where λ is the rate of decay and α is the rate of change of the rate of decay. If α = 1, the Gamma distribution is equivalent to the exponential distribution because the rate of decay λ does not vary. If α < 1, the Gamma distribution models the probability that a certain amount of time elapses before an event occurs, where the probability of the event occuring grows increasingly less likely for larger intervals of time. If α > 1, the Gamma distribution models the probability that a certain amount of time elapses before an event occurs, where the probability of the event occuring grows increasingly more likely up to a certain duration of time (mode) and then decays for greater durations of time.

### Normal Distribution 
- The normal distribution models a r.v. that has a most likely value (mode) and decays for any deviation from that value. It looks like a symmetric "bell shape". It is also referred to as the "bell curve" or the "Gaussian" distribution.
- Most random variables do not follow this distribution, but it is very relevant because the expectation of a randomly chosen sample approaches the normal distribution as the sample size increases. This is important practically because many random variables can be modeled as a sum of many other random variables and hence we can argue that their distribution is approximated by the normal distribution.
- A good description of it and its motivations can be found here: https://www.probabilitycourse.com/chapter4/4_2_3_normal.php
- A good description of its relevance in practical applications, using the CLT, can be found here (with pictures): https://towardsdatascience.com/the-central-limit-theorem-and-its-implications-4a7adac9d6de
