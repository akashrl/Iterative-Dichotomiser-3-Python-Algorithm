#  ID3 (Iterative Dichotomiser 3) Algorithm

See ID3_Proj.pdf for full project and algorithm details.

This assignment was algorithm from scratch in **Python**. No model already implemented were used (like those in the scikit-learn library).

# Algorithm Details

**Visit the Wiki page:** https://en.wikipedia.org/wiki/ID3_algorithm

A binary decision tree with no pruning as well as post-pruning using the ID3 (Iterative Dichotomiser 3) algorithm was implemented. The attribute salaryLevel is the class value and the remaining 8 attributes in the data file are the input features for the decision tree.

The following are the commands needed to be run. matplotlib and tkinter were used for the plots.
- python3 ID3.py train.csv test.csv prune 70 30
- python3 ID3.py train.csv test.csv vanilla 70
- python3 plots_prune.py
- python3 plots_without_prune.py


# Input Format

The python script takes the following arguments:

1. train-file: path to the training set file. (adult.data)

2. test-file: path to the test set file. (adult.test)

3. model: model that you want to use. In this case, we will use:
− vanilla: the full decision tree.
− prune: the decision tree with post-pruning.

4. train-set-size: percentage of dataset used for training.

Each case may have some additional command-line arguments, which will be mentioned in
its format section. Use following examples to get the list of arguments.

The code reads the training set from train-file, extracts the required features, trains the decision tree on the training set, and tests it on the test set from test-file.
For debugging purposes, a small fraction of the dataset, for example, by using X[:100], was used to test with the first 100 data points.
