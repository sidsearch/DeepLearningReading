Natural Language Does Not Emerge 'Naturally' in Multi-Agent Dialog

- What is this paper about?
    This paper is about the natural laguage emergence in multi agent dialog settings. It tells that  natural language does not emerge ‘naturally’, though  natural-language-emergence is present in  recent literature.
    - What is the main contribution?
      - The paer primarily asks the question "what are the conditions that lead to  the emergence of human-interpretable or compositional grounded language?". They find that natural language does not emerge ‘naturally’ in multi-agent dialog.
        - They mention that while agents talking to each other might while agents always successfully invent communication protocols  to achieve their goals with good accuracies, the invented languages are decidedly not compositional, interpretable, 
        - Describe the main approach & results. Just facts, no opinions yet.
          - Authors use a guessing game between two chatbots , q-bot and a-bot where they try to converse in natural language to find a cooperative setting to find the top similar image features. This is modelled as RL problem using REINFORCE algorithm.
            - Then they use series of settings where they find if the language compositional or not. They use these following different settings such as Overcomplete vacobulary, Attribute value vocabulary, Memoryless A-BOT: minimal vocab, Evolution of language to understnad the evolution of the language.
            - 
            - Strengths:
              - The paper is very well written and well presented. It presents some of the ground breaking ideas in emergence of language in visual dialog settings and dives very deep into it.
                - It will be very useful for the community to further explore the compositional nature of the language. 
                - Weaknesses:
                    I think the authors evaluate the task in an synethic data settings which might somewhat limiting to understand if it really scales well to larger dataset. While it may be argued that it is important to use synthetic data to really understand the task first, but authors could have given some example of dialouges using real dataset.
                    - Reflections:
                      - This is directly related last paper which we discussed in the class about visual dilouge task between two agents. This paper further advances the previous paper by analyzing the emergence of language in such settings.
                      - Most interesting thought: This paper presents a very interesting idea and evaluation of the language. I think it is important to take the task and further evaluate it in real world dataset instead of synthetic dataset. I think it is also important to think that if we model the agents differently would that lead to more interpretable agents in terms of more direct optimization.

