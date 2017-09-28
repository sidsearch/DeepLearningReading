Summary:
What is this paper about?
This paper presents a method to joint representation using multimodal compact bilinear pooling(MCB). The authors argue that just concatenating the visual and question representation does not create powerful enough expressive model. since outer product is infeasible due to higher dimensionality, author provide a MCB to get a joint representation.


What is the main contribution?
Bilinear pooling models were proposed  by Tenebaum. In this paper, authors adapt an idea from Gao et al to compress bilinear pooling for a single modality. Then they show the effectiveness of this representation.

Describe the main approach & results. Just facts, no opinions yet.

First we obtain image and text representation using CNN or other neural networks. Then MCB is obtained by randomly projecting the image and text representations to a higher dimensional space  and then convolving both vectors efficiently by using element-wise product in FFT space. Authors rely on  the Count Sketch projection by Charikar which projects  vector v[n dimensional real valued vector] to vector y[d dimensional real valued vector].This allows to project the outer product to a lower dimensional space, which reduces the number
of parameters. Authors also describe the architecture for vqa using MCB. In that setting the image representation obtained by resnet and question representation by lstm is passed through a MCB. After MCB pooling, a fully connected layer connects resulting multimodal representation to 3000 top answers.They aslo use soft attention on top of MCB. They report that this MCB based representation leads to higher performance. In the ablation studies they show that MCB pooling outperforms all other methods.



Strengths:
Authors use the idea from Tenebaum et al and Gao et al to get method to project multimodal representation to a lower dimensional space. The idea to project the representation to a lower dimensional space is a novel method.  The paper is well written and easier to follow. Authors have provided a good archicture diagram and pseudo code to get the model working.
The code for the model is also available which makes it easier to implement and modify the architecture.



Weaknesses:
Although the joint representation is a good method to jointly represent the visual and textual information, it does not indicate the model learns visually grounded question answering. Since it has been shown in the later paper such  "Don’t Just Assume; Look and Answer: Overcoming Priors for Visual Question Answering" by Agarwal et al this model does not perform that well on VQA-CP dataset which is compositional in nature. This indicates that the MCB model has the capacity to encode language priors in VQA tasks which results in lower performance in compositional datasets.


Reflections:
This is one of the best performing model for VQA task. Also this paper provides a method which is used to get better visually grounded models. This model also presents a method which can be extended to other related multimodal joint representation. 

Describe what you believe is your most insightful thought about the paper. It could be next research directions in this line of work, (directly or indirectly related) new ideas that this paper gave you, things that you would be curious to try, connections you've made to other work, etc.

I think combining MCB with co attention or stacked attention model might lead even higher performance for vqa and vqa-cp tasks. In this paper authors present an idea about combining MCB with attention which leads to better performance. Also, I am interested to know if the performance will go down or not while using VGGNet image representation since this paper used Resnet image representation. It will also to be interesting to try the representation.

It will also be intersting to combine the representation learned from this with realtion network.
 
