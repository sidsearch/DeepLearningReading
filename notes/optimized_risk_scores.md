# Optimized risk scores
Risk scores are simple classification models that let users quickly
assess risk by adding, subtracting, and multiplying a few small numbers.
Such models are widely used in healthcare and criminal justice,
but are open built ad hoc. 
In this paper, authors present a principled approach to learn risk scores that are fully optimized for feature selection, integer coefficients, and operational constraints. 
The problem is formulated as the risk score problem as a mixed integer nonlinear program, and present a new cutting plane algorithm to efficiently recover its
optimal solution. 
Our approach can fit optimized risk scores in a way that scales linearly with the sample size of a dataset, provides a proof of optimality, and obeys complex constraints without parameter
tuning. 
We illustrate these benefits through an extensive
set of numerical experiments, and an application where we build a
customized risk score for ICU seizure prediction.