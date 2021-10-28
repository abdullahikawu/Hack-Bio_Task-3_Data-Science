# parkinsons_prediction
Model building to detect onset of Parkinson's disease

XGBClassifier uses a Gradient Boosting algorithm to build a classification model. Gradient boosting combines the outputs of many weak classifiers to produce a single, stronger one (one whose mean squared error is the smallest). A weak classifier, like a decision tree, is one in who error rate is at least slightly better than random guessing; each successive application is thought to correct the errors of its predecessor. In effect, the algorithm can be thought of as introducing a loss function and finding a local minimum of this function by iterating through each weak classifier.
