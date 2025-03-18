Heart Disease DataScience/Machine Learning Capstone for Coding Nomads

![Heart Giphy](https://github.com/user-attachments/assets/9ec55a36-5020-4297-b900-e7176bfe13d1)

Background:

Cardiovascular diseases are the primary cause of death throughout the world (approximately 20.5 million deaths), & carry large health care costs, with cost estimates over $400B for the period of 2018-2019. While preventive and medical interventions are effective in reducing cardiovascular disease, screening to diagnose heart disease before it becomes clinically apparent can reduce both the medical and economic burden.


Purpose:

The purpose of this report was to train a mode using a dataset from the Centre for Disease Control (CDC) & evaluate the model’s ability to accurately predict patients with heart disease. An ML predictive model would be instrumental as an early warning system against heart disease, the world’s number one killer.


What were the Results?

The data were imbalanced so Synthetic Minority Over-Sampling Technique (SMOTE) & Balanced Random Forest (BRF) Classifier were used to improve recall scores. The SMOTE technique generates synthetic data points (instead of duplicating existing ones). The technique identifies the k-nearest neighbours (KNN) of the minority class and creates new samples along the original line segments. This technique prevents overfitting and balances the dataset before training. The BRF randomly undersamples the majority class, so that the model is trained on a balanced subset (equal samples are used from each of the majority and minority classes).  
Balanced Random Forest yielded a recall of 0.79, and a receiver operating characteristics area under the curve of 0.83. While the 0.83 value shows a good predictive ability, the model is not recommended for use in clinical setting. 


What does the Reader gain?

The reader gains an opportunity on learning how to deal with an imbalanced dataset.



