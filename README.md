# Forest cover type classification using AdaBoost

This paper implements AdaBoost, an incremental ensemble method that builds classifiers from decision stumps, from scratch, using nothing but NumPy and pandas.
The ensemble method is used to classify forest cover types based on the dataset from the Roosevelt National Forest in Colorado, available on Kaggle. Since AdaBoost is
a binary classifier, the algorithm is run for every type and the classifier selects the prediction that maximizes the binary classifier of the class. To evaluate the multiclass classification performance, we use cross validation with zero-one loss for different values of the number T of AdaBoost rounds.
