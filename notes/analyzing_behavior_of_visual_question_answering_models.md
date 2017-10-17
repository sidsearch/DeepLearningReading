Summary:
What is this paper about?
This is a paper proposes systematic methods for analyzing visual question answering models. It mainly analyzes two main types of models (1) with attention (2) without attention. It also analyzes VQA challenge winner of 2016.
What is the main contribution?

The major contribution of this paper is novel techniques to analyze VQA models. They analyze two models with and without attentions. This is the first paper analyzing these techniques to get better understanding of the methods.The analysis shows that models are myopic and often jump to conclusion and stubborn(do not change across images).

Describe the main approach & results. Just facts, no opinions yet.

Authors analyze the models in 3 different dimension 
Generalization to novel instances:  
Complete question understanding: 
Complete image understanding:


Models analyzed : CNN+LSTM,CNN+LSTM+attention,MCB

In results of this analsis authors find that VQA models are myopic, often "jump to conclusion" and stubborn. The models with attention are less stubborn where stubborn means that models do not change their answers. The authors also report that since models are training to minimize MLE they capture statistics of the dataset. This tells that the models are doing what the data and optimiztion tell it do. Hence designing new models require new way of modeling compositionality.



Strengths:
This is a very key paper in improving VQA models since understanding the performance of these models can lead to more deeper understanding of why some of the models do not work. The paper is well written and easy to understand. It introduces diffrent key concepts which can be improved to really achieve good general performance in visual question answering tasks. 

Authors report very interesting numbers on how many cases the model fails and why it fails.

Weaknesses:
Although, authors identify key weaknesses of these models they don't tell how these weaknesses can be overcome. Some hint or idea how to overcome these shortcomings of the VQA model can be really helpful. Although it can be argued that it is left for the community to figure it out.

Reflections:

This paper is directly related to the last few papers analyzed in the class where we read about different models for VQA tasks. This paper sets up the ground for next generation of vqa models. Also with VQA-CP and c-VQA dataset the newer models will tested against harder benchmark. The authors identify heavy language prior embedded in these models where the models really do not look at the image. They show that models get same answers for many images while they are totally different.


Most interesting thought: 

I think identification of language prior being heavily used in these model is one of the most improtant discovery. I would like to use models like Dynamic memory network or relation network which are designed for modeling relational tasks. Also, somehow blocking the language prior being passed the final is a key things. If the model can attend the image well and use that information along with the language information(by forcing hte model to use both of these information) that can lead to improved performance.
