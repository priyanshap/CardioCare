# CardioCare
CardioCare-Predictive ML Model for Heart Disease Risk

Implemented Logistic Regression to predict the likelihood of cardiovascular disease (CVD) in patients, focusing on identifying high-risk individuals.

## Data Preparation:
The dataset (framingham.csv) is loaded using Pandas, and initial data cleaning steps include dropping the 'education' column, renaming 'male' to 'Sex_male', and removing rows with missing values (NaN).

## Exploratory Data Analysis:
Basic exploration includes printing the head of the dataset, its shape, and value counts of the target variable (TenYearCHD), which indicates the presence of coronary heart disease (CHD) within ten years.

## Feature Selection and Normalization:
Selected features (age, Sex_male, cigsPerDay, totChol, sysBP, glucose) and target variable (TenYearCHD) are converted into NumPy arrays. Features are then normalized using StandardScaler from sklearn.preprocessing.

## Train-Test Split:
The dataset is split into training and testing sets (70% training, 30% testing) using train_test_split from sklearn.model_selection.

## Visualization:
A count plot (sns.countplot) visualizes the distribution of the target variable (TenYearCHD), showing how many individuals are affected by CHD.

## Logistic Regression Model:
A logistic regression model is implemented using LogisticRegression from sklearn.linear_model, fitted on the training data, and predictions are made on the test set.

## Model Evaluation:
Model accuracy is calculated using accuracy_score from sklearn.metrics, and a confusion matrix (confusion_matrix) with detailed metrics (classification_report) is generated to evaluate the model's performance.
Overall, this project involves preprocessing data, exploring its distribution, applying machine learning techniques (specifically logistic regression), and evaluating the model's predictive accuracy and performance using standard metrics. It aims to predict the likelihood of CHD based on selected health parameters from the Framingham Heart Study dataset.


