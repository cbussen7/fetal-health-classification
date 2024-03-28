# fetal-health-classification

In this project I was tasked with developing an algorithm in R to give automated predictions of fetal health (the variable NSP) using data taken from fetal cardiotocograms (CTGs). In the training data, the variable NSP has been labeled by doctors. The variable meanings are given below.

- LB - FHR baseline (beats per minute)
- AC - # of accelerations per second
- FM - # of fetal movements per second
- UC - # of uterine contractions per second
- DL - # of light decelerations per second
- DS - # of severe decelerations per second
- DP - # of prolongued decelerations per second
- ASTV - percentage of time with abnormal short term variability
- MSTV - mean value of short term variability
- ALTV - percentage of time with abnormal long term variability
- MLTV - mean value of long term variability
- Width - width of FHR histogram
- Min - minimum of FHR histogram
- Max - Maximum of FHR histogram
- Nmax - # of histogram peaks
- Nzeros - # of histogram zeros
- Mode - histogram mode
- Mean - histogram mean
- Median - histogram median
- Variance - histogram variance
- Tendency - histogram tendency
- CLASS - FHR pattern class code (1 to 10)
- NSP - fetal state class code (N=normal; S=suspect; P=pathologic)

To accomplish this goal, I created several models I expected might work for the given scenario, including multinomial regression, decision trees (regular and pruned), random forests, and support vector machines. Throughout this process, I also experimented with models with reduced dimensionality by performing both stepwise feature selection as well as Principle Component Analysis (PCA). Once the models were created, I analyzed which had the best performance.
