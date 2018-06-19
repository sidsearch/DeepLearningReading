## Efficient Neural Architecture Search

we propose efficient neural archiecture search

fast and inexpensive approach

controller discovers NN architectures by searching for optimal subgraph within a large computational graph 

controller is trained with policy gradient to select subgraph that maximizes the expected reward on a validation set 

meanwhile the model corresponding to selected subgraph is trained to minimize a canonical cross entropy loss 

sharing parameters among child models allows ENAS to deliver strong empirical performances while using much fewer GPU hours than exisiting automatic model design approaches 

1000x less expensive than standard ENAS 

PTB, ENAS discovers a novel architecture that achieves a test perplexity of 55.8 establishing state of art among all methods with post training processing 


On CIFAR-10, ENAS finds novel architecture that achives 2.98% test error