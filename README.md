## Brownian-Motion-for-Finance
Brownian Motion for Financial Math is a Python-based project that simulates and analyzes Brownian motion, a key stochastic process in financial mathematics.
The project explores random walks, scaled random walks, and continuous Brownian motion, with applications in modeling stock prices and other financial phenomena. It includes visualizations and statistical analysis to help understand the fundamental properties of stochastic processes like martingales and quadratic variation. Perfect for students and professionals in quantitative finance or stochastic calculus.

## Project Overview

- **Objective**: To understand and simulate Brownian motion and its properties, including how it behaves as a stochastic process (Markov process) and accumulates quadratic variation.
- **Key Concepts**:
  - **Brownian Motion**: A continuous-time stochastic process that is a fundamental building block in financial mathematics.
  - **Quadratic Variation**: A key feature of Brownian motion, differentiating stochastic calculus from ordinary calculus.
  - **Martingale**: A stochastic process where the conditional expectation of future values, given the present, equals the current value, implying no "drift" over time.

## Requirements

To run this project, you will need the following libraries:

- `numpy`
- `scipy`
- `matplotlib`

You can install these libraries using pip:

```bash```
pip install numpy scipy matplotlib


## Simulation Details
In the notebook, we simulate the following:

Random Walks: A symmetric random walk and a scaled random walk are simulated as discrete approximations of Brownian motion.
Brownian Motion: We simulate paths of Brownian motion and analyze its statistical properties, such as expected value and variance over time.
The code is divided into different sections for:

Parameter Setup: Defining the number of simulations (M) and the time horizon (t).
Random Walk Simulation: Discrete random walk paths are generated and plotted.
Brownian Motion Simulation: The limit of the random walk as the time step tends to zero, generating continuous paths of Brownian motion.
Usage
Clone this repository.
Install the required dependencies.
Open the Jupyter Notebook Brownian_Motion_for_Financial_Math.ipynb.
Run the cells sequentially to see the simulation results and visualizations.
Example Output
Random Walk Plot: A visual representation of several paths of a symmetric random walk.
Brownian Motion Plot: A continuous-time simulation showing multiple paths of Brownian motion.

## Brownian Motion
A Brownian motion is a stochastic process **$${\lbrace W_t\rbrace}_{t\in[0,T]}$$**

Filtered probability space $$({\ohm, \mathscr{F}, \mathscr{P}, \lbrace F_t\rbrace}_{t\in[0,T]})$$

**$W : [0,T] \times \ohm \rightarrow \mathscr{R}$**
- $W_0 = 0$
- W has independent increments.
- W has Gaussian (normal) increments.
- W has continuous sample paths (almost surely).

**$W_t \sim N(0,t)$**
- **$\mathcal{E}(W_{t_i + 1} - W_{t_i}) = 0$**
- **$Var(W_{t_i + 1} - W_{t_i}) = t_{i+1} - t_i $**

## Symmmetric Random Walk
Picture you have successive coin tosses, $\omega = \omega_1 \omega_2 \omega_3 ...$ 
 Where $\omega_n$ is the outcome of the $n^{th}$ toss.

| Condition          | Value of $X_j$|
|--------------------|---------------|
| $\omega_j = H$     | 1             |
| $\omega_j = T$     | -1            |


If we define $M_0 = 0,$

$M_k = \ \sum_{j=1}^{k} X_{j}  \$

## Scaled Symmmetric Random Walk
To approximate a Browian Motion we can spped up time and scale down the step size.

$W^(n)(t) = \frac{1}{\sqrt{n}}M_{nt}$


## Limit of Binomial Distribution
As n increases, the binomial distribution converges to the normal distribution with variance t.

$W^(n)(t) = \frac{1}{\sqrt{n}}M_{nt}$




