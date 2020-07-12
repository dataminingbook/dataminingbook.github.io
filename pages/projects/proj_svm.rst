.. title: Support Vector Machines 
.. slug: proj_svm
.. date: 2020-07-12 11:30:54 UTC-04:00
.. tags: 
.. category: 
.. link: 
.. description: 
.. has_math: True
.. type: text

Your goal is to learn a SVM in the traditional dual formulation for the
`<iris-slwc.txt>`_ dataset. This is a simple 2D dataset,
consisting of 2 dimensions (the sepal length and width), and the third
column is the class (+1,-1). One of the class corresponds to
iris-setosa, and the other class to other types of irises.

Implement the stochastic gradient ascent algorithm 21.1 in chapter 21,
with three different kernels, namely, the linear kernel, the
inhomogeneous quadratic kernel, and the homogeneous quadratic kernel.
Use :math:`\epsilon=0.0001` and :math:`C=10`, and hinge loss. 

At the end, print all values of non-zero :math:`\alpha_i`, i.e., for the
support vectors, in the following format:

:math:`i, \alpha_i` one per line

You should also print the number of support vectors.

Do this for both the kernels. The results on the linear kernel should
approximately match the hyperplane :math:`h_{10}` in example 21.7. 

To check when the quadratic kernel is useful. You may try the quadratic
kernel on the `<iris-PC.txt>`_ data. The results should match
those given in Example 21.8.
