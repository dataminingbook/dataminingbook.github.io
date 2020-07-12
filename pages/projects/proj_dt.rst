.. title: Decision Trees 
.. slug: proj_dt
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

The goal of this part is to write a script to compute the decision tree
for an input dataset. You can assume that all attributes are numeric,
except for the last attribute which is the class. 

You should use the Information Gain based on Entropy for computing the
best split value for each attribute. For the stopping criteria at a
node, stop if the purity is at least 95% or stop if the node size is
five or lower.

Note that the best way to implement the splits for numeric attributes is
to sort the values of that attribute from smallest to largest. Then you
can use the mid-point between two distinct (consecutive) values as the
split test of the form :math:`A \le v`. You can then update the class
frequencies on both sides of the split and compute the split entropy for
each decision. After comparing with the entropy for the node, you can
find the best split for the current attribute. Now repeat the whole
process for each numeric attribute at that node, and choose the best
split over all attributes. Finally, split the data according to the best
split, and repeat the whole method recursively, until the stopping
conditions are met.

Your script should output the final decision tree using the format
described below. For example, for toy data below:

+-----+---------+-+------+
| Age | CarType | | Risk |
+=====+=========+=+======+
| 25  |    1    | |  L   |
+-----+---------+-+------+
| 20  |    3    | |  H   |
+-----+---------+-+------+
| 25  |    1    | |  L   |
+-----+---------+-+------+
| 45  |    2    | |  H   |
+-----+---------+-+------+
| 20  |    1    | |  H   |
+-----+---------+-+------+
| 25  |    2    | |  H   |
+-----+---------+-+------+

The decision tree should be printed in the following format:
::

    Decision: Car <= 1.5 , Gain= 0.4591479 
        Decision: Age <= 22.5 , Gain= 0.9182958 
            Leaf: label= H purity= 1 size= 1 
            Leaf: label= L purity= 1 size= 2 
        Leaf: label= H purity= 1 size= 3

Note that each internal node, print the decision followed by the
Information Gain, and for each leaf, print the majority label, purity of
the leaf, and the size. The indentation indicates the tree level. All
nodes at the same level of indentation (tabs) are at the same level in
the tree. For the tree above, :math:`Car <= 1.5` is the root decision. Its
left child is :math:`Age <= 22.5`, and its right child is a leaf. Also, for
:math:`Age \le 22.5` its left and right children appear immediately below
it. 

Test your program on the iris dataset.

