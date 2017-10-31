t is this paper about?
    - This paper presents an approach to differentiate between visual and non-visual questions and if the question is visual then we determine if the question is relevant to the image or not.
      - What is the main contribution?
          - The paper presents a method for studying three types question-image pairs: 
                - Non visual : questions which are not related image at all
                      - Visual False-premise: these questions are visual but not related to the given image
                            - Visual True- premise: these question are related to the image.
                                - The paper introduces datasets and methods to recognize false-premise and non-visual question image pairs.  For visual, non-visual questions authors use LSTM trained on POS tags to capture visual specific linguistic structure.
                                    - Model achieves 92% for detecting non-visual and 74% for detecting false-premise questions which out performs baselines.
                                      - Describe the main approach & results. Just facts, no opinions yet.
                                          - Main approach:
                                                - Authors propose LSTM based model. The input for LSTM embeddings of POS tags of words. Embeddings of POS tags are learnt end to end. 
                                                      - For 2nd task for detecting whether a question Q entails a false-premise for image I.
                                                              - vqa uncertainity
                                                                        - vqa-mlp
                                                                                  - entropy
                                                                                          - pre contained captioning models
                                                                                                    - Question-caption similarity(QC sim) 
                                                                                                              - Question-Question Similarity
                                                                                                                  - Model achieves 92% for detecting non-visual and 74% for detecting false-premise questions which out performs baselines.
                                                                                                                  - Strengths:
                                                                                                                    - The paper is well written and easy to understand
                                                                                                                      - Authors propose a solution for very important problem in visual question answering which leads towards better answers since a lot vqa models do not understand the questions that well. 
                                                                                                                        - The discriminative task of identifying visual  and non-visual questions which are related to the image are modular approach which can be taken to improve the vqa models.
                                                                                                                          - The new dataset and different tasks will also lead to more publication in these areas to improve the quality of vqa models.
                                                                                                                          - Weaknesses:
                                                                                                                            - Authors do not compare some of the other known baselines for this task.  
                                                                                                                              - ???
                                                                                                                              - Reflections:
                                                                                                                                This paper is related to the lat few papers discussed in the class about different weaknesses of vqa models where models do not look at the image well. In this paper authors propose methods to understand the question and image relationship, identify visual, non-visual questions to improve the performance of vqa models.

                                                                                                                                Most interesting thought

                                                                                                                                  - I think this is very interesting line of work where we make the VQA models modular and try to get more better understanding of the model.  I would like to try the combination of these models with some of the other newer models such dynamic memory network  or relation network. Also combining these ideas with
