# Heart-Disease-in-Hospital-Prediction-using-ANN
## 1. **Brief Introduction**
In the healthcare industry, predicting the likelihood of heart disease based on patient data (such as age, cholesterol levels, blood pressure, etc.) can significantly improve diagnosis accuracy and early intervention. The goal of this project is to use a deep learning model, specifically an Artificial Neural Network (ANN), to classify patients as at risk (1) or not at risk (0) of heart disease, based on a dataset containing medical records.

## 2. **What activation function would you use in the output layer and why?**
In this case, since the task is a binary classification problem (predicting heart disease or not), the most suitable activation function for the output layer would be the Sigmoid activation function. This is because the Sigmoid function outputs a probability value between 0 and 1, making it ideal for binary classification tasks. The output of the Sigmoid function can be interpreted as the probability that the patient has heart disease, where:

- 0 indicates no disease (0% probability),

- 1 indicates the presence of disease (100% probability).

## 3. **How would you handle class imbalance if *has_disease = 1* is rare?**
When the target class (patients with heart disease) is underrepresented, the model might get biased towards the majority class (patients without heart disease). To handle this class imbalance, the following strategies can be used:

- **Class Weight Adjustment** : Assign higher weights to the minority class during training, so the model gives more importance to predicting the minority class (heart disease).

- **Resampling** : Either oversample the minority class or undersample the majority class to balance the dataset.

- **Synthetic Data Generation** : Use techniques like SMOTE (Synthetic Minority Over-sampling Technique) to generate synthetic samples for the minority class.
