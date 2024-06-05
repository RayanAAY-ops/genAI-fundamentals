# Steps
ask a question : convert into embedding using openai API
search into an index: to look for the NN thanks to FAISS
pass those NN into a prompt
provide a prompt to the LLM
Get an answer to the user.


In summary, we can  augment our LLM with an index of our choice, by converting the index as retriever. We can parametrize the retriever by using some parameters:
['fetch_k'] = number of vectors retrieved from the index.
['mmr'] = diversify the information
['k'] = number of context vector provided to the LLM

