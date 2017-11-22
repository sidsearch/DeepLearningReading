
What is this paper about?

THis paper is about auto-annotation of image regions to labels.

Authrors propose a system for training the correspondence problem by exploiting additional language constructs to improve the learning process from weakly labeled data.consider both “prepositions” and “comparative adjectives” which
are used to express relationships between objects.  They simultaneously learn the visual features defining “nouns” and the differential visual features defining such binary-relationships using an expectation maximization model.

What is the main contribution?

1. It allows us to learn classifiers for a vocabulary of prepositions and comparative adjectives. These
classifiers are based on differential features extracted from pairs of regions in an
image.
2. This model allows simultaneous learning of nouns and relationships reduces correspondence ambiguity and leads to better learning performance.
3. It also shows that learning priors on relationships that exist between nouns constrains the annotation problem and
leads to better labeling and localization performance on the test dataset.


Describe the main approach & results. Just facts, no opinions yet.
1. The training model learns  
	a)classifiers for nouns and relationships at the same time.
	b)learns priors on possible relationships for pairs of nouns 
2. Uses weakly labeled data.
3. Dataset used: Core1kK
3. 850 training images with nouns and manually labeled relation
4. Uses sementation and features from Duygulu paper
4. Inference model is 100 images


Strength:
1. The paper is well written and easy to understand.
2. It was one of the early papers which provides ideas for scene undestanding with language constructs.
3. It provided methods which extended the visual classifiers for noun,prepositions and comparative adjectives.




Weakness:
1. The model is trainable end to end. It's known that at the time when the paper was published neural networks were not that  popular.
2. Although it learns spatial relationships, but these spatial relationships themselves were not considered outputs in their own right.

Reflections:
1. it is related to the earlier papers which we read in the classs.


Most interesting thought:

It would be interesting to model these tasks with deep learning. The task for learning models for categories or image segmentation has advanced a lot with deep learning. 