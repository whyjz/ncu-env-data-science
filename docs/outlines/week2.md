# Statistical Tests: How do they relate to machine learning?

<!-- **2025.03.04, 2025.03.11** -->
<!-- **2024.02.27, 2024.03.05** -->

## Lecture outline

When to use hypothesis testing?

### Five general steps of hypothesis testing
1. Set up $H_0$ (null hypothesis)
2. Set up $H_1$ (alternative hypothesis)
3. Set up test statistic and significance level ($\alpha$)
4. Find the null distribution for the test statistic; calculate the $p$-value
5. Reject or not reject $H_0$ by comparing $p$ with $\alpha$

### Case study using a one-sample t-test

Background conditions:
- We already know this species' population mean ($\mu_0$) in the large lake.
- We have a sample mean ($\bar{x}$) from 20 fish in the small lake.

Research question (hypothesis):
- Is the mean weight of a fish species from two lakes different?
- This corresponds to a null hypothesis ($H_0$): $\mu = \mu_0$

What other assumptions do we have to make to use a one-sample t-test?
- Should we assume a Gaussian population?
- Should we assume sample variance ($s^2$) equals population variance ($\sigma^2$)?

Choices:
- One-tailed test or two-tailed test?
- At what significance level?

Test statstic $t = \frac{\bar{x} - \mu_0}{s / \sqrt{N}}$
- What is its distribution?

Result reporting: 
- "The fish in the small lake is significantly heavier than that in the large lake at $\alpha = $ 0.xx ($p = $ 0.xxx)."
- "The fish in the small lake shows no significant difference in weight from that in the large lake ($\alpha = $ 0.xx; $p = $ 0.xxx)."

### Type I vs Type II errors 

False positive vs False negative

How do we design $\alpha$ and $N$ when you prefer one type of error over another?

### More about t-tests

**Two-sample t-test**: Assumption towards the samples matters
- Are both variances the same?
- Are two samples potentially dependent?
- Do the data need some arrangements?

T-tests can also test the correlation with the null hypothesis $\rho = 0$.

### p-hacking

What if we repeat the test above 100 times, each with a different sample, and report the test result with the minimum $p$? 

### Non-parametric tests

Parametric vs non-parametric tests: which should I use?

Here are tests we may mention during the class lecture:
- Wilcoxon–Mann–Whitney test: Location (mean) difference 
- Kolmogorov–Smirnov test: Goodness of fit for continuous data
  - Test statistic: maximum vertical distance from two CDF lines
<!-- - Pearson's chi-squared test: Goodness of fit for categorical data -->

### Confidence interval (CI) 

For predicting an unknown population parameter. It uses a similar concept from hypothesis testing but without any hypothesis being made. 

Significance level -> Confidence level

Result reporting: 
- xxx $\pm$ yyy (zzz% CI)
- [aaa, bbb] (zzz% CI)

Frequentist view of CI: how to interpret the interval?

### Bootstrapping

What is the situation where finding a CI of a population parameter is traditionally impossible?

To find the CI of *any* population parameter using bootstrapping:
- Percentile method: CI = $[ \theta^{\ast}_{\alpha/2}, \theta^{\ast}_{(1 - \alpha/2)} ]$ (**Do not use this!**)
- Basic method: CI = $[ 2\theta_s - \theta^{\ast}_{(1 - \alpha/2)}, 2\theta_s - \theta^{\ast}_{\alpha/2} ]$

## Final thoughts 

**How do statistical tests relate to machine learning?**
- A simple alternative (we don't need to run a ML model for all questions!)
- Understanding why having a statistics-based inference is important, maybe
- Something else?

<!-- Do you think an inflated die is fair? How to test it?

Histogram and statistical distributions -->

<!-- List at least one random variable in environmental science and remote sensing that fit each statistical distribution:
- Gaussian distribution (aka normal distribution)
- Gamma distribution
- Beta distribution
- Binomial distribution -->

<!-- Suppose Yushan measures 3952.43 m by a satellite altimeter. And the maximum measurement error of this altimeter is 0.2 m according to its documentation. What is the uncertainty of Yushan’s height? What is the 95% confidence interval of Yushan’s height? -->

## Group discussion & Demos

1. Do you have any questions about the first problem set?