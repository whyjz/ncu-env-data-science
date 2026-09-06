# Warming-up

<!-- **2025.02.25** -->
<!-- **2024.02.20** -->

## Lecture outline

### Intro

What does the term "data science" mean to you?

So we have two terms here:
- Statistics
- Machine learning (ML)
<!-- - Data science -->
How are they different from each other? For example, what is the difference between a "statistical model" and a "machine learning model?" Or maybe they are the same thing? Just fancy words to be created to confuse people?

<!-- What is "learning" as in machine learning? -->

What is the difference between supervised and unsupervised learning?

Checking in your answers for Q4 in the Pre-course Quiz.

### Data skills

Here are things we don't primarily focus on during the class but are essential for building up your data skills for reproducible science.

- Programming
- Collaboration and version control (Git & GitHub)
- Jupyter (incl. Google Colab)
- Data import and wrangling
- Visualization

### Basics of statistics 

Random variable: A **value** that follows a probability distribution. Are the following quantities random variables?
- The number of apples in a basket
- Your height
- The height of a person sitting here who I randomly pick up
<!-- - Today’s temperature -->
<!-- - The number I get by rolling a die -->

<!-- What is a probability density function (PDF)? How is it different from a probability distribution? -->

Now let's revisit expectation, variance, and their mathematical expressions (cont. Q1 in Pre-course Quiz): 

<!-- Derive the expectation and the variance of the Bernoulli distribution $Ber(x|p) = p^x(1-p)^{1-x}$. -->

Gaussian distribution: many distributions converge to this thanks to the central limit theory
  - How does this relate to Q2 in the Pre-course Quiz?

<!-- ### More about probability distributions -->

<!-- - Poisson distribution -->
<!-- - Student t-distribution: Bounded to the mean -->
<!-- - Chi-squared ($\chi^2$) distribution: Bounded to the square of the Gaussians -->
<!-- - Beta and Gamma distributions: different supports for different kinds of environment variables -->

### Statistical Tests

**How do statistical tests relate to machine learning?**
- A simple alternative (we don't need to run a ML model for all questions!)
- Having a statistics-based inference is sometimes important

**Five general steps of hypothesis testing**
1. Set up $H_0$ (null hypothesis)
2. Set up $H_1$ (alternative hypothesis)
3. Set up test statistic and significance level ($\alpha$)
4. Find the null distribution for the test statistic; calculate the $p$-value
5. Reject or not reject $H_0$ by comparing $p$ with $\alpha$

### p-hacking

What if we repeat the test above 100 times, each with a different sample, and report the test result with the minimum $p$? 

### Confidence interval (CI) 

For predicting an unknown population parameter. It uses a similar concept from hypothesis testing but without any hypothesis being made. 

Significance level -> Confidence level

Result reporting: 
- xxx $\pm$ yyy (zzz% CI)
- [aaa, bbb] (zzz% CI)

Frequentist view of CI: how to interpret the interval?

**Bootstrapping**: Dealing with a situation in which finding a CI for a population parameter is traditionally impossible.

To find the CI of *any* population parameter using bootstrapping:
- Percentile method: CI = $[ \theta^{\ast}_{\alpha/2}, \theta^{\ast}_{(1 - \alpha/2)} ]$ (**Do not use this!**)
- Basic method: CI = $[ 2\theta_s - \theta^{\ast}_{(1 - \alpha/2)}, 2\theta_s - \theta^{\ast}_{\alpha/2} ]$

## Group discussion & Demos

1. Discuss how you would reproduce the figure for Q3 in the Pre-course Quiz.
2. Get the data necessary for doing Exercise 5.8 in Hsieh's book.