# ID2214-Fx-assignment
Fx assignment for ID2241 (Programming for Data Science) at KTH

Assignment:

You are requested to answer each of the two theoretical questions below by means of simulations/tests using a Jupyter notebook. You may employ real datasets and learning algorithms, e.g., as implemented in scikit-learn, or use synthetic classifiers/predictions/data, e.g., output by some random functions. You may use NumPy, pandas, scikit-learn and SciPy (send a request to professor in case you would like to use any other package).

You are expected to submit one notebook, clearly separating the two tasks, with extensive comments explaining the assumptions and conclusions.

1a. Methodology

Assume that we want to compare a new algorithm to a baseline
algorithm, for some classification task. As we are not sure what
hyper-parameter settings to use for the new algorithm, we will
investigate 100 different settings for that, while we use a standard
hyper-parameter setting for the baseline algorithm. We first randomly
split a given dataset into two equal-sized halves; one for model
building and one for testing. We then employ 10-fold cross-validation
using the first half of the data, measuring the accuracy of each model
generated from an algorithm and hyper-parameter setting. Assume that
the best performing hyper-parameter setting for the new algorithm
results in a higher (cross-validation) accuracy than the baseline
algorithm. Should we expect to see the same relative performance,
i.e., the new algorithm (with the best-performing hyper-parameter
setting) outperforming the baseline (with the standard hyper-parameter
setting), when the two models (trained on the entire first half) are
evaluated on the second half of the data?

1b. Performance metrics,

Assume that we have evaluated a binary classification model on a test
set with 5000 instances; 4000 belonging to the majority class and 1000
to the minority class. Assume that we have measured the accuracy and
AUC, and also observed a much higher precision for the majority class
than for the minority class. If we would evaluate the model on a
class-balanced test set, which has been obtained from the first by
keeping all instances from the minority class and sampling (without
replacement) 1000 instances from the majority class, should we expect
to see about the same accuracy and AUC as previously observed?
