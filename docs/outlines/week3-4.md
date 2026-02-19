# Linear Models and Regularization: Under what circumstances do we prefer to sacrifice unbiasedness?

<!-- **2025.03.18, 2025.04.01** -->
<!-- **2024.03.12, 2024.03.19** -->

## Lecture outline

### Common components of all regression models

1. **Architecture**: The connection between input and output variables
2. **Loss function**: The target quantity to be optimized. Aka *cost function* or *objective function*
3. **Solver**: The method to find a solution

### Simple linear regression (SLR)

**Architecture**: $y_i = \hat{y}_i + \epsilon_i = a_0 + a_1 x_i + \epsilon_i$

Assumptions (Are these necessary??)
- Only $\epsilon_i$ is a random variable, $\sim N(0, \sigma_i^2)$
- All $\epsilon_i$ are independent and identically distributed (*i.i.d.*); $\text{Cov}(\epsilon_i, \epsilon_j) = 0$ when $i \neq j$.
- $\sigma_i^2$ is the same for all $i$; $\sigma_i^2 = \sigma^2$

**Loss function**: Ordinary least square (OLS); $ J = SSE = \sum_{i=1}^{N} \epsilon_i^2 $
- What are the advantages of using this loss function?

**Solver**: Analytic
- Normal equations

#### More about SLR

Gauss--Markov Theorem and **BLUE** (best linear unbiased estimator)

The sum of squares: How much variability can be explained/modeled by a regression model?
- $SST = SSE + SSR$

What is the difference between $R^2$ and $r$?

Confidence interval vs. Prediction interval

When there is a serial correlation...
- Durbin--Watson statistic

### Multiple linear regression (MLR)

What does "linear" mean in a linear regression model?

#### Components

**Architecture**: $\textbf{y} = \textbf{X}\textbf{a} + \boldsymbol{\epsilon}$  (We'll use this at the class)
Other equivalent expression is also commonly seen in the environmental science studies: 
- $\textbf{d} = \textbf{G}\textbf{m}$    (Many geophysicists use this)

**Loss function**: OLS. $ J = SSE = \boldsymbol{\epsilon}^\text{T} \boldsymbol{\epsilon}$

**Solver**: Analytic.
- What are the normal equations?
- Solution: $\hat{\textbf{a}}=(\textbf{X}^\text{T}\textbf{X})^{-1}\textbf{X}^\text{T}\textbf{y}$

#### More about MLR

Circular and categorical Data: transform them so that we can use a linear model

Analysis of Variance (ANOVA)
- Sum of squares explained by each predictor
- F-test

#### Stepwise regression

When you have lots of potential predictors...
- The more, the better?
- The less, the better?
- When you have no choice but to keep all the predictors?

How do we do stepwise regression?

Criticism: Isn't this **cherry-picking**?

Rank-deficient (or ill-conditioned) problems and regularized least-squares (i.e., a family of shrinkage methods)

### Regularized least-squares models

Regularization tries to redesign the loss function by imposing an additional constraint.

What are its benefits?
- To keep all the predictors in the regression model
- To improve the solution by making the input towards full rank or better conditions.

Example: The one-hot encoding case from the worksheet

#### Ridge regression

a.k.a. L-2 regularization or Tikhonov regression 

**Architecture**: same as MLR

**Loss function**: Regularized OLS. $ J = \boldsymbol{\epsilon}^\text{T} \boldsymbol{\epsilon} + \lambda\textbf{a}^\text{T}\textbf{a}$
- This is the explicit expression using the Lagrange multiplier $\lambda$.
- It is equivalent to a standard OLS ($\boldsymbol{\epsilon}^\text{T} \boldsymbol{\epsilon}$) under a constraint $\textbf{a}^\text{T}\textbf{a} \leq b$. See Appendix B of the textbook for more details.

**Solver**: Analytic
- Solution: $\hat{\textbf{a}}=(\textbf{X}^\text{T}\textbf{X}+\lambda \textbf{I})^{-1}\textbf{X}^\text{T}\textbf{y}$

How to select the **Hyperparameter** $\lambda$?
- **Validation** (This is the time you start to see the so-called validation data!)
- **Cross-validation** (We'll continue to talk about this during the NN topic)

#### Lasso

a.k.a. L-1 regularization or "least absolute shrinkage and selection operator"

**Architecture**: same as MLR

**Loss function**: Regularized OLS. $ J = \boldsymbol{\epsilon}^\text{T} \boldsymbol{\epsilon} + \lambda \sum_{j=1}^{m}|a_j|$
- What is its implicit form?

**Solver**: Typically solved numerically since the loss function is indifferentiable. We'll talk about some possible methods in the next topic.

LASSO also works as a predictor selector -- how so?
- Finding the constraint region of Ridge and LASSO
- What is the shape of the regions?
- Lasso finds a solution with greater sparsity.

### Generalized Least Squares

a.k.a. Weighted least squares (WLS). Exploring more ways to redesign the loss function!

**Architecture**: same as MLR

**Loss function**: WLS; $ J = \boldsymbol{\epsilon}^\text{T} \textbf{C}^{-1}\boldsymbol{\epsilon}$ where $\textbf{C}$ is the covariance matrix of the residual.

**Solver**: Analytically.

What does this model typically imply for the assumption about the data? Why Mahalanobis distance?

## Final thoughts

**Under what circumstances do we prefer to sacrifice unbiasedness?**
- $\textbf{X}^\text{T}\textbf{X}$ is not invertible (i.e., $\textbf{X}$ is a rank-deficient matrix)
- $\textbf{X}^\text{T}\textbf{X}$ is invertible, but $\textbf{X}$ has columns that are highly correlated to each other (i.e., $\textbf{X}$ is an ill=conditioned matrix)
- Are there other reasons? (1)
- Are there other reasons? (2)

## Group discussion & Demos

1. Introduction to Jupyter Notebook / JupyterLab
2. Load an Exercise data set using Jupyter Notebook (hosted by [Google Colaboratory](https://colab.google/), [Callysto Hub](https://www.callysto.ca/), or your local machine)

<!-- 1. Overview of the term project output: an example https://ucb-stat-159-s23.github.io/project-Group28/README.html 
2. Another example is this class webpage. -->