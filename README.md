# Naive_Bayes_Classifier
Examples is a set of text documents along with their target values. V is the set of all possible target values. This function learns the probability terms P(wk |vj,), describing the probability that a randomly drawn word from a document in class vj will be the English word wk. It also learns the class prior probabilities P(vj).

1.Collect all words, punctuation, and other tokens that occur in Examples
•	Vocabulary ← c the set of all distinct words and other tokens occurring in any text document from Examples

2.Calculate the required P(vj) and P(wk|vj) probability terms

•	For each target value vj in V do

•	docsj ← the subset of documents from Examples for which the target value is vj

•	P(vj) ← | docsj | / |Examples|

•	Textj ← a single document created by concatenating all members of docsj

•	n ← total number of distinct word positions in Textj

•	for each word wk in Vocabulary

•	nk ← number of times word wk occurs in Textj

•	P(wk|vj) ← ( nk + 1) / (n + | Vocabulary| )
