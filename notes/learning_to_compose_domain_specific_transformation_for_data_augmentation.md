# what is the paper proposing
* data augmentation using generative sequence model over user-specified transformation functions using generative adversarial process
* uses transformation function which is robust to misspecified user input and is trained on unlabeled data
* transformation model can then be used to perform data augmentation for any end discriminative model

# how it works
* basically user provides set of transformation function h(1),h(2),,... h(k)  and unlabeled data.
* A generative model is trained D and G which produces TF sequence hT(1), hT(2).... hT(k).
* finally a generative model is used to perform data augementation for an end discriminative model D(f) 

# for generator:
Mean field: each sequential TF is chosen independently, reducing the task to learning the  K sampling frequencies of the TFs
Long short-term memory network (LSTM): the input to each cell is a one-hot vector of the previously sampled TF, and the output from each cell of the network is a sampling distribution for the next TF. Making state-based decisions is critical when TFs are lossy when applied together, or are non-commutative.

