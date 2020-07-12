.. title: Closed Itemset Mining 
.. slug: proj_cim
.. date: 2020-07-12 11:30:54 UTC-04:00
.. tags: 
.. category: 
.. link: 
.. description: 
.. has_math: true
.. type: text


Implement the CHARM algorithm for frequent closed itemset mining (see Algorithm 9.2 in chapter 9). Download the file `<mushroom.txt>`_ for your runs. Each line of the file contains a transaction, i.e., as set of items that occur together. The transactions do not have to be of the same length, but you may assume that each line will be sorted on the items.

Your script should accept the filename and minimum support value from the command line. It should be run as: ScriptName mushroom.txt MINSUP. Here MINSUP is in absolute numbers.

Your script should output all the frequent closed itemsets in the following format:

|
| closed itemset - support
|

with one itemset and its support per line. It should also print the total number of frequent closed itemsets on the last line of the output.

Run your code on mushroom.txt for two different values of minsup, namely minsup = 5000, and minsup = 3000, and record the output.

