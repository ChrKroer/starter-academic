---
title: Reading List for my Research Group
date: 2019-07-12
math: true
diagram: true
---

In this post I collect a list of books that I recommend for getting up to speed on the most common types of math and optimization used in my research.

The first three sections are most directly related to my research. After that I give some suggestions on general CS, math, and programming background.

## Optimization

The following are my two favorite resources for getting started on various aspects of optimization:

* [Introduction to Linear Optimization](http://athenasc.com/linoptbook.html) by Bertsimas and Tsitsiklis.  Great starting point. Most other optimization topics rely on linear optimization results covered here. Chapters 1,2, and 4 are most important.
* [Convex Optimization](https://web.stanford.edu/~boyd/cvxbook/) by Boyd and Vandenberghe. An excellent book for getting started with more general convex optimization. Chapters 2-5, 9, and 10.

The following are more advanced and/or specialized books:

* [A Modern Introduction to Online Learning](https://arxiv.org/pdf/1912.13213.pdf) by Orabona. Excellent coverage of contemporary (circa 2019) online learning.
* [Lectures on Modern Convex Optimization](http://www2.isye.gatech.edu/~nemirovs/LMCO_LN2019NoSolutions.pdf) by Nemirovski. Comprehensive treatment of topics such as conic programming, SDPs, interior point methods, and mirror descent/mirror prox-type algorithms. I reopen Chapter 5 of these lecture notes on a yearly basis for various papers.
* [Fundamentals of Convex Analysis](https://www.amazon.com/Fundamentals-Convex-Analysis-Grundlehren-Editions/dp/3540422056/ref=sr_1_1?dchild=1&keywords=fundamentals+of+convex+analysis&qid=1589590457&s=books&sr=1-1) by Hiriart-Urruty and Lemaréchal. A nice text for a more mathy treatment of convex analysis.
* [First-Order Methods in Optimization](https://my.siam.org/Store/Product/viewproduct/?ProductId=29044686) by Amir Beck. This is a good source for things like proximal algorithms and ADMM. Only recommended if you're directly interested in these types of algorithms.



## Game Theory Foundations
The AGT book has excellent introductions to many areas of game theory, targeted at computer scientists.

* [ Algorithmic Game Theory (AGT) ](http://www.columbia.edu/~ck2945/files/algorithmic-game-theory.pdf)  by Nisan, Roughgarden, Tardos, and Vazirani (it's free). Most relevant to my research is Chapters 1-6, and 9-11.

If one is interested in auction theory, then the following book is a good starting point:

* [Auction Theory](https://www.amazon.com/Auction-Theory-Vijay-Krishna/dp/0123745071) by Vijay Krishna

The following are useful but slightly more topical in nature:

* [ Multiagent Systems (MS) ](http://www.masfoundations.org/download.html) by Leyton-Brown & Shoham (it's free)
* [Twenty Lectures on Algorithmic Game Theory (TLAGT)](https://www.cambridge.org/us/academic/subjects/computer-science/algorithmics-complexity-computer-algebra-and-computational-g/twenty-lectures-algorithmic-game-theory?format=PB) by Tim Roughgarden (the individual notes can be found on [Tim's website](http://timroughgarden.org/notes.html) under the course "Algorithmic Game Theory"). Highly recommend reading these on the particular topics that interest you.
* [Lecture notes](http://www.columbia.edu/~ck2945/courses/s20_8100/) from my PhD class.

## Probability Theory


While not of primary importance in my research, I sometimes find myself needing to use concentration inequalities under various assumptions. When that happens, I consult the below resources.

* [Wikipedia](https://en.wikipedia.org/wiki/Concentration_inequality) This gives a nice overview of quite a few of the most useful concentration inequalities
* [Concentration Inequalities](http://www.econ.upf.edu/~lugosi/mlss_conc.pdf) by Boucheron, Lugosi, and Bousquet. When Wikipedia fails you, this short text can sometimes be of help.

## Linear Algebra and Other Math
It is a truth universally acknowledged, that a researcher in possession of a good problem, must be in want of linear algebra. 

* [Numerical Linear Algebra](https://www.amazon.com/Numerical-Linear-Algebra-Lloyd-Trefethen/dp/0898713617) by Trefethen and Bau III. This books is great for building linear algebra intuition. Read and reread parts I, II, and V. Factorizations such as QR and SVD are incredibly helpful in understanding problems in machine learning, optimization, AI, statistics, etc.

* [The Cauchy-Schwarz Master Class: An Introduction to the Art of Mathematical Inequalities](https://www.amazon.com/gp/product/052154677X/ref=x_gr_w_bb_glide_sin?ie=UTF8&tag=x_gr_w_bb_glide_sin-20&linkCode=as2&camp=1789&creative=9325&creativeASIN=052154677X&SubscriptionId=1MGPYB6YW3HWK55XCGG2) by J. Michael Steele. This book helps develop problem-solving skills, and having a strong grasp of Cauchy-Schwarz, AM-GM, etc is very valuable. This is my favorite book for seeing the fun side of math. Not as important as other books listed here, from a strict foundations perspective.


## Computer Science Foundations

* [Algorithm Design](https://www.pearson.com/us/higher-education/program/Kleinberg-Algorithm-Design/PGM319216.html) by Kleinberg and Tardos. Being able to recognize when a problem is NP-hard, and proving it, is an important skill when working on combinatorial problems; even if one does applied research! For example, it tells you when you need to think about integer-programming rather than convex optimization.

## Programming Skills

The following pieces of numerical software provide a good foundation that enables most research that I do. It's all based on a python stack. A reasonable alternative is [julia](https://julialang.org/) with the incredible [JuMP](https://www.juliaopt.org/JuMP.jl/stable/) package for mathematical optimization. Just beware that python is more likely to be used in industry.

* [numpy](https://numpy.org/)  A general familiarity with numpy and scipy is extremely useful for running simulations, testing hypotheses, or implementing algorithms. I recommend installing via the [anaconda](https://www.anaconda.com/download/) distribution.

* [CVXPY](https://www.cvxpy.org/). CVXPY is great for easily constructing mathematical programs and solving them with a variety of solvers. 

* [Gurobi](https://www.gurobi.com/) get a free academic license and install this as a backend to CVXPY. It's the best way to solve linear programs and mixed-integer programs.

* [Mosek](https://www.mosek.com/) get a free academic license and install this as a backend to CVXPY. It's the best way to solve certain conic programs, such as those for computing market equilibria.

It's also important to be able to do data analysis/plotting. For those purposes Pandas and seaborn are good python packages. That said, the R tidyverse is incredibly good for data analysis. I find it much more enjoyable to work with than python. If you're willing to learn two languages, I recommend:

* [R for Data Science](https://r4ds.had.co.nz/) by Grolemund and Wickham. 
