# Distributionally Robust Linear Quadratic Control

-----------

## Abstract

Linear-Quadratic-Gaussian (LQG) control is a fundamental control paradigm that is studied in various fields such as engineering, computer science, economics, and neuroscience. It involves controlling a system with linear dynamics and imperfect observations, subject to additive noise, with the goal of minimizing a quadratic cost function for the state and control variables. In this work, we consider a generalization of the discrete-time, finite-horizon LQG problem, where the noise distributions are unknown and belong to Wasserstein ambiguity sets centered at nominal (Gaussian) distributions. The objective is to minimize a worst-case cost across all distributions in the ambiguity set, including non-Gaussian distributions. Despite the added complexity, we prove that a control policy that is linear in the observations is optimal for this problem, as in the classic LQG problem. We propose a numerical solution method that efficiently characterizes this optimal control policy. Our method uses the Frank-Wolfe algorithm to identify the least-favorable distributions within the Wasserstein ambiguity sets and computes the controller's optimal policy using Kalman filter estimation under these distributions.

------------

### Dependencies

- Numpy 1.24.3
- Pytorch 2.0
- [Pymanopt] https://pymanopt.org/
- [Cvxpy] https://www.cvxpy.org/install/
- [Mosek] https://www.mosek.com/

-----------

### Figure 1 (a)
```
python figure_1a.py
```

![scale_plot](https://github.com/DR-Control/dr-control/assets/133906859/a9faf941-22b3-423f-9acb-11e76f966077)


### Figure 1 (b)
```
python figure_1b.py
```

![convergence](https://github.com/DR-Control/dr-control/assets/133906859/3a3ecbbc-8414-4a0d-b6b1-3748c88a77c8)

### Plotting the results
We plot the results using the plotter.ipynb notebook.
