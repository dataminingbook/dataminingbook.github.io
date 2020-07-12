.. title: Errata for First Edition
.. slug: errata_first
.. date: 2020-07-12 16:30:54 UTC-04:00
.. tags: 
.. category: 
.. link: 
.. description: 
.. has_math: True
.. type: text

This page contains the errata for the first edition. You can 
`contact us via email <contact@dataminingbook.info>`_ if you want to report any errors.


Chapter 1: Data Mining and Analysis
============================================================
* p4, Section 1.3, line 13: as linear combination ****should be**** as a linear combination

* p9, Example 1.3, 3rd line from end: :math:`(153)^{1/3}` **should be** :math:`(152)^{1/3}`

* p9, Example 1.3, last line: :math:`(4^3 + (-1)^3)^{1/3} = (63)^{1/3} = 3.98` **should be** :math:`(4^3 + |-1|^3)^{1/3} = (65)^{1/3} = 4.02`

* p24, Section 1.4.3, last line of subsection Univariate Sample: 
  
  where :math:`f_\mathbf{X}` is the probability mass or density function for :math:`\mathbf{X}` 
  
  **should be** 
  
  where :math:`f_X` is the probability mass or density function for :math:`X`

* p30, Section 1.7, Q1: in (1.5) **should be** in Eq. (1.5)


Chapter 2: Numeric Attributes
============================================================

* p34, Equation (2.2): :math:`\hat{F}(x) \ge q` **should be** :math:`F(x) \ge q`

* p34, Line after Equation (2.2):

  That is, the inverse CDF gives the least value of :math:`X`, for which
  :math:`q` fraction of the values are higher, and :math:`1 − q`
  fraction of the values are lower.

  **should be**

  That is, the inverse CDF gives the least value of :math:`X`, for which
  :math:`q` fraction of the values are '''lower''', and :math:`1 − q`
  fraction of the values are '''higher'''.

* p53, Example 2.6, line 1: ... range for :math:`{\tt Income}` is :math:`2700-300=2400` **should be** ... range for :math:`{\tt Income}` is :math:`6000-300=5700`

* p55, In Eq (2.32): :math:`P(-k \le z \le k) = P\bigl(0 \le t \le k/\sqrt{2}\bigr)` **should be** :math:`P(-k \le z \le k) = 2 \cdot P\bigl(0 \le t \le k/\sqrt{2}\bigr)`

* p58, Total and Generalized Variance, Line 2: ...product of its eigenvectors **should be** ...product of its eigenvalues

* p58, two lines above Example 2.8: :math:`tr(\Lambda)` **should be** :math:`tr(\mathbf{\Lambda})`

* p61, Q3: :math:`mu` **should be** :math:`\mu` so that it reads

.. math::
    \sum_{i=1}^n (x_i - \mu)^2 = n(\hat{\mu} - \mu)^2 + \sum_{i=1}^n (x_i - \hat{\mu})^2


Chapter 3: Categorical Attributes
============================================================
* p81, Table 3.6, Attribute value for :math:`X_2`: :math:`{\tt Short} ( a_{23})` **should be** :math:`{\tt Long} ( a_{23})`


Chapter 4: Graph Data
============================================================
* p103, 2 lines above Eq (4.3): :math:`\gamma_{jk} = 0` **should be** :math:`\gamma_{jk}(v_i) = 0`

* p103, Eq (4.3): :math:`\gamma_{jk}` **should be** :math:`\gamma_{jk}(v_i)`

* p103, Example 4.5, last line: :math:`\gamma_{jk} > 0` **should be** :math:`\gamma_{jk}(v_5) > 0` 

* p104, Example 4.5:

  :math:`c(v_5) = \gamma_{18} + \gamma_{24} + \gamma_{27} + \gamma_{28} + \gamma_{38} + \gamma_{46} + \gamma_{48} + \gamma_{67} + \gamma_{68}`

  **should be**

  :math:`c(v_5)  = \gamma_{18}(v_5) + \gamma_{24}(v_5) + \gamma_{27}(v_5) + \gamma_{28}(v_5) + \gamma_{38}(v_5) + \gamma_{46}(v_5) + \gamma_{48}(v_5) + \gamma_{67}(v_5) + \gamma_{68}(v_5)`

