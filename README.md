# MCQ-Model
This is a ipynb that can answer MCQ type questions with an accuracy of about 99%. 
This was created for the LLM Science competetion hosted by kaggle. The competetition wanted to create a model that can answer user's questions that can hopefully compete with models that can go upto 10 times its size.  My teammate Prasann(@Prasann2004(Github) ) and I devoted about 2 months in order to come up with this solution. We experimented with a large number of models like llama 7B,Deberta V3,Mistral 7B,etc, however due to technical limitations and lack of adequate amount of knowledge(as this was our first experience with LLMs) we weren't able to incorporate large models like Llama and Mistral. So we sticked to Deberta V3 models. 
The notebook uploaded uses ensemble of 6 models with weights computed using a self devised method. 

Our model makes use of RAG to gather information related to a question and answer on basis of that. 
![Science LLM](https://github.com/Nb4159/MCQ-Model/assets/122211644/1f537ab9-d6ce-4a7c-ae84-e800864a0230)

The notebook used for training the models is already provided in the repo. We trained 6 deberta models for this task:
1) https://huggingface.co/namban4123/Deberta_for_multiple_choice
2) https://huggingface.co/Prasann15479/LLM_Science_1
3) https://huggingface.co/namban4123/LLM_Model_Multiple_choice_questions
4) https://huggingface.co/Prasann15479/LLM_Science_1
5) https://huggingface.co/Prasann15479/LLM_Science_1
6) https://huggingface.co/namban4123/LLM_Science


The datasets we used for training our models are:
1) https://www.kaggle.com/competitions/kaggle-llm-science-exam/data
2) https://www.kaggle.com/datasets/mbanaei/all-paraphs-parsed-expanded
3) https://www.kaggle.com/datasets/cdeotte/40k-data-with-context-v2
4) https://www.kaggle.com/datasets/cdeotte/60k-data-with-context-v2

Also thanks to everyone on kaggle whose ideas and datasets helped us along the way and made it possible for us to deliver this model.
