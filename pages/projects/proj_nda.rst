.. title: Numeric Data Analysis
.. slug: proj_nda
.. date: 2020-07-12 11:30:54 UTC-04:00
.. tags: 
.. category: 
.. link: 
.. description: 
.. type: text

Download the *magic04.data* data file from the `UCI ML Repository
<https://archive.ics.uci.edu/ml/datasets/MAGIC+Gamma+Telescope>`_. The
dataset has 10 real attributes, and the last one is simply the class
label, which is categorical, and which you will ignore for this
assignment. Assume that attributes are numbered starting from 0. 

Write a script to answer the following questions. 

#. Compute the multivariate mean vector

#. Compute the sample covariance matrix  as inner products between the
   columns of the centered data matrix (see **Eq. (2.38)** in chapter
   2). 

#. Compute the sample covariance matrix  as outer product between the
   centered data points (see **Eq. (2.39)** in chapter 2)

#. Compute the correlation between Attributes 1 and 2 by computing the
   cosine of the angle between the centered attribute vectors. Plot the
   scatter plot between these two attributes.

#. Assuming that Attribute 1 is normally distributed, plot its
   probability density function.

#. Which attribute has the largest variance, and which attribute has the
   smallest variance? Print these values. 

#. Which pair of attributes has the largest covariance, and which pair
   of attributes has the smallest covariance? Print these values.