* p107: :math:`\mathbf{p}_1 = \frac{1}{2} \pmatrix{1\\ 1\\ 2\\ 1\\ 2}` **should be** :math:`\mathbf{p}_1 = \frac{1}{2} \pmatrix{1\\ 2\\ 2\\ 1\\ 2}`

* p127, 4th Line after Eq (4.22): initial :math:`n_0` edges **should be** initial :math:`n_0` nodes

Chapter 5: Kernel Methods
============================================================
* p138, Example 5.4:

  :math:`\mathbf{\mu}_\phi = \sum_{i=1}^5 \phi(\mathbf{x}_i) =  \sum_{i=1}^5 \mathbf{x}_i` 
    
  **should be**

  :math:`\mathbf{\mu}_\phi = \frac{1}{5}\sum_{i=1}^5 \phi(\mathbf{x}_i) =  \frac{1}{5} \sum_{i=1}^5 \mathbf{x}_i`

* p140, 7th Line after Eq (5.3): :math:`\sum_{i=1}^{m_a} \sum_{j=1}^{m_a} \alpha_i \alpha_{\!j} K(\mathbf{x}_i, \mathbf{x})` **should be** :math:`\sum_{i=1}^{m_a} \sum_{j=1}^{m_a} \alpha_i \alpha_{\!j} K(\mathbf{x}_i, \mathbf{x}_j)`

* p141, 3rd line and 10th Line before Sec 5.1.2: There is an extra left bracket in definition of :math:`\phi(\mathbf{x})`, that is,
  
  :math:`\big( ( K(\mathbf{x}_1, \mathbf{x}), ...` **should be** :math:`\big( K(\mathbf{x}_1, \mathbf{x}), ...`

* p144, 2nd line: :math:`\int a(\mathbf{x})^2\; d\mathbf{x} < 0` **should be** :math:`\int a(\mathbf{x})^2\; d\mathbf{x} < \infty`

* p144, last line: :math:`\sum_{k=1}^q` **should be** :math:`\sum_{k=0}^q`

* p156, Section 5.4.2: all occurrences of path/paths **should be** walk/walks

* p160, Example 5.15L :math:`\mathbf{S} = -\mathbf{L} = \mathbf{A}-\mathbf{D}` **should be** :math:`\mathbf{S} = -\mathbf{L} = \mathbf{A}-\mathbf{\Delta}`

Chapter 6: High-dimensional Data
============================================================

* p164: In the definitions of the hyperball and and hypersphere

  :math:`\mathbf{x} = (x_1, x_2, \ldots, x_d)` **should be** :math:`\mathbf{x} = (x_1, x_2, \ldots, x_d)^T`


* p171: :math:`\mathbf{0}_d = (0_1,0_2,\ldots,0_d)` **should be** :math:`\mathbf{0}_d = (0_1,0_2,\ldots,0_d)^T`

* p172, Section 6.6, 1st Line after Eq. (6.11): 

  :math:`\mu` in equation :math:`\mu=\mathbf{0}_d` **should be** in bold.


* p178, section Volume in d dimensions:

  :math:`x_1 = r \cos\theta_1\cos\theta_2 \cos\theta_3 = r c_2 c_2 c_3` **should be** :math:`x_1 = r \cos\theta_1\cos\theta_2 \cos\theta_3 = r c_1 c_2 c_3`

  :math:`x_3 = r \cos\theta_1\sin\theta_2 = r c_1 s_1` **should be** :math:`x_3 = r \cos\theta_1\sin\theta_2 = r c_1 s_2`

* p178, Equation for :math:`J(\theta_1, \theta_2, \theta_3)`, Entry in first row, fourth column: :math:`r c_1 c_2 s_3`**should be** :math:`-r c_1 c_2 s_3`

* p207, line 3, Alg 7.2: :math:`\eta_1, \eta_2, ..., \eta_d` **should be** :math:`\eta_1, \eta_2, ..., \eta_n`

Chapter 7: Dimensionality Reduction
============================================================
* p186, line 1: :math:`\mathbf{a}_r` is vector **should be** :math:`\mathbf{a}_r` is a vector

* p207, line 3, Alg 7.2: :math:`\eta_1, \eta_2, ..., \eta_d` **should be** :math:`\eta_1, \eta_2, ..., \eta_n`

Chapter 8: Itemset Mining
============================================================
* p235, Example 8.13, 2nd last line: :math:`...,AB(3), AD(4),...` **should be** :math:`..., AB(4), AD(3), ...`

