## Contributors

1. Darren Chia
2. Keng
3. Jared

This is a mini project for SC1015 (INTRO TO DATA SCI & ART INTELLIGENCE). The project focuses on mental health from [Kaggle](https://www.kaggle.com/datasets/michaelacorley/unemployment-and-mental-illness-survey). This repository contains all the Jupyter Notebooks, datasets, images, video presentations, and the source materials/references we have used and created as part of the Mini Project for SC1015: Introduction to Data Science and AI.

## Table of content
  1. Problem Formulation
  2. Data Preparation and Cleaning
  3. Exploratory Data Analysis
  4. Random Forest
  5. Dectree
  6. Neural Network
  7. Logistic Regression
  8. SVM
  9. Conclusion


## 1. Problem Formulation

Problem Statement: 1. How can we identidy early mental illness?
                   2. Does mental illness affect employability>

Success: Determined using clear mental health symptoms and features related employment.

Rationale: We believe that this dataset as well as the question is relavant to Singaporean, especically since mental health is a huge concerns. Being a student in NTU, our group would like to use our knowledge to solve real world problems that could benefit many individuals.

## 2. Data Preparation and cleaning

In this section of the project, we prepared and cleaned the data to help us analyze our data better so that it matches our problem statment.

We performed the following:

 1. Features selection: We remove features deem as unhelpful to our project and 13 features were dropped.
 2. Missing entries: We replaced missing entries with 0, with the assumption that they do not have problem related to the features.
 3. Replacing categorial data: We replace categorical data to numerical e.g. (Male/Female to 1/0) 
 4. Standardization: We standardize our features name, coverting the name to uppercase and space to underscore.


## 3. Exploratory Data Analysis
Then we process to split the dataset into 2 seperate parts one focusing on mental health and other focus on employment. We explored the 2 dataframes by generating correlation matrix to find out features with the strongest correlation.

To achieve this:
1. Generate correlation matrix one for mental health and other for employment
2. Explored the features with strongest correlation between mental health and employment
3. Study if any other feature could be a factor for mental health/employment

## 4. Random Forest

Reason: We perform random forest, which combine multiple decision trees to improve prediction accuracy, enabling us to fit categorical and numerical date into the model.

## 5. Dectree

Reason: We wanted a highly interpretable model that could also address mental health issues and unemployment. Unfortunetely, by using this model we sacrificed reliability in exchange for more interpretable result.

## 6. Neural Network

Reason: We wanted a model that could learn complex patterns and representations from data, that could provide a more valuable insight between mental health and employment.

## 7. LogisticRegression

Reason: We wanted a model that includs interpretability and efficiency, while able to incoporate categorical data. It similar to linear regression as both provides coefficient and probability, making it valuable for discerning relationships between features and the target variables such as mental health and employment.

## 8 SVM

Reason: We choose svm for its effectiveness in high-dimensional spaces, making them suitable for datasets with numerous feature. The model ability to perform classification betwwen class were also part of the reason why we choose this model.

## Conclusion
In summary, the selection of decision trees, SVM, neural networks, random forests, and logistic regression is driven by their respective strengths in interpretability, handling high-dimensional data, learning complex patterns and providing probabilistic interpretations. Notably we found out that having clear mental health symptoms does affect employment since we choose feature related to mental health to predict employment, and the confusion matrix generate indicates little false positive and negative.

## References
- https://www.kaggle.com/datasets/michaelacorley/unemployment-and-mental-illness-survey
- https://www.simplilearn.com/tutorials/machine-learning-tutorial/random-forest-algorithm#:~:text=Step%201%3A%20Select%20random%20samples,as%20the%20final%20prediction%20result.
- https://www.w3schools.com/python/python_ml_logistic_regression.asp
- https://www.datacamp.com/tutorial/svm-classification-scikit-learn-python
- https://www.analyticsvidhya.com/blog/2021/09/introduction-to-artificial-neural-networks/#:~:text=An%20Artificial%20Neural%20Network%20(ANN)%20is%20a%20machine%20learning%20model,learn%20patterns%20and%20make%20predictions.



