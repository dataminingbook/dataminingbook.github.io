.. title: High Dimensional Analysis
.. slug: proj_hda
.. date: 2020-07-12 11:30:54 UTC-04:00
.. tags: 
.. category: 
.. link: 
.. description: 
.. has_math: true

High Dimensional Data Analysis
=====================================
Write a script to do the following:

*Hypersphere Volume*: Plot the volume of a unit hypersphere as a
function of dimension. Plot for :math:`d=1, \cdots, 50`. 

*Hypersphere Radius*: What value of radius would one need to
maintain a hypersphere volume of 1 with increasing $d$. Plot this value
for :math:`d = 1, \cdots, 100`.

*Nearest Neighbors*: Assume we have a unit hypercube centered at
:math:`(0.5, \cdots, 0.5)`. Generate $n=10000$ uniformly random points
in $d$ dimensions, in the range $(0,1)$ in each dimension. Find the
ratio of the nearest and farthest point from the center of the space.
Also store the actual distance of the nearest $d_n$ and farthest $d_f$
points from the center.  Plot these value for :math:`d = 1, \cdots,
100`.

*Fraction of Volume*: Assume we have a hypercube of edge length
$l=2$ centered at the origin :math:`(0,0, \cdots, 0)`. Generate
$n=10,000$ points uniformly at random for increasing dimensionality
:math:`d = 1, \cdots, 100`. Now answer the following questions:

* Plot the fraction of points that lie inside the largest hypersphere
  that can be inscribed inside the hypercube with increasing $d$. After
  how many dimensions does the fraction goes to essentially zero? 

* Plot the fraction of points in the thin shell of width :math:`\epsilon =
  0.01` inside the hypercube (i.e., the difference between the outer
  hypercube and inner hypercube, or the thin shell along the
  boundaries). What is the trend that you see? After how many dimensions
  does the fraction of volume in the thin shell go to 100% (use binary
  search or increase the dimenionality in steps of 10 to answer this.
  You may use maximum dimensions of upto 2000, and you may use a
  threshold of 0.0001 to count the volume as essentially being 1 in the
  shell, i.e., a volume of 0.9999 can be taken to be equal to 1 for
  finding the smallest dimension at which this happens).


Diagonals in High Dimensions
==================================

Your goal is the compute the empirical probability mass function (EPMF)
for the random variable $X$ that represents the angle (in degrees)
between any two diagonals in high dimensions.

Assume that there are $d$ primary dimensions (the standard axes in
cartesian coordinates), with each of them ranging from -1 to 1.  There
are $2^{d}$ additional half-diagonals in this space, one for each corner
of the $d$-dimensional hypercube.

Write a script that randomly generates $n=100000$ pairs of
half-diagonals in the $d$-dimensional hypercube, and computes the angle
between them (in degrees). 

Plot the EPMF for three different values of $d$, as follows
$d=10,100,1000$.  What is the min, max, value range, mean and variance
of $X$ for each value of $d$?

What would you have expected to have happened analytically? In other
words, derive formulas for what should happen to angle between
half-diagonals as :math:`d \to \infty`. Does the EPMF conform to this trend?
Explain why? or why not?

What is the expected number of occurrences of a given angle :math:`\theta`
between two half-diagonals, as a function of $d$ (the dimensionality)
and $n$ (the sample size)?
