# THE EFFECTS OF ARM NUMBER & VARIANCE ON MULTI-ARMED BANDITS

## Introduction
The multi-armed bandit problem is a great demonstration of the efficacy of various algorithms for reinforced learning. It involves giving an algorithm a set of 'slot machine' levers to pull and letting it decide which lever to pull next. The problem presents a unique challenge for an algorithm to balance between exploration versus exploitation in choosing which lever is the most advantageous choice. Some algorithms are completely exploratory - pulling levers to gather more information about their environment. Others are completely exploitative - strategically selecting the most lucrative option based on past and current estimations of each arm's output. The remaining algorithms are somewhere in between, balancing learning with exploiting in various ways.

## Setup
For the purposes of this project, four different algorithms and their rates of success on a multi-armed bandit environment were analyzed. These algorithms include Random Selection, Greedy, Epsilon-Greedy, and Softmax. To compare them, a Monte-Carlo style setup was implemented to produce an optimized average accumulative award for each algorithm over a set of 100 runs. The number of pulls an algorithm takes before running out of a set amount of 'money' M was also calculated as a means of endurance analysis, assuming that each algorithm starts with the same M value and each pull produces a positive (or negative) reward.

## Results
Two main factors were tested to see how they influenced the outputs of each algorithm: the effects of manipulating the arm numbers as well as the variance between the arms' payout distributions. It was found that increasing the number of Bandit arms heightened the efficiency of the Softmax and Epsilon-Greedy algorithms, whereas the Greedy and Random Selection algorithms excelled at lower arm numbers. Variance affected outputs in the opposite way, where high variance favored the luck-influenced Greedy and Random Selection algorithms, and low variance favored the strategizing Softmax and Epsilon-Greedy algorithms.

## License
This work is public domain.
