.. title: Classification Assessment
.. slug: proj_ca
.. date: 2020-07-12 11:30:54 UTC-04:00
.. tags: 
.. category: 
.. link: 
.. description: 
.. has_math: True
.. type: text


Paired t-Test and Bayes Classifier
===================================

Download the datafile *iris.data* from the `UCI Machine Learning
Repository <https://archive.ics.uci.edu/ml/datasets/iris>`_. This has
five attributes with 150 instances. The last column of the data
is a categorical attribute for the class of Iris flower. 

In this assignment you will evaluate the performance of the Full Bayes
and Naive Bayes classifier on the iris dataset. 
You have to assess via the paired t-test whether the classifiers are
significantly different or not.

You will implement Algorithm 22.4 in chapter 22, except that instead of
the K-fold cross validation, use K rounds of bootstrap resampling (as
described in Algorithm 22.3:lines 1-4). For each bootstrap sample
:math:`\mathbf{D}_i` you need to learn the paramerers of the Bayes
classifiers -- full and naive -- and then test on :math:`\mathbf{D} \setminus
\mathbf{D}_i` and record the error rates. Finally tabulate the
difference in the performance of the full and naive Bayes classifier for
each round. From the difference values in each of the :math:`K` rounds
compute the :math:`z`-score value (line 9; Algorithm 22.4) and then test if
the two classifiers are different or not at :math:`\alpha=0.95` and
:math:`\alpha=0.99` confidence level. Use :math:`K=30`.

Note that the only difference between the full and naive Bayes
classifier is that the former uses the full covariance matrix, whereas
the latter uses a diagonal one.  

You should implement the Bayes classifiers on your own, but you may use
builtin functions to find out the critical values for the t-distribution
for a given confidence level :math:`\alpha`. *Note*: In python you will
find *scipy.stats* module useful for this; in R, you may use *qt*).

