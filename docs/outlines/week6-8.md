# Neural Networks: How can you trust complex models that seem like black boxes?

<!-- **2024.03.26, 2024.04.02, 2024.04.09** -->

**2025.04.08, 2025.04.15**

## Lecture outline

Neural Network (NN): its biological origin and how it relates to data science

### Perceptrons

This is the most basic structure of a neural network!

**Architecture**: For a model with only a single output variable $y$: $\hat{y} = f\Big(\sum_i w_i x_i + b\Big)$
- **Activation function** $f$:
  - Heaviside step function
  - logistic function (or $tanh$)
  - Rectified linear unit (ReLU)
  - Softplus

Limitation on non-linear separation: only works for the *linearly separable* cases.

### Multi-layer Perceptrons (MLP)

The simplest NN that has a practical use!

**Architecture**: For a model with only a single output variable $y$: $h_j = f\Big(\sum_i^{m_1} w_{ji} x_i + b_j\Big),\quad \hat{y} = g\Big(\sum_j^{m_2} \tilde{w}_{kj} h_j + \tilde{b}_k\Big)$
- **Hidden layer**: transform the linear perceptron model into a non-linear model.
  - number of model parameters. In NN, model parameters are also called **weights.**
  - **Hyperparameters** parameters related to the architecture. Examples: number of hidden nodes.

**Loss function**: The most common selection is the mean squared error (MSE). 

**Solver**: Must be solved numerically. (see below)

### Optimizing a non-quadratic loss function

Now the loss function $J(\textbf{w})$ can have many local minima in the parameter space. An analytical solution is no longer possible.

#### Newton's method

This method involves the calculation of the Hessian matrix $\textbf{H}_0$, which contains all the second order derivatives of $J$ assessed at $\textbf{w}_0$. One iteration can be expressed as

$\textbf{w}_{k+1} = \textbf{w}_k - \textbf{H}_k^{-1} \nabla J(\textbf{w}_k)$

#### Gradient descent method 

This method replaces the Hessian matrix $\textbf{H}_0$ with a fixed or a flexible step size $\eta$, which is typically called a **learning rate**:

$\textbf{w}_{k+1} = \textbf{w}_k - \eta \nabla J(\textbf{w}_k)$

### Optimizing an MLP NN

Challenges due to its architecture:
- Curse of dimensionality?

Challenges due to the solver:
- Optimation process falls into local minimum depending on the initial weight selections.

How to address these challenges? Ensembles? Regularizations?

If the number of nodes is sufficiently large, we can achieve universal approximation even with only one hidden layer!

#### Back-Propagation

The life save of the MLP problem!

From the textbook: "Nowadays, the term ‘back-propagation’ is used somewhat ambiguously."
- It could mean the original back-propagation algorithm (with inefficient gradient descent)
- or, more likely, it could mean using only the first part involving the backward error propagation to compute the gradient of J

### Gradient descent method

### Extreme learning Machine (ELM)

The idea of using ensembles -> transform a non-linear problem back to a linear problem

**Architecture**: Same as MLP; however, two rules are used to transform it into a linear problem.
1. The weights applied to the input layer are randomly assigned for each ensemble member.
2. The actiovation function of the hidden layer is an identical function.

**Loss function**: Same as MLP.

**Solver**: the problem is analytically solved for each ensemble member.

#### Advantages of ELM

What are the advantages?

<!-- How to determine the number of hidden layer nodes $L$? -->

<!-- Skip connection -->

<!-- ### Radial Basis Functions (RBF)

This is another way to reduce the non-linearity of NN into a linear problem.

Why is it called "Radial Basis?" We'll revisit this during the kernel method section. -->

### Tuning and validation

Grid search, random search, validation, cross-validation, and double cross-validation

<!-- ### Other Emsemble methods

Help reduce the variance error (Section 8.3)

- Bagging
- Stacking -->
