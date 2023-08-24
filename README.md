# Wine-Reviews

Problem Statement: Predict score (score) based on some numeric feature like price, category features like interruption, and one text feature (drink description)

Dataset: Wine Review A large collection of reviews from experts in wine drinkers, each person drinks and describes the wine and the selection points are based on how good the drink is.

Solution:
My approach is described in 5 steps:

Step 1: Exploration, argumentation, and basic model building is based on non-textual features only.

Drag step: create and set BOW, n-gram, word or char, tf-idf, model hyperparameters such as alpha in Lasso and Ridge, use mean squared error as a measure, and use column transformers and pipelines to make the case as simple as possible.

Third step: Combine the BOW model with the non-textual feature model by a custom column adapter and use the best hyperparameters of BOW from the last tuning.

The fourth step: build the send2vec model with word2vec. For a sentence, first represent a word with a vector, then average it to represent the sentence, and apply it to all sentences.
I used custom column and pipeline adapters to make everything as simple as possible.

Final step: combine word2vec with BOW, again with custom column adapters and pipelines.

The first steps I used the linear model, and the last step I set the gradient boost and random forest.


In most any cloud collections it doesn't come very close if you get a useful resource but I do follow my intuition and break everything down into very small problems.
