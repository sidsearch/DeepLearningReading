# Optimized risk scores
Risk scores are simple classification models that let users quickly
assess risk by adding, subtracting, and multiplying a few small numbers.
Such models are widely used in healthcare and criminal justice,
but are open built ad hoc. 
In this paper, authors present a principled approach to learn risk scores that are fully optimized for feature selection, integer coefficients, and operational constraints. 
The problem is formulated as the risk score problem as a mixed integer nonlinear program, and present a new cutting plane algorithm to efficiently recover its
optimal solution. 
The proposed approach can fit optimized risk scores in a way that scales linearly with the sample size of a dataset, provides a proof of optimality, and obeys complex constraints without parameter
tuning. 


## problem definition
(X_i, Y_i) are training samples.
<lambda, x> where lambda is a coefficient vector and lambda_0 is the intercept. predicted risk is modeled as for example i belongs to  positive class as 

P(i)  = Pr(y=1|x) = 1/1+exp(-<lambda,x>)

In this setup lambda represents points for feature j. Given features x_i, users tally the points to get a risk score s_i = <lambda, x_i>


,,,,,,,
