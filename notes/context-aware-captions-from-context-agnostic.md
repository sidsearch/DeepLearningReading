# Context aware image captioning method 

What is this paper about?
This paper proposes method which uses a new method to get image captions using context
1. Justification: This task explain why the image belongs to the target class. For example given an image of bird, target class gree, distractor class red, the method exolains why it bebelongs in the target class.
2. Discriminative image captioning : This task identifies a target image given two images.  


What is the main contribution?
1. This paper provides a novel inference method which uses introspective speaker(IS) allowing speaker(S) to reason about pragmatic behavior without additional training.
2. It  proposes 2 new tasks (a) justification (b) discriminative image captioining 
3. It also proposes a new dataset(CUB-justify) to evaluate justification systems

Describe the main approach & results. Just facts, no opinions yet.
(1) Reasoning Speaker:
   goals of RS is to select utterences which are good sentences as per the generative model p and are discriminative per f 
 -  RS(I, c_t, c_d) = arg max \lambda p(s|I, c_t) + (1-lambda) f(s,c_t,c_d)
 
(2) Introspective Speker: (3) Emitter-Suppresor Beam Search for RNNs
 
(4) Experimental results: The proposed method achieves competitive performance on CIDEr-D and METEOR evaluation metrics.


Strengths:
1. In this papers, authors show that using a context-aware method we can further improve the captioning models. It also provides better justification.
2. One of the strength is the new dataset which can be further used to develop new context-aware image captioing models. This lays the ground for future mdoel development which are context-aware
3. The introduction of the new tasks (a) justification can be used judge the justification of the model's sentence generation 
				     (b) discriminative image captioning task will lead to model development which are better suited for discriminative tasks
4. The experiments are well explained and detailed. 

Weakness:
1. Code or dataset(CUB-justify) is not available online although authors say that they will provide these artifacts.
2. Quality of writing is not very clear. Especially, the overall picture of the paper was not super clear in an easy manner.

Reflections:
This is an interesting line of work compared to other image captioning papers discussed in class as it explores justification and discrimination of the target context and class in detail. I would be interested in applying some knowledgebase with the memory modules to create justification for the image captions generated. I think, trying a modular approach which might not be end to end could also be interesting.

Most interesting thought regarding the paper
I think, there are two primarily intersting direction associated with this work. (1) creatiom of new dataset and creation of new tasks for image captioning which will lead to more interpretable models in image captioning domain (2) This also leads the work of integrating reasoning and visual grounding with image captioning models.




 
