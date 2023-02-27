# embedding_openai_gpt3
Observations
- using ada model from openai improves answers compared to basic model from transformers
- hallucinations by model can be effectively reduced by prompt engineering

Improvements
- I used top 10 similar results to user query, but we can experiment with a bigger number to improve context for model
- a bigger knowledge base can be used to enrich the contexts provided
- metrics other than cosine similarity can be experimented to evaluate similarity
- models with bigger embedding size can be used to enhance embeddings
- use other text generation models 

Possible alternatives to this approach
- we can finetune gpt3 for this specific task but that gets expensive as data size increases and time-consuming
- I would also research and add a way to evaluate generated responses to actual facts related to the task, 
   as hallucinations can prove fatal in some domains e.g medical
