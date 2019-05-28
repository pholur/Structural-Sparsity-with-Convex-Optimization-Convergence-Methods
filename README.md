# Structural-Sparsity-with-Convex-Optimization-Convergence-Methods
In this project, we solve for structural sparsity in the inverse problem of solving for source estimates, originally passed through an affine function with a gain matrix A and error matrix E. The MAP optimal solution is the same for E as a Gaussian distribution. The affine function is given by, **Y = AX + E**.

It is important to know that A need not be square and in most cases, it is in fact a map between some sources and detecting sensors. In many cases, the **number of sources highly out-number the number of sensors**. As a result, if X is generally tall and of dimension m x n, where n is the number of time instances and m is the number of sources, A is then of dimension k x m where k is the number of sensors. A then is wide. Further, E is then of dimension k x n. The inverse problem requires estimating X given Y.

The 3 files in this project compare the convergence rates of different solvers including ADMM, PGD, and APGD in solving for the structured and sparse X regularized with an L-21 norm as defined in the code and report. The *2.ipynb file uses the MNE library to use I/O operations and determine brain source locations; this process uses the same functions coded by hand in the *1.ipynb files.

Descriptions for each notebook is provided in each file and run self-sufficiently. The code requires some additional libraries that may be installed with >> pip install software-name. For further questions, please contact pholur@g.ucla.edu.

