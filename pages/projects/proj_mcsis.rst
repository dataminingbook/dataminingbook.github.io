.. title: Monte Carlo Sampling for Itemset Support 
.. slug: proj_mcsis
.. date: 2020-07-12 11:30:54 UTC-04:00
.. tags: 
.. category: 
.. link: 
.. description: 
.. has_math: True
.. type: text

Look at the data file `<T10.txt>`_.  It contains one line per transaction, and each transaction is a list of items that appear in it. You are to use monte carlo sampling to find the relative support of the item set $X = \{39, 704, 825\}$, as follows:
 
* Write a program  to construct the sampling distribution of the relative support of $X$. Your program should draw 100 random samples of size 10,000 and compute the support of $X$ in each sample. Plot the sampling distribution of relative support of $X$.

* Based on the sampling distribution your program should compute the lower and upper bound for the support of $X$ at the 95% confidence level.
      
* Your program should find the mean and standard deviation of the possible relative  support values of $X$ in the samples, and compare the mean with the actual relative support of $X$ in the database.

* Either accept or reject the hypothesis that the true relative support of $X$ is 0.0106 at the 95% confidence level.

