---
title: "The memory of expected value and variance"
date: 2021-10-25T12:41:56+02:00
description: ""
categories:
- Research
- Economics
tags:
- regression
keywords:
- tech
coverImage: https://s6.favim.com/orig/150824/dice-luck-numbers-probability-Favim.com-3173606.jpg
coverSize: partial
thumbnailImage: https://s6.favim.com/orig/150824/dice-luck-numbers-probability-Favim.com-3173606.jpg
thumbnailImagePosition: left
metaAlignment: center
Math: True
---
Reviewing the basic statistical concepts: expected value and variance.
<!--more-->
{{< toc >}}
# Definition of the expected value
In probability theory, the expected value of a random variable {\displaystyle X}X, often denoted E(X), E[X], or EX, is {{< hl-text orange>}}a generalization of the weighted average{{< /hl-text >}}, and is intuitively the arithmetic mean of a large number of independent realizations of X. The expectation operator E is also commonly stylized as E or $\mathbb {E}$ . The expected value is also known as the **expectation**, **mathematical expectation**, **mean**, **average**, or **first moment**. Expected value is a key concept in economics, finance, and many other subjects.

# Expected value of a continuous or a discrete random variable

Let X be **a continuous random variable** with range [a, b] and probability
density function f(x). The expected value of X is defined by:

$$ E(x) = \int_a^b xf(x) \mathrm{d}x$$

Let’s see how this compares with the formula for **a discrete random variable**:
$$ E(x) = \sum_{i=1}^n  x_ip(x_i) $$

The discrete formula says to take a weighted sum of the values $x_i$ of X, where the weights are the probabilities $p_(x_i)$. Recall that f(x) is a probability density. Its units are prob/(unit of X).

# Definition of variance

In probability theory and statistics, {{< hl-text orange>}}variance is the expectation of the squared deviation of a random variable from its population mean or sample mean{{< /hl-text >}}.

$$ Var(X)= E[(X - \mu )^2]$$

Variance is a measure of dispersion, meaning it is a measure of how far a set of numbers is spread out from their average value. Variance has a central role in statistics, where some ideas that use it include descriptive statistics, statistical inference, hypothesis testing, goodness of fit, and Monte Carlo sampling.

![](https://upload.wikimedia.org/wikipedia/commons/thumb/f/f9/Comparison_standard_deviations.svg/400px-Comparison_standard_deviations.svg.png)
Example of samples from two populations (总体) with the same mean but different variances. The red population has mean 100 and variance 100 (SD=10) while the blue population has mean 100 and variance 2500 (SD=50).

An advantage of variance as a measure of dispersion is that it is more amenable to **algebraic manipulation** than other measures of dispersion such as the expected absolute deviation; for example, ***the variance of a sum of uncorrelated random variables is equal to the sum of their variances***. A disadvantage of the variance for practical applications is that, unlike the standard deviation, ***its units differ from the random variable***, which is why **the standard deviation** is more commonly reported as a measure of dispersion once the calculation is finished.

There are two distinct concepts that are both called "variance". One, as discussed above, is part of **a theoretical probability distribution** and is **defined by an equation**. The other variance is **a characteristic of a set of observations**. When variance is calculated from observations, those observations are typically measured from a real world system. If **all** possible observations of the system are present then the calculated variance is called the {{< hl-text orange>}}population variance{{< /hl-text >}}. Normally, however, only a subset is available, and the variance calculated from this is called the {{< hl-text orange>}}sample variance{{< /hl-text >}}. The variance calculated from a sample is considered **an estimate of the full population variance**. There are multiple ways to calculate an estimate of the population variance, as discussed in the section below.

# Variance of a continuous or a discrete random variable

If the generator of random variable X is discrete with probability mass function $x_{1} \mapsto p_{2}$, $x_{1} \mapsto p_{2}$,..., $x_{n} \mapsto p_{n}$, then
 $$ Var(X)=\sum _{i=1}^{n} p_{i}\cdot (x_{i}-\mu )^{2} $$,

 where $\mu$  is the expected value. That is,

 $$ \mu = \sum_{i=1}^{n} p_{i}x_{i} $$

If the random variable X has a probability density function f(x), and F(x) is the corresponding cumulative distribution function, then

$$ Var(X)=\sigma^{2} = \int_{\mathbb {R} }(x-\mu)^{2}f(x)\,dx =\int_{\mathbb {R} }x^{2}\,dF(x)-\mu^{2},$$

or equivalently,

$$ Var(X)=\int_{\mathbb {R} }x^{2}f(x)\,dx-\mu^{2}$$
