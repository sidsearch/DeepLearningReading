
##Learn a function that maps input patterns into target space such that L1 norm in the target space approximates "semantic distance" in input space.
##Learning process minimizes a discriminative loss function that drives the similarity metric to be small for pairs of faces from the same person, and large for pairs from different person
## Architecture: Siamese network

* Given 2 inputs X1 and X1, find function G_W, parametrized by W, where similarity metric E_W(X1,X2) = || G_W(X1)- G_W(X2) || is small if X1, X2 belong to same category, and large if they belong to different categories
*  
