Deep learning is relly hard to train. Authors present residual networks for east of training substantially deeper than earlier networks.

Empirical evidence tell that ResNet is easier to optimize and gain from increased depth. 152 layers, 8 times deeper than VGG.

ResNet formulates that, H(x) = F(x)-x can be asymptotically approximated by a stacked neural network, then instead of completely approximating F(x) by a stacked neural net, we divide that into multiple residual connections such (F(x) +x) to be approximated.

Formally a residual block can be formulated as y = F(x,W(i)) +x, where x,y are input, output layers and F(x,W(i)) is the residual mapping. The dimension of x and W must be same and when it is not same, the authors say that W(s) is used to project x to the same dimension of W(i)


