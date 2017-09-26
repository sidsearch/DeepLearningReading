#Visual Question Answering
Summary:
What is this paper about?
This paper proposes the visual question answering task. The task is to have an image and question pair to get an answer if asked a natural language question. The goal is to understand the image and underlying context to answer a question.

What is the main contribution?
1. A dataset whcih has 0.25M images, 0.76M questions, 10M answers. 
2. Benchmarks and methods for VQA are also compared with human performance

Describe the main approach & results. Just facts, no opinions yet.
1.One of the primary contribution of this work is the visual qa dataset. 
2. An interface was designed to collect questions about the images. Subjects also provide the answers for the questions.
3. A detailed analysis of the dataset was presented which helps understand the composition of the questins and answers with images. Thus helping to understand the task better.

Strengths:
1. The main strength of the paper is the nicely curated dataset which can set the environment for a lot of consecutive work.
2. The paper is very well written and easy to understand
3. The authors also provide a lot of benchmarks which can be used to get started with the vqa task.
4. Usually the code and demo are also available.

Weaknesses:
1. The primary weakness of the paper is the split of the dataset. These weaknesses have been addresses in later papers from the same authors with vqa-cp and c-vqa datasets.
Because of the split of the dataset, sometimes it becomes easier for the model to encode language prior in the model which leads to good performance but the model actually
 does not understand the image well. So in order to develop truly intelligent systems or systems which can reason dataset split needs to better.

Reflections:
This paper leads to a lot of new research in the direction of vqa. There has been a lot of developement in the past few years in this area. There are also many new datasets which try to 
overcome the limitations of the dataset. While the dataset has limitations it was able to set the path for developement of a lot of new methods and innovations.

Most interesting thought: Describe what you believe is your most insightful thought about the paper. It could be next research directions in this line of work, (directly or indirectly related) new ideas that this paper gave you, things that you would be curious to try, connections you've made to other work, etc.

I think the authors have done a great service to the community by providing with this amazing dataset and the task. This has already led the path of development of many new models and methods in the 
world of visual question answering.
