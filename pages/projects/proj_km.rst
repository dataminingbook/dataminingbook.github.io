.. title: Kernel Methods 
.. slug: proj_km
.. date: 2020-07-12 11:30:54 UTC-04:00
.. tags: 
.. category: 
.. link: 
.. description: 
.. has_math: true
.. type: text

Download the datafile *iris.data* from the `UCI Machine Learning
Repository <https://archive.ics.uci.edu/ml/datasets/iris>`_. This has
five attributes with 150 instances. Ignore the last column of the data,
which is a categorical attribute for the type of Iris flower. 

Kernel Feature Space
=======================

Compute the centered and normalized homogeneous quadratic kernel matrix
:math:`\mathbf{K}` for the iris dataset using the kernel
function in input space. 

Next, explicitly transform each point :math:`\mathbf{x}_i` to the feature space :math:`\phi(\mathbf{x}_i)`, using the homogeneous quadratic kernel. Center these points and normalize them. Finally verify that the pair-wise dot products of the centered and normalized points in feature space yield the same kernel matrix computed directly in input space via the kernel function. To do this, compute the matrix difference between the kernel matrices from the two approaches, and then print the sum of the differences.

Principal Components of Kernel Matrix
===========================================

Compute the principal components (PCs) of the centered and normalized
kernel matrix computed above. *Note*: in Python you may use
**numpy.linalg.eig**; in R you may use **eigen**.

How many components are required to capture 90% of the total variance? 

Project each of the original points/rows of :math:`\mathbf{K}` onto the
first two PCs and create a scatter plot of the projected points.  What
is the range of values in each PC dimension?
