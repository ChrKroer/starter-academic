---
title: Optimal Mechanism Design via Optimal Transport
date: 2020-12-02
math: true
draft: true
diagram: true

---


$\newcommand{\mP}{{\mathcal P}}$
$\newcommand{\mT}{{\mathcal T}}$
$\newcommand{\mM}{{\mathcal M}}$
$\newcommand{\mU}{{\mathcal U(X)}}$
$\newcommand{\mL}{{\mathcal L_1(X)}}$


Suppose that you have $n$ goods that you wish to sell to a single buyer. That buyer draws their valuation from a density $f$ on the space of possible valuations. How should you do this?
This post will explain an approach based on optimal transport.

### Mechanism Design Problem
More specifically, we assume that valuations are additive across the goods, and they come from the compact space 
$X = \prod_{i=1}^n [x_i^{\text{low}}, x_i^{\text{high}}]$, where $0 \leq x_i^{\text{low}} \leq x_i^{\text{high}}$.
The valuation vector is drawn according to a density function $f: X \rightarrow \mathbb R_+$ which is assumed to be continuous and differentiable, with bounded partial derivatives. 

A mechanism $\mathcal M$ lets the buyer report a valuation $x$ and then receive a (potentially randomized) allocation of goods, along with a payment. More concretely, the mechanism consists of:
- an allocation function $\mathcal P: X \rightarrow [0,1]^n$  specifying the vector of probabilities $\mathcal P(x)$ that the buyer receives each good upon reporting a valuation vector $x$.
- a payment function $\mathcal T: X \rightarrow \mathbb R$ specifying how much the buyer pays upon reporting $x$.

A few comments about this setup are in order. First, our allocation function $\mP$ returns probabilities. This means that we are potentially going to allow our mechanism to assign items fractionally, or in other words, sell lottery tickets. Second, we are constraining ourselves to mechanisms that take a reported valuation vector, yielding an allocation probability and payment.
By the [revelation principle](https://en.wikipedia.org/wiki/Revelation_principle), direct mechanisms such as the above, where the buyer reports their valuation vector, are without loss of generality.

We will assume that the buyer is interested in maximizing their expected utility. For a given type $x$, reporting type $x'$ yields expected utility $\langle x, \mP(x') \rangle - \mT(x')$.

Our goal will be to find $\mP$ and $\mT$ such that we have the following two conditions:
* Incentive compatibility: for any buyer typer $x\in X$, reporting $x$ should yield at least as much utility as reporting any other type $x'\in X$:
$$\langle x, \mP(x) \rangle - \mT(x) \geq \langle x, \mP(x') \rangle - \mT(x')$$
* Individual rationality: for any buyer typer $x\in X$, participating truthfully in the mechanism should yield nonnegative utility:
$$\langle x, \mP(x) \rangle - \mT(x) \geq 0$$

Subject to these constraints, we wish to pick the mechanism that maximizes revenue when the buyer reports truthfully. The revenue for a particular pair $\mP,\mT$ is:
$$ \int_X \mT(x) f(x)dx $$


### Reducing optimal mechanism design to that of finding truthful utility functions

A classical result due to Rochet (1987) states that the set of IC and IR mechanisms can be characterized in terms of utility functions that are induced by reporting truthfully under the mechanism. The induced utility $u$ associated to a mechanism $\mP,\mT$ is the expected value that a given type gets for reporting truthfully:
$$ u(x) = \langle x, \mP(x) \rangle - \mT(x)$$

Rochet's characterization states that a mechanism $\mM$ is IC and IR if and only if its induced utility function $u$ is convex, nonnegative, nondecreasing, and $1$-Lipschitz with respect to the $\ell_1$ norm. Moreover, given such a function $u$ which is differentiable, a corresponding IC and IR mechanism can be constructed by setting $$\mP(x) = \nabla u(x),\quad \mT(x) = \langle \nabla u(x), x\rangle - u(x).$$
If $u$ is not differentiable then for the measure-zero points of nondifferentiability, a similar construction can be performed using subgradients.

Let $\mU$ be the set of continuous, convex, and nondecreasing functions on $X$. Let $\mL$ be the set of all $1$-Lipschitz functions on $X$.
With the above characterization in mind, we can reduce our search for an optimal mechanism to the problem of optimizing over the intersection $\mU \cap \mL$, with the additional constraint of nonnegavitiy. The revenue for a given $u$ is
$$ \int_X \left[ \langle \nabla u(x), x\rangle - u(x) \right] f(x)dx $$
and it follows that an optimal mechanism is derived from a solution $u$ to the optimization problem
\begin{align}
 \max_{u \geq 0} & \int_X \left[ \langle \nabla u(x), x\rangle - u(x) \right] f(x)dx \\\\
 \text{s.t.}\ \ & u \in \mU \cap \mL
\end{align}

test


### References
* Rochet, J. C. (1987). A necessary and sufficient condition for rationalizability in a quasi-linear context. Journal of mathematical Economics, 16(2), 191-200.

