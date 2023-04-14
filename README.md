# Project for AI course
> Master degree in Computer Engineering, Cybersecurity and Artificial Intelligence - University of Cagliari

> **Authors**: [Nicola Deidda](https://github.com/MrDeiv) and [Luca Minnei](https://github.com/minn3)

## Requests
1) Remove stop words and punctuation from every document

2) Apply stemming to every remaining word in every document

3) Apply 5-fold cross-validation on the data set: randomly subdivide it into 5 disjoint subsets of identical size and repeate the steps below for each of the 5 training folds (made up of four subsets) and corresponding testing folds (the remaining subset):

- extract the set of all distinct words from the training fold, and compute the discriminant capability of each word using, for instance, the Information Gain measure defined in section 5.4.2 of the attached paper; then select the first N words as features (you can try different values for N in distinct experiments, for comparison, e.g., N = 100, 500, 1000)

- compute a N-dimensional feature vector for every document in the training and testing folds, e.g., as the word occurrence (1 if a word is present in the email body, 0 otherwise), frequency, or TF-IDF (see the attached paper): you can choose one kind of feature, or maybe use and compare them all

- train a classifier on the training fold, and compute the number of misclassifications on the corresponding testing fold

4) finally, estimate the misclassification rate as the sum of the number of misclassified documents in the 5 testing folds, divided by the overall number of documents

## Dataset
https://scikit-learn.org/0.19/datasets/twenty_newsgroups.html

## Documentation
See the notebook
