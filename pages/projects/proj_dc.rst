.. title: Density Clustering 
.. slug: proj_dc
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

Write a script to implement the DENCLUE density-based clustering
algorithm Algorithm 15.2 in chapter 15.  The script should take as input
a dataset :math:`\mathbf{D}`, the minimum density :math:`\xi`, the tolerance for
convergence :math:`\epsilon`, and the width :math:`h`. Do not make any
assumptions about the data (i.e., column names, etc), except that the
last column gives the "true" cluster id.

Run your script on the iris dataset, with :math:`\epsilon=0.0001`. Your
script should output the following:

* The number of clusters, and the size of each cluster
* The density attractor, followed by the set of point in that cluster.
* Purity of the clustering, based on the true id.

For Iris, you should use a value of :math:`\xi` that gives you 3 clusters in
the end, i.e., try different values and then finally report only the
results for the value that gives you 3 clusters, since there are 3 true
clusters in the data. Select the value of :math:`h` empirically.

To speed up the computation for estimating the density at a point, you
may want to first identify the K nearest neighbors, and use only those
neighbors. 

