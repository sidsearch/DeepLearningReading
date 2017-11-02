Visual Dialog

- Summary:
  - What is this paper about?
  - This paper introduces a new task called visual dialog which about an AI agent to have a meaningful conversation with humans about visual content.
  - What is the main contribution?
    - This paper proposes a new AI task where machine must hod a conversation with human about visual content.
    - Authors curate novel two person chat data collection protocol to curate large scale visual dialog dataset. VisDial.
    - Authors introduce a family of neural encoder-decoder models for visual dialog with 3 novel encoders
      - Late fusion:
      - Hierarchical Recurrent Encoder:
      - Memory Network:
    - Authors also propose retrieval-based evaluation protocol for visual dialog where AI agent is asked to sort a list of candidate answers. 
  - Describe the main approach & results. Just facts, no opinions yet.
    - VisDial dataset:
      - This is the dataset collected by authors using AMT. This is collected on COCO dataset. questioner sees a blurred image instead of the caption. The conversation seeded with blurred images resulted in questions that was blob recognition. 
    - VisDial dataset analysis: VisDial has less visual priming bias. The question lengh is well distributed. In visdial answer set only 63% is covered by the top 1000 answers. It has interesting set of answers such as ‘I think so’, ‘I cant’ tell’ etc.
    - Neural visual dialog models:
- Strengths:
  - The authors present a new AI task which will lead to a lot of new direction in AI research. Overall this is a great direction for AI research. 
  - The visdial dataset will serve as one of the most important starting points for the visual dialog ai tasks.
  - The models presented in the paper also serve as starting point for many researchers in the domain of visual dialog ai task.
  
- Weaknesses:
  - The paper does not provide a lot of historical detail of developement of visual dialog task.
  - Authors do not present their model performance on other visual QA datasets. 
  - 
- Reflections:
    This paper is further advancement of the visual qa task where a model tries to find the answer for visual content. The paper is well written and model, data are available which makes it very easy to experiment with.

Most important thought

  I think using the visual dialog model for other tasks can be very interesting such dataset completion where the agents can help complete the dataset with human help. I think also experimenting the models presented in this paper with visual qa tasks could be interesting. In an other way around using a generative model to generate images when ai agents ask question can also be interesting task.

