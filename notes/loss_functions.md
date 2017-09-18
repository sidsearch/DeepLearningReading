# loss functions
* computationally feasible loss functions representing price paid for inaccuracy of predictions in classification problems.


# cross entropy loss
cross entropy is calculated as 
 = - sum p(x) log q(x) 

Often neural networks are trained to minimize the cross entropy between the ground truth distribution and predicted distribution.

# logistic loss
when prediction is (p) and label is (y), loss function l(p,y) for logistic loss is 

log(1+exp(-yp))


# hinge loss 
max(0,1-yp) 

# squared 

1/2(p-y)^2



