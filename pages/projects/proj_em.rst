.. title: Expectation Maximization Clustering 
.. slug: proj_em
.. date: 2020-07-12 11:30:54 UTC-04:00
.. tags: 
.. category: 
.. link: 
.. description: 
.. has_math: True
.. type: text

Download the datafile *iris.data* from the `UCI Machine Learning
Repository <https://archive.ics.uci.edu/ml/datasets/iris>`_. This has
five attributes with 150 instances. The last column of the data 
is a categorical attribute for the type of Iris flower. 

Write a script that implements the Expectation-Maximization (EM)
algorithm for clustering (see Algorithm 13.3 in Chapter 13). Run the
code on the iris dataset. Use the first four attributes for clustering,
and use the labels only for the purity-based clustering evaluation (see
below). In your implementation, you should estimate the full covariance
matrix for each cluster. 

For EM initialization, use the first :math:`n/k` points for cluster 1,
the next :math:`n/k` for cluster 2, and so on. For convergence testing,
you can compare the sum of the euclidean distance between the old means
and the new means over the :math:`k` clusters. If this distance is less
than :math:`\epsilon=0.001` you can stop the method.

Your program output should consist of the following information:

#. The final mean for each cluster

#. The final covariance matrix for each cluster

#. Number of iterations the EM algorithm took to converge.

#. Final cluster assignment of all the points, where each point will be assigned to the cluster that yields the highest probability :math:`P(C_i|\mathbf{x}_j)` 

#. Final size of each cluster

Finally, you must compute the *purity score* for your clustering,
computed as follows: Assume that :math:`C_i` denotes the set of points
assigned to cluster :math:`i`  by the EM algorithm, and let :math:`T_i`
denote the true assignments of the points based on the last attribute.
Purity score is defined as:

.. math::
    Purity= \frac{1}{n} \sum_{i=1}^k max_{j=1}^k \{C_i  \cap T_j\}

