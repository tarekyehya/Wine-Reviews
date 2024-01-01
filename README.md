# Wine-Reviews
business statement : Knowing the quality from the view of the customers based their reviews and information about the product.
Problem Statement: Predict score (score) based on some numeric feature like price, category features like interruption, and one text feature (drink description)

Dataset: Wine Review A large collection of reviews from experts in wine drinkers, each person drinks and describes the wine and the selection points are based on how good the drink is.

Solution:
Challenges : we have a Text features and the non-text features only get bad results.
my approach was how to make the best income from all features.
In about 7 notebooks, start exploring, cleaning up, build a basic model on non-text-only features.
then build model based on BOW features ( extracted from the reviews ) and tuning using tf-idf, n-gram parsers and analyzar.
then build a model based on a combination of numeric, categorical, and BOW features ( text and non text features ).
then build a model based on word2vec ( we used word2vec in representing the sentences ).
then build a model based on a combination of word2vec and BOW.
I’m going to use keras to build a deep learning solution to see which works best.
I have used custom column transformer and pipeline heavily