* p236, 5th line: :math:`...,AD(4),...` **should be** :math:`..., AD(3),...`

Chapter 9: Summarizing Itemsets
============================================================
* p250, 2nd line under '''Generalized Itemsets''': :math:`k`-tidsets **should be** :math:`k` tidsets

* p250, 4th line from bottom: :math:`Z = Y \setminus X` **should be** :math:`Z = X \setminus Y`

* p252, Eq. (9.3) and Eq. (9.4): :math:`\bigl|X\setminus Y\bigr|` **should be** :math:`\bigl|X\setminus W\bigr|` on the right hand side in both equations, so that they read

  :math:`\textbf{Upper Bounds} \bigl(\bigl|X\setminus Y\bigr| \text{is odd} \bigr): sup(X)  \leq\sum_{Y \subseteq W \subset X} -1^{\bigl(\bigl|X\setminus W\bigr|+1\bigr)} sup(W)`

  :math:`\textbf{Lower Bounds} \bigl(\bigl|X\setminus Y\bigr| \text{is even}\bigr): sup(X)  \geq\sum_{Y \subseteq W \subset X} -1^{\bigl(\bigl|X\setminus W\bigr|+1\bigr)} sup(W)`

* p254, Section '''Nonderivable Itemsets''', 1st Equation after line 1: :math:`\bigl|X\setminus Y\bigr|` **should be** :math:`\bigl|X\setminus W\bigr|` , so that it reads

  :math:`\mathit{IE}(Y) = \sum_{Y \subseteq W \subset X}\, -1^{\bigl(\bigl|X\setminus W\bigr|+1\bigr)} \cdot sup(W)`

Chapter 10: Sequence Mining
============================================================
* p264, alg 10.2, line 9: :math:`\mathbf{P}` **should be** :math:`P_a`

Chapter 11: Graph Pattern Mining
============================================================
* p288, sec 11.3, 2nd paragraph, line 6: :math:`sup(C) = sup(t)` **should be** :math:`sup(C') = sup(t)`

* p290, Figure 11.8: The last tuple in the DFS-code for graph :math:`C_{19}` **should be** :math:`\langle 2, 0, a, a \rangle` and not :math:`\langle 2, 0, a, b\rangle`

* p292, Algorithm 11.2, Line 14: :math:`b=\langle u_r, v, L(u_r), L(v), L(u_r, v)\rangle` **should be** :math:`b=\langle u_r, v, L(\phi(u_r)), L(\phi(v)), L(\phi(u_r),\phi(v))\rangle`

* p293, Figure 11.9 (c): There there **should be** one more extension for :math:`\phi_5`, namely :math:`\langle 0, 3, a, b\rangle`

* p294, Algorithm 11.3, Line 12: :math:`N_{G_j}` **should be** :math:`N_{G}`

* p295, Algorithm 11.4, Line 0: :math:`C` **should be** :math:`C = \{t_1, t_2, ..., t_k\}` 

Chapter 12: Pattern and Rule Assessment
============================================================
* p322 (Alg 12.1) and p326 (Alg 12.2): replace = with :math:`\gets`

Chapter 13: Representative-based Clustering
============================================================
* p343, in 3rd equation: :math:`P(C_i)` **should be** :math:`P(C_1)`
 
* p335, Algorithm 13.1, line 7: :math:`\mathbf{\mu}^t_i` **should be**  :math:`\mathbf{\mu}^{t-1}_i`

Chapter 14: Hierarchical Clustering
============================================================
* p366, Fig 14.2: (a) :math:`m=1`, (b) :math:`m=2`, and (c) :math:`m=3` **should be** (a) :math:`n=1`, (b) :math:`n=2`, and  (c) :math:`n=3`, respectively.

* p373, sec 14.4: EXERCISES AND PROJECTS **should be** EXERCISES

* p373, Q1, :math:`SMC(X_i, X_j)`, :math:`JC(X_i, X_j)`, :math:`RC(X_i, X_j)` **should be** :math:`SMC(\mathbf{x}_i, \mathbf{x}_j)`, :math:`JC(\mathbf{x}_i, \mathbf{x}_j)`, :math:`RC(\mathbf{x}_i, \mathbf{x}_j)`, respectively.

Chapter 15: Density-based Clustering
============================================================
* p385, line after Eq. (15.6): ... having two parts. A vector ...  **should be** ... having two parts: a vector ...

