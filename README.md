# Learning Dynamics
This repository references papers on learning dynamics from temporal data. We are more precisely concerned with:

- The dynamics: learning $f$ in $\dot{X} = f(X,t)$ from noisy observations $(Y(t_i) = X(t_i) + \varepsilon)_{1\le i \le n\}$ and not simply interactions such as $X_1\to X_2$ as in Gene Regulatory Network Inference.
- Mechanistic form: we seek an interpretable form for $f$. Therefore, methods concerned with simply learning $f$ using a neural network or gaussian process are not enough. Typically, one assumes that $f$ takes a parametric form: $f(X,t) \equiv f(X,t,\theta)$, for instance $f_1(X,t,\theta) := \theta_1 X_1 - \theta_2 X_2^2$ would be the parametric vector field of the first variable $X_1$.

We focus mostly on learning ODEs from biological data, but same approaches usually apply to PDEs and other research fields than Biology.

### Sparse and SINDy-like methods

- [Automatic differentiation to simultaneously identify
nonlinear dynamics and extract noise probability
distributions from data, 2022](https://iopscience.iop.org/article/10.1088/2632-2153/ac567a)
- [Ensemble-SINDy: Robust sparse model discovery in the low-data, high-noise limit, with active learning and control, 2022](https://royalsocietypublishing.org/doi/full/10.1098/rspa.2021.0904)
- [Identification of dynamic mass-action biochemical reaction networks using sparse Bayesian methods, 2022](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1009830)
- [Inferring Biological Networks by Sparse Identification of Nonlinear Dynamics, 2016](https://ieeexplore.ieee.org/document/7809160)
- [Discovering governing equations from data by sparse identification of nonlinear dynamical systems, 2016](https://www.pnas.org/doi/10.1073/pnas.1517384113)
- [Gaussian processes meet NeuralODEs: A Bayesian framework for learning the dynamics of partially observed systems from scarce and noisy data, 2022](https://arxiv.org/pdf/2103.03385.pdf)

### Symbolic regression

- [D-CODE: Discovering Closed-form ODEs from Observed Trajectories, 2022](https://openreview.net/pdf?id=wENMvIsxNN)
- [AI Feynman: A physics-inspired method for symbolic regression, 2020](https://www.science.org/doi/10.1126/sciadv.aay2631)
