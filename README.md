﻿# Linear regression healthcare cost calculator

In this project, we aim to predict healthcare costs using a regression algorithm. We are provided with a dataset containing information about different people, including their healthcare costs. Our goal is to build a model that can accurately predict healthcare costs based on new data.

## Dataset

The dataset used in this project is sourced from [FreeCodeCamp](https://www.freecodecamp.org/). It contains various attributes such as age, sex, BMI, number of children, smoking status, region, and healthcare expenses. 

### Features
- age: Age of the individual.
- sex: Gender of the individual.
- bmi: Body mass index (BMI) of the individual.
- children: Number of children/dependents covered by healthcare.
- smoker: Smoking status of the individual (yes/no).
- region: Region of the individual (northeast, northwest, southeast, southwest).

### Target Variable
- expenses: Healthcare expenses incurred by the individual.

## Data Preprocessing

- Converted categorical data (sex, smoker, region) into numerical values using one-hot encoding.
- Split the dataset into training (80%) and testing (20%) sets.
- Created separate datasets for features (x) and target variable (y).

## Model Development

We built a neural network regression model using TensorFlow's Keras API.

- **Input Layer:** 50 neurons with ReLU activation function.
- **Hidden Layer:** 25 neurons with ReLU activation function.
- **Output Layer:** 1 neuron (for regression) without activation function.

The model was compiled using the mean absolute error as the loss function and the Adam optimizer.

We applied early stopping to prevent overfitting, monitoring the validation loss and restoring the best weights.

## Model Evaluation

The model was evaluated on the test dataset. The mean absolute error (MAE) was used as the evaluation metric.

The MAE obtained was 2035.08, indicating that the model predicts healthcare costs with an average error of $2035.08.

## Conclusion

The neural network regression model performed well in predicting healthcare costs based on the provided dataset. Further optimizations and fine-tuning can be explored to improve the model's performance.

