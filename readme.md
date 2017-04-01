# Quora Question Pairs

[Competition Homepage](https://www.kaggle.com/c/quora-question-pairs)

### Description

Where else but Quora can a physicist help a chef with a math problem and get cooking tips in return? Quora is a place to gain and share knowledge—about anything. It’s a platform to ask questions and connect with people who contribute unique insights and quality answers. This empowers people to learn from each other and to better understand the world.

Over 100 million people visit Quora every month, so it's no surprise that many people ask similarly worded questions. Multiple questions with the same intent can cause seekers to spend more time finding the best answer to their question, and make writers feel they need to answer multiple versions of the same question. Quora values canonical questions because they provide a better experience to active seekers and writers, and offer more value to both of these groups in the long term.

Currently, Quora uses a Random Forest model to identify duplicate questions. In this competition, Kagglers are challenged to tackle this natural language processing problem by applying advanced techniques to classify whether question pairs are duplicates or not. Doing so will make it easier to find high quality answers to questions resulting in an improved experience for Quora writers, seekers, and readers.

### Evaluation

Submissions are evaluated on the log loss between the predicted values and the ground truth.

### Submission File

For each ID in the test set, you must predict the probability that the questions are duplicates (a number between 0 and 1). The file should contain a header and have the following format:

```
test_id,is_duplicate
0,0.5
1,0.4
2,0.9
etc.
```