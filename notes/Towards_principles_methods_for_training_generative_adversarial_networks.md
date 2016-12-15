GANs are starting to be  widely used. Yet it is very hard to train. Often we rely on heuristics to train GANs. 

not too different from variational autoencoders. core idea is we first sample from a prior z~ p(z) and then output our final sample g_theta(z). Always g_theta(zz) is a neural 
network parametrized by theta. the main difference is how we train g_theta

1. Kullback-leibler(KL) divergence between unknown data P_r and our generators P_g 

KL(p_r||P_g)  = integrate(P_r(x) log[P_r(x)/P_g(x)] dx 
