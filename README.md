# learning_dynamics
This repository references papers on learning dynamics from temporal data. We are more precisely concerned with:

- The dynamics: learning $f$ in $\dot{X} = f(X,t)$ from noisy observations $(Y(t_i) = X(t_i) + \varepsilon)_{1\le i \le n\}$ and not simply interactions such as $X_1\to X_2$ as in Gene Regulatory Network Inference.
- Mechanistic form: we seek an interpretable form for $f$. Therefore, methods concerned with simply learning $f$ using a neural network or gaussian process are not enough. Typically, one assumes that $f$ takes a parametric form: $f(X,t) \equiv f(X,t,\theta)$, for instance $f_1(X,t,\theta) := \theta_1 X_1 - \theta_2 X_2^2$ would be the parametric vector field of the first variable $X_1$.

We focus mostly on learning ODEs from biological data, but same approaches usually apply to PDEs and other research fields than Biology.

### SINDy-like methods

- [Ensemble-SINDy: Robust sparse model discovery in the low-data, high-noise limit, with active learning and control, 2022](https://royalsocietypublishing.org/doi/full/10.1098/rspa.2021.0904)
- [Identification of dynamic mass-action biochemical reaction networks using sparse Bayesian methods, 2022](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1009830)
- [Inferring Biological Networks by Sparse Identification of Nonlinear Dynamics, 2016](https://ieeexplore.ieee.org/document/7809160)
- [Discovering governing equations from data by sparse identification of nonlinear dynamical systems, 2016](https://www.pnas.org/doi/10.1073/pnas.1517384113)
