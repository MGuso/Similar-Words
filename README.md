# Similar Words
With a word as an input, this algorithm returns a list of the most similar words to it using AI

This code contains an algorithm that searches for the most similar words to a specified word. To achieve this, the specified word is projected to a vector using the tokenizer of the NLP model GPT2. Once the vector of the first word is obtained, the same procedure is applied to get the vectors of the 50,000 (arbitrary value) most common words in the English language. Then, the vector of the specified word is compared to every vector of the set of words using the cosine similarity. Sorting the set of words by the value of the result of this operation, by a descending order, a list of the most similar words is obtained. Finally, the algorithm returns a dataframe with that list.
