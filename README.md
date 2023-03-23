# Heart Disease Prediction
### CSE4020- Machine Learning Project 

---
#### Modules Implemented:

1. Data Pre-processing: The heart disease dataset was imported from the UCI repository and loaded. It contains several
health parameters like age, sex, chest pain type, resting blood pressure, serum cholesterol in
mg/dl, maximum heart rate achieved, etc that affect a person’s heart. The raw data was processed
to make it compatible with the machine learning algorithm. We checked if the dataset contained
missing/null values. Since the dataset was already clean, we further went to the exploratory data
analysis part.

2. Exploratory Analysis: Before training the model, we need to observe and analyze the data to see what we are working
with. The goal is to learn more about the data, the different types of data, outliers, and how to
handle them. In our dataset, the target variable decides if a particular person has heart disease or
not. 1 represents a defective heart and 0 represents a non-defective heart. The pie chart
distribution of the target shows that over 50% of people suffer from heart diseases. The
distribution of sex and target variables shows that the ratio of males with heart disease is slightly
greater than that of females with heart disease. The plot distribution of age and target variable
shows that people over the age of 40 have a higher risk of suffering from heart disease, and the
distribution of cholesterol levels and target shows that most people who get heart diseases have
cholesterol levels of over 200 mg/dl. The distribution of blood pressure and target variable
implies that over 50% of the patients have higher blood pressure (more than 120 mmHg)
irrespective of whether they have heart disease or not.

3. Training and Testing: The next step is to split the data into training and testing data to train our machine learning
algorithm with the training data and evaluate the model’s performance using the testing data.

4. Performance Evaluation: We need to find the best model for our training data. For this purpose, we've taken three
algorithms- Logistic Regression, Random Forest, SVM, Decision Tree, and XGBoost Classifiers.
We then computed the accuracy scores of these models and visualized them using a barplot. We
inferred that the SVM model gave the highest accuracy. We performed hyperparameter tuning of
these models. But the results don't improve much since the dataset is small. These ML models
were stacked using Kfold with KNN as the final estimator, and the performance accuracy of this
stacking ensemble was computed. We found that it gave the highest accuracy score of 90% and
performed better than the other single base models.

