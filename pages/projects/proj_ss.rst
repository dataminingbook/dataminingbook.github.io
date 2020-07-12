.. title: Sequence Support 
.. slug: proj_ss
.. date: 2020-07-12 11:30:54 UTC-04:00
.. tags: 
.. category: 
.. link: 
.. description: 
.. has_math: True
.. type: text

Your goal here is to write a program that obtains the support of a list of sequences, in a sequence database. 

The program should take as input the following two files:

* FILE1: A list of sequences (one per line) that comprise the
  dataset. See the file: `<sequencedb.txt>`_. Lines beginning with '>' are comments, but serve to demarcate one sequence from the next. You may assume that the alphabet will remain :math:`\Sigma = \{A,C,G,T\}`.

* FILE2: A list of substrings (one per line), i.e., consecutive subsequences, whose supports have to be computed. See the file: `<seqin.txt>`_. 

Your program should output for each sequence in FILE2 the following info:

sequence - support
