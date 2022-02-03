---
title: AI, Games, and Markets

summary: Advanced MS and senior undergraduate class on how to make a poker AI, create an internet advertising market, and more

# Schedule page publish date (NOT talk date).
publishDate: "2019-12-03T00:00:00Z"
date: "2022-01-18T13:00:00Z"
date_end: "2022-05-01T15:00:00Z"

semester: "Spring"
year: "2022"

authors: []
tags: []

# Is this a featured course? (true/false)
featured: false


# Enable math on this page?
math: true
---


## Course Summary
This is a course on how techniques from AI and optimization enable large-scale game solving and market design. We will cover the core ideas behind recent superhuman AIs for games such as Poker and Go. Then, we will discuss how AI and game theory ideas are used in large-scale marketplaces such as internet advertising, recommender systems, and electricity markets. This is intended to be an advanced MS level and senior undergraduate course for students in Operations Research and Financial Engineering. 

We will most likely cover the following applications:

* How to make a go or poker AI
* Market design for large-scale internet advertising auctions
* Electricity market design


# Admin stuff

## Course Info

* *Instructor:* [ Christian Kroer ](http://www.christiankroer.com)
* *Time:* Mondays & Wednesdays 1:10-2:25pm
* *Location:* 702 Hamilton Hall
* *Office hours:* Wednesday 2:25-3:30pm Mudd 314
* *Courseworks site:* [courseworks site](https://courseworks2.columbia.edu/courses/147216)
## Prerequisites

* Mathematical maturity; ability to follow proofs
* Linear algebra: vector and matrix algebra
* Calculus: derivates, optimality conditions, Lagrange multipliers
* Optimization: linear programming, mixed-integer programming (this can potentially be learned along the way)

## Course Structure

The course will be lecture-based, with Christian Kroer giving the lectures. At the end of the course there will be a few lectures of project presentations by students.

Readings will consist of a mixture of textbooks and course notes, which will be uploaded after lectures.

Students will complete a project, which should be done in groups of 3-4 students. Special permission is needed to do an individual project.

Grading will be as follows:

* 50% final project write-up
* 25% homework (there will be 4-5 homeworks)
* 5% Project proposal
* 5% Project milestone report
* 5% Final project presentation
* 10% Participation

## Homework

Homeworks will be posted on courseworks.

Homework lateness policy
* All homeworks due at midnight on stated date
* Everyone gets 3 late days
* If you are handing in late, you must email the TAs and me to say that you are using a late 
day
* Include in the email how many you have used

# Course Content

## Outline
A rough outline is as follows:

* Intro to game theory and market design 
* Market design and the internet
  * Internet advertising auctions
  * Recommender systems
  * Bias and fairness in machine learning and internet advertising
* Fair Resource Allocation
  * Fair division via competitive equilibria
  * Fair course seat allocation 
  * Allocating food to food banks
* Electricity markets
* Nash equilibrium
  * Zero-sum games, minimax theorem
  * No-regret learning
  * Perfect-information games and go AIs, Monte Carlo tree search
  * Imperfect-information games and poker AIs
  * Deep learning for solving games at scale
* Security games with applications to airport, wildlife, power grid security


## Textbooks

The primary book is:

* [ Algorithmic Game Theory (AGT) ](http://www.columbia.edu/~ck2945/files/algorithmic-game-theory.pdf)  by Nisan, Roughgarden, Tardos, and Vazirani (it's free)

Additionally, we may use some sections of the following books. They are also recommended for supplementary reading:

* [ Handbook of Computational Social Choice (HCSC) ](http://www.cambridge.org/download_file/898428) by Brandt, Conitzer, Endriss, Lang, & Procaccia (it's free, password: cam1CSC)
* [ Multiagent Systems (MS) ](http://www.masfoundations.org/download.html) by Leyton-Brown & Shoham (it's free)
* [Twenty Lectures on Algorithmic Game Theory (TLAGT)](https://www.cambridge.org/us/academic/subjects/computer-science/algorithmics-complexity-computer-algebra-and-computational-g/twenty-lectures-algorithmic-game-theory?format=PB) by Tim Roughgarden (the individual notes can be found on [Tim's website](http://timroughgarden.org/notes.html) under the course "Algorithmic Game Theory")
* [ Introduction to Online Convex Optimization (Hazan) ](https://ocobook.cs.princeton.edu/OCObook.pdf) by Hazan (it's free)
* [ A Modern Introduction to Onlinea Learning (Orabona) ](https://arxiv.org/pdf/1912.13213.pdf) by Orabona (it's free)


## Project

Students will complete a semester-long project on topics related to the course. This project can be applied, theoretical, or a mixture.
Students are encouraged to formulate their own project proposals. That said, I will also provide some candidate project topics on courseworks.

Students are welcome to propose a topic of their own. 
Some project ideas can also be found on courseworks.

Project rules:

* Teams should have 3-4 students. Smaller teams require instructor permission.
* You must choose a project by March 23rd
* A one-page project proposal is due March 25th
* A 2-page midterm progress report is due April 15th
* A 5-10 page whitepaper, formatted as a [NeurIPS conference paper](https://neurips.cc/Conferences/2020/PaperInformation/StyleFiles), is due May 8th
* Each team must make a ~20m presentation of their project

## Extremely Tentative Schedule

<div class="schedule">

| #  | <div style="width:45px">Date</div> | Topic | Reading | Lecture notes |
|---|--------|----------|---|---|
| 1 | 1 / 19 | Course Intro |  |  [Lec. note 1](http://www.columbia.edu/~ck2945/files/ai_games_markets/lecture_note_1_introduction.pdf)|
| 2 | 1 / 24 | Intro to game theory and auctions | AGT Ch 1, 2 | [Lec. note 2](http://www.columbia.edu/~ck2945/files/ai_games_markets/lecture_note_2_gt.pdf)|
| 3 | 1 / 26 | Intro to game theory and auctions | AGT Ch 9, 10 | [Lec. note 3](http://www.columbia.edu/~ck2945/files/ai_games_markets/lecture_note_3_intro_auctions_and_mech_design.pdf)|
| 4 | 1 / 31 | Regret Minimization | Lecture note (you may skip the proofs of Theorems 2 and 3) | [Lec. note 4](http://www.columbia.edu/~ck2945/files/ai_games_markets/lecture_note_4_regret_and_sion.pdf)|
| 5 | 2 / 2 | Nash eq. from regret min. | Lect. Note 5 | [Lec. note 5](http://www.columbia.edu/~ck2945/files/ai_games_markets/lecture_note_5_nash_from_rm.pdf)|
| 6 | 2 / 7 |   | | |
| 7 | 2 / 9 | |  | |
| 8 | 2 / 14 |  |  |  |
| 9 | 2 / 16 | | | |
| 10 | 2 / 21 |  | |  |
| 11 | 2 / 23 |  | | |
| 12 | 2 / 28 |  |  |  |
| 13 | 3 / 2 |  |  | |
| 14 | 3 / 7 |  | |  |
| 15 | 3 / 9 |  |  |  |
| 16 | 3 / 14 | <div style="background-color:tomato;">Spring break: no class </div> |  |
| 17 | 3 / 16 | <div style="background-color:tomato;">Spring break: no class </div> |  |
| 18 | 3 / 21 |  |  |  |
| 19 | 3 / 23 |  | | |
| 20 | 3 / 28 |  | | |
| 21 | 3 / 30 |  | | |
| 22 | 4 / 4 |  |  |  |
| 23 | 4 / 6 |  |  |  |
| 24 | 4 / 11 |  |  | |
| 25 | 4 / 13 |  |  | |
| 26 | 4 / 18 |  |  | |
| 27 | 4 / 20 |  |  | |
| 28 | 4 / 25 | Project presentations (Maybe?) |  | |
| 29 | 4 / 27 | Project presentations |  | |
| 30 | 5 / 2 | Project presentations |  | |


</div>

### Related Courses

Below is a list of related courses at other schools. 

<div class="other_courses" >

| Professor | Title | Year | School |
|-----------|-------|------|--------|
| John P. Dickerson | [ Mechanism Design ](https://mech-design.github.io/) | 2022 | UMD |
| Gabriele Farina & Tuomas Sandholm | [ Computational Game Solving ](https://www.cs.umd.edu/class/spring2018/cmsc828m/) | 2021 | CMU |
| Christian Kroer  | [ Economics, AI, and Optimization ](http://www.columbia.edu/~ck2945/courses/s20_8100/) | 2020 | Columbia |
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

</div>
