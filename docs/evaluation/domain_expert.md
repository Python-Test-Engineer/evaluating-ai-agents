# Professional Evaluation

The technique of an (untested) LLm generating question/answer pairs to act as ground truths to then test an LLM seems illogical but current thinking states this is quite effective.

At the end of the day, the final judge of the LLM is a human. 

A number of sets of questions can be made and the LLM evaluated against them by a domain expert.

Whilst a numerical rating system is the immediate choice, there are many flaws with this.

The domain expert can rate the repsonse for the following:

1. Accuracy. Is the answer factually correct?
2. Relevance. Is the answer relevant to the question?
3. Completeness. Is the answer complete?
4. Clarity. Is the answer clear?

Only those that get a YES to ACCURACY and RELEVANCE will be considered as they are essential for a good response.

This is a very effective way of evaluating the LLM and will help us to improve our system and will be modiofied in the future as needed.

### Example
![domain expert](../images/rag/evaluation_excel.png)