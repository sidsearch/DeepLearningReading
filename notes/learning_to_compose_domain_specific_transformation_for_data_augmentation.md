# what is the paper proposing
* data augmentation using generative sequence model over user-specified transformation functions using generative adversarial process
* uses transformation function which is robust to misspecified user input and is trained on unlabeled data
* transformation model can then be used to perform data augmentation for any end discriminative model

# how it works
* basically user provides set of transformation function h(1),h(2),,... h(k)  and unlabeled data.
* A generative model is trained D and G which produces TF sequence hT(1), hT(2).... hT(k).
* finally a generative model is used to perform data augementation for an end discriminative model D(f) 

