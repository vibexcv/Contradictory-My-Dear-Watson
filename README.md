# Contradictory-My-Dear-Watson
Kaggle Competition: https://www.kaggle.com/competitions/contradictory-my-dear-watson


# Description from Kaggle:
Our brains process the meaning of a sentence like this rather quickly.

We're able to surmise:

    Some things to be true: "You can find the right answer through the process of elimination.”
    Others that may have truth: "Ideas that are improbable are not impossible!"
    And some claims are clearly contradictory: "Things that you have ruled out as impossible are where the truth lies."

Natural language processing (NLP) has grown increasingly elaborate over the past few years. Machine learning models tackle question answering, text extraction, sentence generation, and many other complex tasks. But, can machines determine the relationships between sentences, or is that still left to humans? If NLP can be applied between sentences, this could have profound implications for fact-checking, identifying fake news, analyzing text, and much more.
The Challenge:

If you have two sentences, there are three ways they could be related: one could entail the other, one could contradict the other, or they could be unrelated. Natural Language Inferencing (NLI) is a popular NLP problem that involves determining how pairs of sentences (consisting of a premise and a hypothesis) are related.

Your task is to create an NLI model that assigns labels of 0, 1, or 2 (corresponding to entailment, neutral, and contradiction) to pairs of premises and hypotheses. To make things more interesting, the train and test set include text in fifteen different languages! You can find more details on the dataset by reviewing the Data page.

Evaluation
Goal

Your goal is to predict whether a given hypothesis is related to its premise by contradiction, entailment, or whether neither of those is true (neutral).
For each sample in the test set, you must predict a 0, 1, or 2 value for the variable.

Those values map to the logical condition as:

    0 == entailment
    1 == neutral
    2 == contradiction

Metric

Your score is the percentage of relationships you correctly predict. This is known as accuracy.
Submission File Format

You should submit a csv file with exactly 5195 entries plus a header row. Your submission will show an error if you have extra columns (beyond id and prediction) or rows.

The file should have exactly 2 columns:

    id (sorted in any order)
    prediction (contains your predictions: 0 for entailment, 1 for neutral, 2 for contradiction)
