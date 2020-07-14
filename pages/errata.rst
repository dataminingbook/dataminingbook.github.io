.. title: Errata
.. slug: errata
.. date: 2020-07-08 16:30:54 UTC-04:00
.. tags: 
.. category: 
.. link: 
.. description: 
.. has_math: True
.. type: text

This page contains the errata for the second edition. You can 
`contact us via email <contact@dataminingbook.info>`_ if you want to report any errors.


Chapter 8
==========

* pg 230, fig 8.5: nodes labeled *AC, CD* and *BCD* should be shaded gray

* pg 232, fig 8.6: nodes labeled *AC, CD* and *BCD* should be shaded gray

Chapter 10
==========

* pg 265, fig 10.2: nodes labeled *C, AT, GT, TA, TG, AAA, AGA* and *AGG* should be shaded gray. Also, extensions of an infrequent pattern are not shown.

Chapter 12
==========

* pg 311, table 12.11: *conv* should be :math:`\infty` for row 1, since *conf* is 1

* pg 311, table 12.12: *conv* should be :math:`\infty` for rows 1 and 3, since *conf* is 1


Chapter 15
==========

* pg 377, Algorithm 15.1, Line 17: if :math:`\mathbf{y} \in Core`
  **should be** if :math:`\mathbf{y} \in Core` and :math:`id(\mathbf{y}) = \emptyset`

  This will prevent an infinite loop.

Chapter 22
==========

* pg 549, eq 22.7: :math:`\frac{1}{k} \sum_{i=1}^r F_i` **should be** :math:`\frac{1}{k} \sum_{i=1}^k F_i`