* p387, Alg 15.2, line 20: In the numerator :math:`K\left(\frac{\mathbf{x}_t - \mathbf{x}_i}{h} \right) \cdot \mathbf{x}_t` **should be** :math:`K\left(\frac{\mathbf{x}_t - \mathbf{x}_i}{h} \right) \cdot \mathbf{x}_i`

Chapter 16: Spectral and Graph Clustering
============================================================
* p411, 2nd last equation: :math:`\frac{1}{2}p_{rs}` **should be** :math:`p_{rs}` so that it reads 

  :math:`p_{rs} = \frac{d_r}{2m}\frac{d_s}{2m}  = \frac{d_r d_s}{4m^2}`

* p413, Line 5: :math:`\sum_{j=1}^n \mathbf{d}^T \mathbf{c}_i` **should be** :math:`\mathbf{d}^T \mathbf{c}_i`

* p413, Line 10: :math:`(\mathbf{d}_i^T\mathbf{c}_i)^2` **should be** :math:`(\mathbf{d}^T\mathbf{c}_i)^2`

* p424, Q5: :math:`\mathbf{c}_n = \frac{1}{\sqrt{n}} \mathbf{1}` **should be** :math:`\mathbf{c}_n = \frac{1}{\sqrt{\sum_{i=1}^n d_i}} \mathbf{\Delta}^{1/2}\mathbf{1}`

* p424, Q6 (b): :math:`\mathbf{K} = \mathbf{M}` **should be** :math:`\mathbf{K} = \mathbf{M} + \mathbf{I}`

Chaper 17: Clustering Validation
============================================================
* p428, Example 17.1, Table below 2nd para: :math:`n=100` **should be** :math:`n=150` for the total count

* p463, Q10: Add the sentence Assume that the clusters are: :math:`C_1 = \{a,b, c,d, e\}, C_2 = \{g, i\}, C_3 = \{f,h, j \}, C_4 = \{k\}`.

Chapter 18: Probabilistic Classification
============================================================
* p472, Table 18.2: 13/50 **should be** 11/50

* p472, Example 18.2, 2nd Para, lines 6 and 7: :math:`P(c_1|\mathbf{x})` and  :math:`P(c_2|\mathbf{x})` **should be** :math:`\hat{P}(c_1|\mathbf{x})` and  :math:`\hat{P}(c_2|\mathbf{x})`, respectively.

Chapter 20: Linear Discriminant Analysis
============================================================
* p503: Example 20.2: There **should be** no transpose operator :math:`T` on the mean vectors, i.e.,

  :math:`\mathbf{\mu}_1 = \pmatrix{5.01\\3.42}^T \qquad \mathbf{\mu}_2 = \pmatrix{6.26\\2.87}^T \qquad \mathbf{\mu}_1 - \mathbf{\mu}_2= \pmatrix{-1.256\\0.546}^T`

  **should be**

  :math:`\mathbf{\mu}_1 = \pmatrix{5.01\\3.42}  \qquad \mathbf{\mu}_2 = \pmatrix{6.26\\2.87} \qquad \mathbf{\mu}_1 - \mathbf{\mu}_2 = \pmatrix{-1.256\\0.546}`

* p509, Example 20.4, line 4: ''iris-virginica'' **should be** :math:`{\tt Iris\text{-}versicolor}`

* p512, Q1:  In part (a) :math:`\mathbf{S}_B` **should be** :math:`\mathbf{B}`, and in (b) :math:`\mathbf{S}_W` **should be** :math:`\mathbf{S}`


Chapter 21: Support Vector Machines
============================================================

* p526, 7th line, in :math:`L_{dual}`: :math:`(C - \alpha_i + \beta_i)` **should be** :math:`(C - \alpha_i - \beta_i)`

* p536, Algorithm 21.1, line 15: :math:`\mathbf{\alpha}_{t+1} = \alpha` **should be** :math:`\alpha_{t+1} \gets  \alpha`

* p538, Example 21.8, line 5: homogeneous quadratic kernel :math:`K(\mathbf{x}_i,\mathbf{x}_j) = ( \mathbf{x}^T_i \mathbf{x}_j)^2` **should be** inhomogeneous quadratic kernel :math:`K(\mathbf{x}_i,\mathbf{x}_j) = (1+ \mathbf{x}^T_i \mathbf{x}_j)^2`

