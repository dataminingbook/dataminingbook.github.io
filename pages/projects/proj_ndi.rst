.. title: Non-Derivable Itemsets 
.. slug: proj_ndi
.. date: 2020-07-12 11:30:54 UTC-04:00
.. tags: 
.. category: 
.. link: 
.. description: 
.. has_math: True
.. type: text

Your goal here is to write a program to compute whether an itemset is derivable or not. The program should take as input the following two files:

* FILE1: A list of itemsets with their support values (one per line). See the file: `<itemsets.txt>`_ (the format is "itemset - support"; one per line)

* FILE2: A list of itemsets (one per line), whose support bounds have to be derived. See the file: `<ndi.txt>`_


Your program should output for each itemset in FILE2 the following
info:

itemset:     *[l,u]*      derivable/non-derivable 

where l and u are the lower and upper-bounds on the support. 

