# Heart Disease Prediction Using Machine Learning
![Heart Giphy](https://github.com/user-attachments/assets/9ec55a36-5020-4297-b900-e7176bfe13d1)
## Overview

Cardiovascular diseases are the leading cause of death globally, with approximately 20.5 million deaths annually. The economic burden is also significant, with costs estimated to exceed $400 billion for the 2018-2019 period. While preventive and medical interventions are effective in reducing cardiovascular diseases, diagnosing heart disease before it becomes clinically apparent can significantly reduce both medical and economic costs.

This project focuses on training a machine learning model to predict heart disease using a dataset from the **Centre for Disease Control (CDC)**. The goal is to evaluate the model's ability to accurately predict patients who are at risk for heart disease. An accurate predictive model could serve as an early warning system, helping reduce the world’s number one killer.

## Problem Statement

The main problem tackled in this project was the imbalance of the data, where there are significantly more non-disease cases than disease cases. This imbalance can negatively affect the performance of machine learning models, especially in terms of sensitivity (recall).

## Dataset

The dataset used in this project comes from the **CDC** and contains multiple features relevant to heart disease prediction, such as age, cholesterol levels, blood pressure, and others.

*Link to Dataset:*  
Provide a link to the dataset if publicly available, or you can describe the data’s source in more detail here.

### Data Preprocessing

To address data imbalance, we implemented the following techniques:
- **SMOTE (Synthetic Minority Over-sampling Technique)**: This method generates synthetic data points for the minority class (patients with heart disease) to balance the dataset.
- **Balanced Random Forest Classifier**: This technique was used to improve recall scores by adjusting the weights of each class during model training.

## Model Development

### Algorithms Used
- **Balanced Random Forest Classifier**: The main model used for training. This classifier is specifically designed to handle imbalanced data by modifying how trees are built to reduce bias towards the majority class.

### Performance Evaluation
The model was evaluated using several metrics:
- **Recall**: The model achieved a recall score of 0.79, meaning it correctly identified 79% of actual heart disease cases.
- **ROC AUC**: The model achieved a Receiver Operating Characteristic (ROC) Area Under the Curve (AUC) score of 0.83. This indicates that the model has good predictive ability, distinguishing between patients with and without heart disease.

### Model Limitations
While the model performed well with a recall of 0.79 and an AUC of 0.83, it is not recommended for clinical use due to potential false positives and other limitations that need to be addressed for real-world applications.

## Key Learnings

- **Handling Imbalanced Data**: One of the main challenges was dealing with imbalanced data, and we used SMOTE and the Balanced Random Forest Classifier to mitigate this issue.
- **Evaluation Metrics**: Understanding and choosing the right evaluation metrics (like recall and AUC) is crucial when working with imbalanced datasets, especially in a medical context where false negatives are more costly.
- **Model Deployment Considerations**: Although the model shows promise, deploying it in a clinical setting requires further validation, calibration, and integration with healthcare systems.

## Conclusion

This project demonstrates the potential of machine learning in predicting heart disease and its importance as an early warning system. Although the model achieved good predictive performance, further work is needed to enhance its accuracy and ensure its suitability for real-world clinical applications.

## Next Steps / Future Work

- **Model Optimization**: Further fine-tuning and experimenting with different models and techniques could help improve the model’s performance.
- **Feature Engineering**: Investigating additional or more relevant features could enhance predictive accuracy.
- **Clinical Validation**: Collaborating with healthcare professionals to validate the model’s performance in real-world clinical settings.

## Code and Implementation

You can find the complete code for this project in the [GitHub Repository](https://github.com/FrankF2025/DSML_Capstone_Heart_Disease/tree/main).

Here is a brief overview of the key steps involved in the project:

### Step 1: Data Collection
- Import and explore the dataset.

### Step 2: Data Preprocessing
- Handle missing values, normalize/scale data, and address imbalanced data using SMOTE.

### Step 3: Model Training
- Train a Balanced Random Forest Classifier on the dataset.

### Step 4: Model Evaluation
- Evaluate the model using various metrics, including recall and ROC AUC.

### Step 5: Model Interpretation
- Interpret the model's results and assess its performance.

## References

- [SMOTE Paper](https://arxiv.org/abs/1106.1813) - Chawla et al., 2002
- [Balanced Random Forest Classifier Paper](https://www.ijcai.org/Proceedings/15/Papers/420.pdf)

## Acknowledgments

Thank you to the **CDC** for providing the dataset and the open-source community for the tools and libraries that made this project possible.

