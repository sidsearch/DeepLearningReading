Summary:
What is this paper about?
The authors present a system  that can compute a score linking an image to a sentence. This score is used for used to attach a descriptive
sentence to a given image, or to obtain images that illustrate a given sentence.This score is obtained by comparing an estimate of meaning obtained from the image to the one from the sentence where the estimate comes from discriminative procedure learnt from data.

What is the main contribution?
1. Authors introduce a dataset to solve this problem.
2. Authors introduce a novel representation intermediate between images and sentences.
3. Authors present  novel, discriminative approach that produces very good results at sentence annotation.


Describe the main approach & results. Just facts, no opinions yet.

The proposed model assumes that there is a space of meanings that comes between the space of Sentences and the space of Images. 
Authors evaluate similarity between a sentence and an image by 
(a) mapping each to the meaning space then 
(b) comparing the results. 
The model leaarns the mapping from images  and resp. sentences to meaning discriminatively from pairs of images  and assigned meaning representations.

Meaning is represented as a triplet object, action, scene.
Authors use various image features such as Felzenszwalb detectors, Hoiem et al. classification responses, Gist-based scene classification responses.  
SVM is used a classifier to predict nodes. 
They represent a sentence by computing similarity between sentence and triplets.


Strengths:
This paper is very well written and easy to understand.
This work laid out some of the foundations for image captioning task which has been followed by many other papers in this area.

Weaknesses:
There has been many other works after this paper which improve upon this work such "show and tell neural caption generator". 
This paper was written before the deep learning resurgence happened in computer vision community.
It tries to use the solutions available to different subproblems related to image captioning to create solution, though it is not direct weakness in its own time.

This model is also not really end to end but this weakness has been further addressed.
Reflections:

This is related to some of the papers which read in the beginning of course about image captioning such as "Show and Tell: A Neural Image Caption Generator", "Knowing When to Look: Adaptive Attention via A Visual Sentinel for Image Captioning", "Context-aware Captions from Context-agnostic Supervision" etc. 


Most interesting thought:

I think image captioning is solved but not fully solved. There are further challenges building end to end models which somewhat attacked in "DenseCap: Fully Convolutional Localization Networks for Dense Captioning". But it is not clear if these models fully understand picture or not. I think there needs to more work where the image captioning models are trained with less data to understand if these models are compositional or not in nature.