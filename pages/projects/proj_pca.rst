.. title: Principal Component Analysis
.. slug: proj_pca
.. date: 2020-07-12 11:30:54 UTC-04:00
.. tags: 
.. category: 
.. link: 
.. description: 
.. has_math: True
.. type: text

Download the datafile *magic04.data* from the `UCI Machine Learning
Repository
<https://archive.ics.uci.edu/ml/datasets/MAGIC+Gamma+Telescope>`_. The
dataset has 10 real attributes, and the last one is simply the class
label, which is categorical, and which you will ignore for this
assignment.  

Principal Component
======================

Compute the dominant eigenvalue and eigenvector of the covariance matrix
:math:`\mathbf{\Sigma}` via the power-iteration method. One can compute the
dominant eigen-vector/-value of the covariance matrix iteratively as
follows.

Let

.. math::
    \mathbf{x}_0 = \begin{pmatrix} 1 \\ 1\\ \vdots \\ 1 \end{pmatrix}

be the starting vector in :math:`R^d`, where :math:`d=10` is the number of
dimensions. 

In each iteration :math:`i`, we compute the new vector: 

.. math::
    \mathbf{x}_i = \mathbf{\Sigma} \; \mathbf{x}_{i-1}

We then find the element of :math:`\mathbf{x}_i` that  has the maximum
absolute value, say at index :math:`m`. For the next round, to avoid
numerical issues with large values, we re-scale :math:`\mathbf{x}_i` by
dividing all elements by :math:`x_{im}`, so that the largest value is always
1 before we begin the  next  iteration.
 
To test convergence, you may compute the norm of the difference between
the scaled vectors from the current iteration and the previous one, and
you can stop if this norm falls below some threshold, say 0.0001. That
is, stop if 

.. math::
    \|\mathbf{x}_i - \mathbf{x}_{i-1}\| < 0.0001 
    
For the
final eigen-vector, make sure to normalize it, so that it has unit
length. Also, the ratio :math:`\frac{x_{im}}{x_{i-1,m}}` gives you the
largest eigenvalue.

First Two Principal Components
================================

Now compute the first two principal components (PCs) of the covariance
matrix :math:`\mathbf{\Sigma}` using a generalization of the above iterative
method. 

Let :math:`\mathbf{X}_0` be a :math:`d \times 2` matrix with two non-zero column
vectors of length :math:`d`, with unit length.  We will iteratively multiply
:math:`\mathbf{X}_0` with :math:`\mathbf{\Sigma}` on the left.

The first column will not be modified, but the second column will be
orthogonalized with respect to the first one by subtracting its
projection along the first column (see section 1.3.3 in chapter 1). That
is, let :math:`\mathbf{a}` and :math:`\mathbf{b}` denote the first and second
column of :math:`\mathbf{X}_1`, where 

.. math::
    \mathbf{X}_1 = \mathbf{\Sigma} \; \mathbf{X}_0

Then we orthogonalize :math:`\mathbf{b}` as follows: 

.. math::
    \mathbf{b} = \mathbf{b} - \left({\mathbf{b}^T \mathbf{a} \over \mathbf{a}^T\mathbf{a}}\right) \mathbf{a}

After this :math:`\mathbf{b}` is guaranteed to be orthogonal to
:math:`\mathbf{a}`. This will yield the final matrix :math:`\mathbf{X}_1` with
the two column vectors denoting the current estimates for the first and
second eigenvectors (or the principal components). Before the next
iteration, normalize each column to be unit length, and repeat the whole
process. That is, from :math:`\mathbf{X}_1` obtain :math:`\mathbf{X}_2` and so
on, until convergence.

To test for convergence,
you can look at the total absolute difference between
:math:`\mathbf{X}_{i}` and :math:`\mathbf{X}_{i-1}`. If the difference is less than some
threshold, use :math:`\epsilon=0.001`, then we stop.

Once you have obtained the two principal components: :math:`\mathbf{u}_1` and  :math:`\mathbf{u}_2`,
project each of the original points :math:`\mathbf{x}_i` onto those two vectors, to obtain the new
projected points in 2D (see *Eq. (7.6)*). Plot these projected points in the two PC dimensions. 



