Gradient Descent Variants
-------------------------

There are mainly 3 variants of gradient descent, which differ in how much data we use to compute the gradient of the objective function. Depending on the amount of the data, we make a tradeoff between the accuracy of the parameter update and time to perform an update.

Batch gradient descent
-----------------------
Vanilla GD aka batch gradient descent, computes gradient of the cost function, w.r.t. the parameters \theta for the entire training dataset

	theta = theta - eta. gradient(J(theta))

As we need to calculate the gradients of the whole datasets to perform just one update,batch GD is very slow. Also intractable for datasets that do not fit in memory.

BGD also does not allow models to be updated online with new examples on the fly.

Stochstic gradient descent
--------------------------
SGD performs parameter update on each example such x_i,y_i where 
	theta = theta - eta. gradient(J(theta, x_i,y_i))
	
difference from Batch GD is that it removes redundancy as it does not compute the gradient on the same examples again.

Mini Batch gradient descent
---------------------------
Mini Batch takes best of the both batch and stochastic gradient descent and performs an update on every mini batch of n training examples

for example it takes x[i:i+n] and y[i:i+n] and performs an parameter update on those.

Challenges so far
------------------
Vanilla mini batch GD does not guarrente convergence.
1. Choosing proper learning rate can be difficult. small
