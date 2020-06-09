# Background
Auto loans, mortgages, student loans, debt consolidation ... these are just a few examples of credit and loans that people are seeking online. Peer-to-peer lending services such as LendingClub or Prosper allow investors to loan other people money without the use of a bank. However, investors always want to mitigate risk, so you have been asked by a client to help them use machine learning techniques to predict credit risk.

In this assignment, you will build and evaluate several machine-learning models to predict credit risk using free data from LendingClub. Credit risk is an inherently imbalanced classification problem (the number of good loans is much larger than the number of at-risk loans), so you will need to employ different techniques for training and evaluating models with imbalanced classes. You will use the imbalanced-learn and Scikit-learn libraries to build and evaluate models.

# Resampling
**Which model had the best balanced accuracy score?**
For resampling we used the following methodologies:
    - Naive random oversampling
    - SMOTE oversampling
    - Undersampling (Cluster Centroids)
    - Combination (SMOTEENN)
The best balanced accuracy scored was for random over-sampler followed very closely by SMOTE. The worst resampling was for undersampling where the score dropped by a considerable amount. 

**Which model had the best recall score?**
The best recall score was for SMOTE. Random over-sampler didn't perform too well in this metric. Undersampling was again the worst methodology.

**Which model had the best geometric mean score?**
Random over-sampler was the best methodology regarding geometric mean score followed by SMOTE.


# Ensamble
**Which model had the best balanced accuracy score?**
We use two different ensamble methodologies: Balanced random forest classifier and the easy ensemble AdaBoost classifier.
The best accuracy was for easy ensemble AdaBoost classifier with a very high 93.33% score.

**Which model had the best recall score?**
The best recall score was also for easy ensemble AdaBoost classifier.

**Which model had the best geometric mean score?**
The best geometric mean score was also for easy ensemble AdaBoost classifier.

**What are the top three features?**

	importance
    - total_rec_prncp	0.071744
    - total_rec_int	0.067427
    - total_pymnt_inv	0.064612