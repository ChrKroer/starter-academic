---
title: Economics, AI, and Optimization

summary: PhD class on how AI and optimization enables large-scale economic solution concepts.

# Schedule page publish date (NOT talk date).
publishDate: "2019-12-03T00:00:00Z"
date: "2020-01-21T13:00:00Z"
date_end: "2020-05-01T15:00:00Z"

semester: "Spring"
year: "2020"

authors: []
tags: []

# Is this a featured course? (true/false)
featured: false


# Enable math on this page?
math: true
---

### Course Info

* *Instructor:* [ Christian Kroer ](http://www.christiankroer.com)
* *Time:* Mondays & Wednesdays 1:10-2:25pm
* *Location:* 233 Mudd
* *Office hours:* Wednesday 2:25-3:30pm (or anytime; but email me first in that case)

### Course Summary
Economics, AI, and Optimization is an interdisciplinary course that will cover selected topics at the intersection of economics, operations research, and computer science. A recurring theme in the course will be how economic solution concepts are enabled at scale via AI and optimization methods. We will describe several successful practical applications, including how to:

* Make a poker AI
* Fairly allocate course seats to students, food to food banks, etc
* Protect wildlife or airports
* Conduct large-scale auctions for spectrum or Internet ads

### Course Structure

The course will be lecture-based, with Christian Kroer giving the lectures. At the end of the course there will be a few lectures of project presentations by students.

Readings will consist of a mixture of textbooks and course notes, which will be uploaded after lectures.

Students will complete a project, which may be done individually or in groups of 2-3 students. 

Grading will be as follows:

* 50% final project write-up
* 20% homework (there will only be 1-2 homeworks)
* 15% Final project presentation
* 10% Participation
* 5% Project proposal


### Outline
A rough outline is as follows:

* Intro to game theory and market design
* Nash equilibrium
  * Zero-sum games, minimax theorem
  * First-order methods/Online convex optimization/regret minimization in games
  * Deep learning for solving games at scale
  *	How the above is used in making superhuman poker AIs
* Security games
  * Stackelberg equilibrium
  * Basic Stackelberg security game model
  * Mixed-integer programming, deep learning for scaling up
  * Applications to airport, wildlife, power grid security
* Market design
  * Fisher markets and market equilibrium
  * Optimization methods for computing market equilibria
  * Machine learning methods for large markets
  * fair division, course allocation 
  * Internet ad auctions
  * Spectrum auctions

We will also cover some subset of the following:

* Matching markets
* Data science in multiagent systems

### Textbooks

The primary book is:

* [ Algorithmic Game Theory (AGT) ](http://www.columbia.edu/~ck2945/files/algorithmic-game-theory.pdf)  by Nisan, Roughgarden, Tardos, and Vazirani (it's free)

Additionally, we may use some sections of the following books. They are also recommended for supplementary reading:

* [ Handbook of Computational Social Choice (HCSC) ](http://www.cambridge.org/download_file/898428) by Brandt, Conitzer, Endriss, Lang, & Procaccia (it's free, password: cam1CSC)
* [ Multiagent Systems (MS) ](http://www.masfoundations.org/download.html) by Leyton-Brown & Shoham (it's free)
* [Twenty Lectures on Algorithmic Game Theory (TLAGT)](https://www.cambridge.org/us/academic/subjects/computer-science/algorithmics-complexity-computer-algebra-and-computational-g/twenty-lectures-algorithmic-game-theory?format=PB) by Tim Roughgarden (the individual notes can be found on [Tim's website](http://timroughgarden.org/notes.html) under the course "Algorithmic Game Theory")
* [ Introduction to Online Convex Optimization (Hazan) ](https://ocobook.cs.princeton.edu/OCObook.pdf) by Hazan (it's free)
* [ A Modern Introduction to Onlinea Learning (Orabona) ](https://arxiv.org/pdf/1912.13213.pdf) by Orabona (it's free)

### Schedule
| #  | <div style="width:45px">Date</div> | Topic | Reading | Lecture notes |
|---|--------|----------|---|---|
| 1 | 1 / 22 | Introduction | AGT Ch 1 | [Lecture note 1.pdf](http://www.columbia.edu/~ck2945/files/s20_8100/lecture_note_1_introduction.pdf) |
| 2 | 1 / 27 | Introduction to game theory | AGT Ch 1, Hazan Ch 1 | [Lecture note 2.pdf](http://www.columbia.edu/~ck2945/files/s20_8100/lecture_note_2_gt_and_regret.pdf)|
| 3 | 1 / 29 | Hedge, Online convex optimization | Hazan Ch 1, Ch 5.0-5.4 | [Lecture note 3.pdf](http://www.columbia.edu/~ck2945/files/s20_8100/lecture_note_3_oco_and_sion.pdf)|
| 4 | 2 / 3 | Online Mirror Descent | Orabona Ch. 6.0-6.4 | See previous note |
| 5 | 2 / 5 | OMD convergence, Minimax theorem | Orabona Ch. 6.0-6.4 | See previous note |
| 6 | 2 / 10 | Blackwell approachability, regret matching  | [Farina blog](http://www.cs.cmu.edu/~gfarina/2016/approachability/)| [Lecture note 4.pdf](http://www.columbia.edu/~ck2945/files/s20_8100/lecture_note_4_blackwell_rm_rmp.pdf)|
| 7 | 2 / 12 | From Regret to Nash |  | [Lecture note 5.pdf](http://www.columbia.edu/~ck2945/files/s20_8100/lecture_note_5_nash_from_rm.pdf) |<!-- | 7 | 2 / 12 | Extensive-form games, sequence form  |  | | -->
| 8 | 2 / 17 | Extensive-Form Games, DGFs | AGT Ch 3.7 - 3.11 | [Lecture note 6.pdf](http://www.columbia.edu/~ck2945/files/s20_8100/lecture_note_6_extensive_form_games.pdf) |
| 9 | 2 / 19 | Counterfactual Regret Minimization | | See previous note |
| 10 | 2 / 24 | Subgame solving, deep learning | [BS18](https://arxiv.org/pdf/1705.02955.pdf) Sections 1 and 2 (preferably whole paper), [BSA18](http://www.cs.cmu.edu/~noamb/papers/18-NIPS-Depth.pdf) Section 2 (preferably whole paper), [DeepStack](https://arxiv.org/pdf/1701.01724.pdf) sections "DeepStack" and "Deep Counterfactual Value Networks"| [Lecture note 7.pdf](http://www.columbia.edu/~ck2945/files/s20_8100/lecture_note_7_efg_decomposition.pdf) |
| 11 | 2 / 26 | Stackelberg Equilibrium, Security Games | | [Lecture note 8.pdf](http://www.columbia.edu/~ck2945/files/s20_8100/lecture_note_8_stackelberg_games.pdf)|
| 12 | 3 / 2 | Stackelberg wrap-up, Intro to Fair Division | HCSC Ch 11 | [Lecture note 9.pdf](http://www.columbia.edu/~ck2945/files/s20_8100/lecture_note_9_fair_division.pdf) |
| 13 | 3 / 4 | Eisenberg-Gale convex program | AGT Ch 5 & 6 | See previous note |
| 14 | 3 / 11 | Dominant-Resource Fairness | | [Lecture note 10.pdf](http://www.columbia.edu/~ck2945/files/s20_8100/lecture_note_10_drf.pdf) |
| 15 | 3 / 30 | Intro to Auctions | AGT Ch 9 & 10 | [Lecture note 11.pdf](http://www.columbia.edu/~ck2945/files/s20_8100/lecture_note_11_intro_auctions.pdf) |
| 16 | 4 / 1 | Auctions with Budgets - Second Price | [Multiplicative Pacing Equilibria in Auction Markets](https://arxiv.org/abs/1706.07151) | [Lecture note 12.pdf](http://www.columbia.edu/~ck2945/files/s20_8100/lecture_note_12_budgets_in_auctions.pdf) |
| 17 | 4 / 6 | Auctions with Budgets - First Price | [Pacing Equilibrium in First-Price Auction Markets](https://arxiv.org/abs/1811.07166) | [Lecture note 12.pdf](http://www.columbia.edu/~ck2945/files/s20_8100/lecture_note_12_budgets_in_auctions.pdf) |
| 18 | 4 / 8 | Auctions with Budgets - Dynamics | [Learning in Repeated Auctions](https://ygur.people.stanford.edu/sites/g/files/sbiybj5191/f/learning_in_repeated_auctions_with_budgets_regret_and_equilibrium.pdf) | [Lecture note 13.pdf](http://www.columbia.edu/~ck2945/files/s20_8100/lecture_note_13_dynamic_auctions.pdf) |
| 19 | 4 / 13 | Large-Scale Market equilibrium  | | [Lecture note 14](http://www.columbia.edu/~ck2945/files/s20_8100/lecture_note_14_large_scale_market_equilibrium.pdf)|
| 20 | 4 / 15 | Large-Scale Market equilibrium | | See previous note |
| 21 | 4 / 20 | Large-Scale Market equilibrium | | See previous note |
| 22 | 4 / 22 | Indivisible Goods - Fair Division | For trying fair division: http://www.spliddit.org/ | [Lecture note 15](http://www.columbia.edu/~ck2945/files/s20_8100/lecture_note_15_indivisible_fair_division.pdf) |
| 23 | 4 / 27 | Indivisible Goods - Fair Division Algorithms |  | See previous note |
| 24 | 4 / 29 | Indivisible Goods - A-CEEI |  | See previous note |
| 25 | 5 / 4 | Indivisible Goods - A-CEEI |  | See previous note |

<!-- | 20 | 4 / 15 | Large-Scale Market equilibrium - Abstraction | | | -->
<!-- | 21 | 4 / 20 | Indivisible Fair Division | | | -->
<!-- | 22 | 4 / 22 | Max Nash Welfare| | | -->
<!-- | 23 | 4 / 27 | A-CEEI | | | -->
<!-- | 24 | 4 / 29 | Indivisible Fair Division | | | -->
<!-- | 25 | 5 / 3 | Course evals, Field overview (topics left out etc), companies that do this stuff, EAO at Columbia, Conferences and Journals, Q\& A, | | | -->


<!-- | 15 | 3 / 11 | Market equilibrium abstraction,  Internet ad auctions | | | -->
<!-- | 16 | 3 / 16  | A-CEEI: Matching students to courses | [A-CEEI paper](http://www.columbia.edu/~ck2945/papers/a-ceei.pdf), [Solving A-CEEI and applying it at Wharton](http://www.columbia.edu/~ck2945/papers/course_match.pdf) | | -->
<!-- | - | 3 / 18 | Spring break |  | |  -->
<!-- | - | 3 / 23 | Spring break |  | |  -->
<!-- | 17 | 3 / 25 | Allocation of food to food banks | Prendergast. The Allocation of Food to Food Banks. Working paper, 2017. [pdf](https://faculty.chicagobooth.edu/canice.prendergast/research/foodwithmodel.pdf)  | | -->
<!-- | 18 | 3 / 30 | Spectrum auctions | Cramton. Spectrum Auction Design, 2013. [pdf](http://www.cramton.umd.edu/papers2005-2009/cramton-spectrum-auction-design.pdf) Fréchette, Newman, & Leyton-Brown. Solving the Station Repacking Problem. AAAI, 2016. [pdf](http://www.cs.ubc.ca/~kevinlb/pub.php?u=2016-AAAI-SATFC.pdf) | | -->
<!-- | 19 | 4 / 1 |  | | | -->
<!-- | 20 | 4 / 6 |  | | | -->
<!-- | 21 | 4 / 8 |  | | | -->
<!-- | 22 | 4 / 13 |  | | | -->
<!-- | 23 | 4 / 15 |  | | | -->
<!-- | 24 | 4 / 20 |  | | | -->
<!-- | 25 | 4 / 22 |  | | | -->
<!-- | 26 | 4 / 27 |  | | | -->
<!-- | 27 | 4 / 29 |  | | | -->
<!-- | 28 | 5 / 4 |  | | | -->


### Related Courses

Below is a list of related courses at other schools. 

| Professor | Title | Year | School |
|-----------|-------|------|--------|
| John P. Dickerson | [ Applied Mechanism Design for Social Good ](https://www.cs.umd.edu/class/spring2018/cmsc828m/) | 2018 | UMD |
| Fei Fang | [ Artificial Intelligence Methods for Social Good ](https://feifang.info/artificial-intelligence-methods-for-social-good-spring-2018/) | 2018 | CMU |
| Yiling Chen | [ Topics at the Interface between Computer Science and Economics ](https://canvas.harvard.edu/courses/9622) | 2016 | Harvard |
| Vincent Conitzer | [ Computational Microeconomics: Game Theory, Social Choice, and Mechanism Design ](http://www.cs.duke.edu/courses/spring16/compsci590.4/) | 2016 | Duke |
| Sanmay Das | [ Multi-Agent Systems	 ](http://www.cse.wustl.edu/~sanmay/teaching/cse516-spring16/) | 2016 | Wash U |
| Ariel Procaccia | [ Truth, Justice, and Algorithms ](http://www.cs.cmu.edu/~arielpro/15896s16/index.html) | 2016 | CMU |
| Milind Tambe | [ Security and Game Theory	 ](http://teamcore.usc.edu/Courses/ISE599/) | 2016 | USC |
| Constantinos Daskalakis | [ Games, Decision, and Computation ](https://stellar.mit.edu/S/course/6/sp15/6.891/index.html) | 2015 | MIT |
| Tuomas Sandholm | [ Foundations of Electronic Marketplaces	 ](http://www.cs.cmu.edu/~sandholm/cs15-892F15/cs15-892.htm) | 2015 | CMU |
| Tim Roughgarden | [ Algorithmic Game Theory	 ](http://timroughgarden.org/f13/f13.html) | 2013 | Stanford |
