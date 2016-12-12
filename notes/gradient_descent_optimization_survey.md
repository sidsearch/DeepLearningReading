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

