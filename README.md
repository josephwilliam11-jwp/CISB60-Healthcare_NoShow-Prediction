# Predicting Patient Appointment No-Shows Using Machine Learning and Deep Learning

## About This Project

For my CISB 60 final project at Mt. San Antonio College, I explored whether machine learning and deep learning could help predict which patients are more likely to miss their scheduled medical appointments.

I chose this topic because I work in healthcare and understand how missed appointments can affect scheduling, staff productivity, and patient care.

## Dataset

I used the Medical Appointment No Shows dataset from Kaggle. It contains 110,527 appointment records from healthcare facilities in Brazil in 2016.

I reviewed and cleaned the dataset before building my models. I also looked at patient ages, appointment waiting times, and attendance patterns.

Dataset: https://www.kaggle.com/datasets/joniarroba/noshowappointments/data

## Models Used

I compared three approaches:

- Random Forest classifier
- Artificial Neural Network using TensorFlow/Keras
- Tuned Random Forest using GridSearchCV

I evaluated the models using accuracy, precision, recall, and F1-score.

## Model Results

| Model | Accuracy | Precision | Recall | F1-Score |
|---|---|---|---|---|
| Random Forest | 77.80% | 40.17% | 20.32% | 26.99% |
| Artificial Neural Network | 79.82% | 50.94% | 1.81% | 3.50% |
| Tuned Random Forest | 63.05% | 31.98% | 73.63% | 44.59% |

## What I Learned

One of the biggest things I noticed was that patients with longer waiting times had higher no-show rates in this dataset.

The tuned Random Forest identified more missed appointments than the other models, although it also incorrectly flagged more patients who attended.

This helped me understand why accuracy alone isn't always the best way to evaluate a model, especially when the goal is to identify patients who might miss appointments.

## Tools Used

Python, Pandas, NumPy, Matplotlib, Scikit-learn, TensorFlow/Keras, and Jupyter Notebook.

## Limitations

The dataset is from Brazil in 2016, so the results might not represent current healthcare settings in the United States. The models would need additional testing before being used in an actual healthcare organization.
